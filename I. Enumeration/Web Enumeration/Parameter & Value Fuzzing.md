
| ***Command***                                                                                                                        | ***Usage***                                                                                  |
| ------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------- |
| `wenum -w <wordlist> --hc 404 -u <url/?param=FUZZ>`<br>                                                                              | **GET** Parameter Fuzzing using `wenum`                                                      |
| `ffuf -w <wordlist> -u 'http://<SERVER_IP>:<PORT>/<page>?FUZZ=value' -fs <most-common-size>`                                         | **GET** Parameter Fuzzing using most common parameter names. Filter out `<most-common-size>` |
| `ffuf -u <url> -X POST -H "Content-Type: application/x-www-form-urlencoded" -d "param=FUZZ" -w <wordlist> -mc 200 -v`                | **POST** Value fuzzing - Post request.                                                       |
| ***Wordlists to Use***:                                                                                                              |                                                                                              |
| `/opt/useful/seclists/Discovery/Web-Content/burp-parameter-names.txt`                                                                |                                                                                              |
| `LFI-Jhaddix.txt`                                                                                                                    | LFI path traversal                                                                           |
| `Discovery/Web-Content/default-web-root-directory-linux.txt`<br>OR<br>`Discovery/Web-Content/default-web-root-directory-windows.txt` | LFI web root Fuzzing                                                                         |
| `seq 1 1000 > ids.txt`                                                                                                               | Generating a wordlist for sequential fuzzing                                                 |



