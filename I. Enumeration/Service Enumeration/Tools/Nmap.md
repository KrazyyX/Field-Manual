
| ***Command***                                                                                                                  | ***Usage***                       |
| ------------------------------------------------------------------------------------------------------------------------------ | --------------------------------- |
| `sudo nmap <IP>/<SUBNET> -sn`                                                                                                  | Host discovery using ping scan.   |
| `nmap -sV -top-port 100 -sU <ip>`                                                                                              | UDP Scan for the top 100 ports    |
| `nmap -sV -sC -vvv 10.10.10.68 -Pn -oN scan.txt`<br>ADD `-p-` to cover all ports.                                              | Useful all in 1 scan.             |
| `nmap --source-port 53 ...`                                                                                                    | Scanning through a filtered port. |
| `for PORT in {0..1000}; do timeout 1 bash -c "</dev/tcp/<IP>/$PORT&>/dev/null" 2>/dev/null && echo "port $PORT is open"; done` | Manual port scan                  |
