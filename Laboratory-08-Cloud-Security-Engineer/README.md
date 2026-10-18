
# Mission 8: The Cloud Security Engineer

## Mission Overview

This mission focuses on securing a Linux server by deploying an Nginx container and configuring the UFW host-based firewall. The firewall is configured to block incoming traffic by default while allowing the required SSH and web application ports.

## Objectives

- Explain the Principle of Least Privilege, Attack Surface, and Default Deny Policy.
- Deploy and test an Nginx Docker container.
- Configure UFW with a default deny incoming policy.
- Allow SSH and TCP port 8080.
- Document the firewall configuration and provide screenshots.

## Commands Executed

```bash
docker run -d --name secure-web-app -p 8080:80 nginx
curl -s http://localhost:8080 | head -n 5
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
sudo ufw allow 8080/tcp
sudo ufw status numbered
```

## Skills Learned

- Understanding basic cloud security principles.
- Deploying and testing a Docker container.
- Configuring a host-based firewall.
- Managing network access with UFW.
- Documenting technical work in Markdown.
