# Day 5 - Linux Deep Dive

## Section 1: System Monitoring
- top, htop = live process viewer
- free -h = RAM usage
- df -h = disk space
- uname -a = system info
- uptime = how long server running

## Section 2: Log Management
- tail -f /var/log/syslog = live logs
- grep "error" file.log = filter logs
- docker logs container = container logs

## Section 3: Network Commands
- ping google.com = test connectons
- ip a = Show IP address
- ss -tuln = open ports
- curl url = fetch webpage
- nslook domain = DNS lookup

## Section 4: Process Management
- ps aux = all running processes
- kill PID = stop a process
- systemctl status = service status

## Section 5: File Permissions
- chmod 755 file = set permissions
- chown user file = change owner
- chmod +x script = make executable

## Section 6: Disk Management

- df -h = overall disk space
- du -sh /* = size of each folder
- find / -size +100M = find large files
- docker system df = dokcer disk usage
- docker system prune = clean dokcer junk
- sudo apt clean && autoremove = clean apt cache
- journalctl --vacuum-size=100M = trim logs

## Rule: Disk Use% over 85% = danger zone
