
# Firewall Configuration

## 1. Allow SSH

```bash
sudo ufw allow ssh
```

This rule allows SSH connections needed for remote administration.

## 2. Set Default Policies

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

These commands block incoming connections by default while allowing outgoing traffic.

## 3. Enable UFW

```bash
sudo ufw enable
sudo ufw status verbose
```

These commands activate the firewall and display its status and default policies.

## 4. Allow Port 8080

```bash
sudo ufw allow 8080/tcp
sudo ufw status numbered
```

This rule permits incoming TCP traffic on port 8080 for the web application.

## 5. Why SSH Must Be Allowed First

If UFW is enabled before allowing SSH, remote administrators may lose their SSH connection and be locked out of the server.
