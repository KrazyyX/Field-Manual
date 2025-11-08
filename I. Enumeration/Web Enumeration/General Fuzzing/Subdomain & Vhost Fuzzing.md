
| ***Command***                                                       | ***Usage***                    |
| ------------------------------------------------------------------- | ------------------------------ |
| `gobuster vhost -u <url> -w <wordlist> --append-domain`             | Vhost Fuzzing using `gobuster` |
| `gobuster dns -d <domain-name> -w`                                  | Subdomain Fuzzing              |
| ***Wordlists to use***                                              |                                |
| `/usr/share/seclists/Discovery/DNS/subdomains-top1million-5000.txt` |                                |
| `/usr/share/seclists/Discovery/DNS/namelist.txt`                    |                                |
