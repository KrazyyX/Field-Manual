# Cheatsheet


| ***Command***                                                                                                                                                                                                | ***Usage***                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------- |
| `ffuf -w <wordlist> -u <url/FUZZ>`                                                                                                                                                                           | Basic Fuzz                                     |
| `ffuf -w <wordlist> -u <url/FUZZ> -e .php,.html,.txt,.bak,.js`                                                                                                                                               | Fuzzing w/ Extensions                          |
| `ffuf -w <wordlists> -u <url> -ic -e <extensions> -recursion`                                                                                                                                                | Recursive Fuzzing. Specify `-recursion-depth`. |
| `python3 ~/webfuzz_api/api_fuzzer.py http://IP:PORT`                                                                                                                                                         | Fuzzes API endpoints.                          |
| ***Common Wordlists***                                                                                                                                                                                       |                                                |
| 1. `Discovery/Web-Content/common.txt`<br><br>2. `Discovery/Web-Content/directory-list-2.3-medium.txt`<br><br>3. `Discovery/Web-Content/raft-large-directories.txt`<br><br>4. `Discovery/Web-Content/big.txt` |                                                |
