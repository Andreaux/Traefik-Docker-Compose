Version: 2.0

# Traefik-Docker-Compose
A Simple Docker Compose File to run Traefik with Cloudflare SSL certificates to provide wildcard SSL certificates to internal Homelab services. This can be used standalone, but it's tailored to go along my Nextcloud all-in-one Docker Compose Stack: https://github.com/Andreaux/Nextcloud-Docker-Compose

## Warning!
If you are using a previous version of this Docker Compose file, this version has transitioned to persisting configuration and certificates on an NFS share. Do not simply update to this version without understanding the difference.

# How to use this package?
1. Create a Cloudflare account and set up DNS for the domain you want to use with your HomeLab
2. Create an API key with Cloudflare
3. Edit data/traefik.yml and fill in your Cloudflare-registered e-mail address
4. Modify the .env file (or set up the same environment variables if you're using a package manager like Portainer for example) and fill in your Cloudflare username and API token or key, as well as the other variables for the docker-compose.yml.
5. Rename default.config.yml into config.yml and enable/set up what you need (or leave as-is for now)
6. Create a folder for the persistent data somewhere and share it with NFS (I use version 4).
You can use a local folder too, in that case remove the NFS definition at the top and change the volume mapping in the compose file -- instructions are there)
7. Create and launch Traefik with docker-compose up -d

Everything should "just work".

# Support this project
If you find this useful, a coffee through Ko-Fi is all it takes to make me happy <3 (I love coffee :D) Click the Sponsor button on the top of this page or visit https://ko-fi.com/andreaux to buy me a coffee.
