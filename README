# Docker Compose Setup for Certbot

This repository contains a Docker Compose setup to run Certbot for obtaining and managing SSL/TLS certificates using manual DNS validation.

## Prerequisites

- Docker installed on your system
- Docker Compose installed on your system
- A domain name pointing to your server
- Access to your domain's DNS settings

## Steps

- Run the command:

  ```
  docker compose run --rm  certbot certonly -d <your_domain> --manual --agree-tos --email <your_email>
  ```
   
   This command obtains a certificate with certbot for your domain using manual domain validation.
- The response will be certbot asking that your domain has an endpoint to a file containing a validation data. After this is complete, click Enter to continue.
- Certificates will be created in the `letsencrypt/live/<your_domain>` folder in the root folder.
- Run the commands: 
```
sudo chown -R <your_username>:<your_username> ./letsencrypt ; sudo chmod -R 755 ./letsencrypt
```
  
  This will read access to the files in the folders.
- Copy and paste certificates where needed.