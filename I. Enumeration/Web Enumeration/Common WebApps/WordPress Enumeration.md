
| ***Command***                                                                         | ***Usage***                                                                                                    |
| ------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| `sudo wpscan --url <url> --enumerate --api-token <API-token>`                         | Uses the `WPScan` tool to perform automated scanning.                                                          |
| `curl -s http://<url> \| grep WordPress`                                              | Finds the WordPress version.                                                                                   |
| `curl -s http://<url>/ \| grep plugins`<br><br>`curl -s http://<url>/ \| grep themes` | Identify the Wordpress themes and plugins installed.<br><br>**NOTE**: plugins usually have *readme.txt* files. |
| Manually visit: `/wp-content/plugins/` & `/wp-content/themes/` in case of no hits.    |                                                                                                                |

# Overview

Wordpress is a popular CMS.
## User roles
1. Administrator: This user has access to administrative features within the website. This includes adding and deleting users and posts, as well as editing source code.
2. Editor: An editor can publish and manage posts, including the posts of other users.
3. Author: They can publish and manage their own posts.
4. Contributor: These users can write and manage their own posts but cannot publish them.
5. Subscriber: These are standard users who can browse posts and edit their profiles.

# Methodology

1. Enumerate the WordPress Version
2. Enumerate plugins and themes installed. Note down version numbers.
3. Run `wpscan` to identify if directories have listing enabled.
4. Run `wpscan` to identify users.
5. Verify if any vulnerabilities exist with WordPress version OR Plugin version.

