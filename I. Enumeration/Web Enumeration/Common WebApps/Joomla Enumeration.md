
| ***Command***                                                                                           | ***Usage***                                                                            |
| ------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| Check `robots.txt`                                                                                      | Joomla's robots.txt looks a certain way, so this would help identify if it was Joomla. |
| `curl -s http://dev.inlanefreight.local/administrator/manifests/files/joomla.xml \| xmllint --format -` | Fingerprint which Joomla version is being used.                                        |
| `droopescan scan joomla --url http://<url>`                                                             | Plugin-based scanner that works for Joomla and others.                                 |

# Related Pages

[Joomla Exploitation](III.%20Exploitation/Web%20Exploitation/Common%20WebApp%20Exploitation/Joomla%20Exploitation.md): Performing Password brute-forcing, RCE, and other exploits specific to the Joomla version.

# Overview

Joomla is a popular CMS.