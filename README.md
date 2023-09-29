# Introduction
This project is inspired by my numerous attempts to solve same two problems using nginx, CORS and 
Proxying HTTPS to another server. It enables you to use just a docker compose combined with your certificates for ssl to do both. This is mostly for one-off setups and surely not production ready.
# Guide:
1. Generate fullcert.pem and privkey.pem certificate files to replace the mocked ones. Certbot is recommended to use.
2. Change the listening port on server in docker compose file (Default: 9999)
3. Change proxied server (target server) in default.conf file (Default: target.example.com)
4. (Optional): Add proxy headers if target server supports those
