# Traefik-https-test
Testing let's encrypt ssl certificates with Traefik using the cloudflare provider.

# What you need : 
- Valid domain with dns management in cloudflare (if you are using another dns provider please check https://docs.traefik.io/configuration/acme/)
- docker

# How to run 
- Change cloudflare.env to match your email/api key for your cloudflare account
- Change the domains/frontends for the cert in docker-compose.yml to point to your backend/containers
- Chage the domains in the traefik.toml in order to get certificates and add your email in the acme section
- hostfile your frontend domains/sub-domains to your localhost
- Run docker-compose up and enjoy!

