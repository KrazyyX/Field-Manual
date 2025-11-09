# Cheatsheet

| ***Command***                                                                | ***Usage***                     |
| ---------------------------------------------------------------------------- | ------------------------------- |
| ![img](https://academy.hackthebox.com/storage/modules/113/jenkins_login.png) | Easily Recognizable login page. |
|                                                                              |                                 |
# Related Pages
[Jenkins Exploitation](III.%20Exploitation/Web%20Exploitation/Common%20WebApp%20Exploitation/Jenkins%20Exploitation.md): Performing RCE and reverse shells.
# Overview

[Jenkins](https://www.jenkins.io/) is an open-source automation server written in Java that helps developers build and test their software projects continuously.

Jenkins runs on Tomcat port 8080 by default.
- also utilizes port 5000 to attach slave servers.

Jenkins supports the following authentication methods:
- A local database.
- LDAP
- Unix user database.
- Delegate security to a servlet container.
- No authentication at all.