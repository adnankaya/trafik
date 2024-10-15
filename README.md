# trafik

trafik is a comprehensive project demonstrating how to efficiently manage and deploy multiple domain-based applications using Docker Compose and Traefik. This repository provides a well-structured and scalable solution for running various web applications, APIs, or services under different domain names, all within a single Docker environment.

## File & folder structure

```bash

app1
├── # ... other files
└── docker-compose.production.yml
app2
├── # ... other files
└── docker-compose.production.yml
trafik
├── Dockerfile
├── README.md
├── docker-compose.yml
└── traefik.yml

0 directories, 1 file

```

## Why You Need This
Do you have a Docker-enabled web server where you want to host multiple applications, each accessible under its own unique domain name (like app1.com and app2.com)? Look no further!

This repository provides a solution for running and managing such a multi-domain setup using Docker Compose and Traefik. It streamlines application deployment and ensures efficient traffic management across your domains.

## Want to have $200 on digital ocean ? Click the following DigitalOcean button to get your $200. 

[![DigitalOcean Referral Badge](https://web-platforms.sfo2.digitaloceanspaces.com/WWW/Badge%203.svg)](https://www.digitalocean.com/?refcode=fefa8cc1cbc0&utm_campaign=Referral_Invite&utm_medium=Referral_Program&utm_source=badge)


## Key Features:
- Docker Compose: Centralized configuration and orchestration of multiple Docker containers.
- Traefik: Reverse proxy and load balancer for handling HTTP traffic and routing requests based on domain names.
- Multiple Domain Support: Ability to manage and serve applications under different domain names seamlessly.
- Configuration Flexibility: Customizable Traefik configuration for advanced routing rules, SSL/TLS termination, and more.
- Scalability: Easily scale individual applications or the entire infrastructure as needed.
- Best Practices: Adheres to Docker and Traefik best practices for optimal performance and security.

## Example Usage:

- Clone the repository: `git clone https://github.com/adnankaya/trafik`
- Configure domain names and application settings in the docker-compose.yml file.
- Start the Docker Compose environment: `docker-compose up -d --build`
- Access your applications using their respective domain names.

### Additional Considerations:

- Consider using a DNS provider to map your domain names to the IP address of your Docker host or a load balancer.
- Explore advanced Traefik features like middleware, labels, and custom headers for fine-grained control over routing and request handling.
- Implement security measures such as SSL/TLS certificates, rate limiting, and access controls.