# Day 3 - Linux Deep Dive

## Section 1: System Monitoring
- top = live process monitor
- htop = better version of top
- free -h = check RAM usage
- df -h = check disk space
- uname -a = system information
- uptime = how long server running

## Section 2: Log Management

- tail -n 50 /var/log/syslog  =  last 50 lines
- tail -f /var/log/syslog  =  watch live logs
- grep -i "error" /var/log/syslog  =  search logs
- sudo docker logs CONTAINER_ID  -  docker logs
- sudo docker logs -f ID  =  live docker logs

## Section 3: Network Commands

- ping -c 4 google.com  =  test connectivity
- ip a  =  check IP address
- ss -tuln  =  check open ports
- curl http://localhost  =  check open ports
- wget URL  =  download files
- nslookup google.com  =  DNS lookup
- traceroute google.com  =  trace netwrok path

## Section 4: Process Management

- ps aux  =  see all processes
- pas aux | grep name  =  find specific process
- kil PID  =  stop process
- kill -9 PID  =  force kill
- killall name  =  kill by name
- sleep 100 &  =  run in background
- jobs  =  see background jobs
- kill %1  =  kill job number 1
- nohup  =  keep running after logout

## systemctl Commnads

- sudo systemctl status nginx  =  check status
- sudo systemctl start nginx  =  start service
- sudo systemctl stop nginx  = stop service
- sudo systemctl restart nginx  =  restart service
- sudo systemctl enable nginx  =  enable on boot

## Errors I Faced

- kill PID  =  wrong! PID is not literal work
- kill 4521  =  correct! use actual number

## Real World Usage

- ps aux | grep myapp  =  find problematic process
- kill -9 PID  =  kill it
- tail -f /var/log/app  =  watch logs live
- curl localhost:8080  = test if site is up
