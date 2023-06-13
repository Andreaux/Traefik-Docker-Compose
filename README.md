# Traefik-Docker-Compose
A Simple Docker Compose Stack to run Traefik with Cloudflare SSL certificates to provide wildcard SSL certificates to internal Homelab services. This can be used standalone, but was originally intended to go along my Nextcloud all-in-one Docker Compose Stack.

# How to use this package?
1. Create a Cloudflare account and set up DNS the domain you want to use with your HomeLab
2. Create an API key with Cloudflare
3. Edit data/traefik.yml and fill in your Cloudflare-registered e-mail address
4. Create a .env file (or set up environment variables if you're using a package manager like Portainer for example) and fill in your Cloudflare username and API key as well as other variables from docker-compose.yml.
5. Rename default.config.yml into config.yml and enable what you need (or leave as-is for now)
6. Create and launch Traefik with docker-compose up -d

Everything should "just work".

# Support this project
If you find this useful, a coffee through Ko-Fi is all it takes to make me happy <3 (I love coffee :D) Click the Sponsor button on the top of this page or visit https://ko-fi.com/andreaux to buy me a coffee.
