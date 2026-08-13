# Week 2 — Linux Administration

## Topics Covered

- Users and groups
- File ownership
- File permissions
- chmod
- chown
- Processes
- Process IDs (PIDs)
- systemd
- systemctl
- journalctl
- Basic network troubleshooting

## File Permissions

Linux permissions are divided into:

- User/Owner (`u`)
- Group (`g`)
- Others (`o`)

Common permissions:

- Read (`r`)
- Write (`w`)
- Execute (`x`)

### Numeric Permissions


4 = read
2 = write
1 = execute

Examples:

644 = rw-r--r--
755 = rwxr-xr-x

**Symbolic Permissions**
chmod u+x file
chmod g+w file
chmod o-r file
chmod go-x file

**Ownership**
chown user:group file

Example:
chown alex:developers project.txt

**Processes**

A process is an instance of a program currently running.

Useful commands:

ps aux

**Services**
systemctl status nginx
systemctl start nginx
Logs
journalctl
journalctl -u nginx

**Networking**
ss -tulpn
ping <IP-address>
ss -tulpn
ping <IP-address>
