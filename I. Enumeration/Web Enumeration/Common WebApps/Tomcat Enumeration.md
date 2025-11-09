# Cheatsheet


| ***Command***                                          | ***Usage***             |
| ------------------------------------------------------ | ----------------------- |
| `curl -s http://<tomcat-root>/docs/ \| grep Tomcat `   | Finding Tomcat Version. |
| Look for the `/manager` and `/host-manager` endpoints. |                         |

# Related Pages

[Tomcat Exploitation](III.%20Exploitation/Web%20Exploitation/Common%20WebApp%20Exploitation/Tomcat%20Exploitation.md): Includes brute force and RCE techniques.
# Overview

[Apache Tomcat](https://tomcat.apache.org) is an open-source web server that hosts applications written in Java.


 `Web.xml` is **Very** important to check in case of potential *LFI*.
### General Tomcat Folder Structure

```shell
├── bin
├── conf
│   ├── catalina.policy
│   ├── catalina.properties
│   ├── context.xml
│   ├── tomcat-users.xml
│   ├── tomcat-users.xsd
│   └── web.xml
├── lib
├── logs
├── temp
├── webappsdroopescan scan dr
│   ├── manager
│   │   ├── images
│   │   ├── META-INF
│   │   └── WEB-INF
|   |       └── web.xml
│   └── ROOT
│       └── WEB-INF
└── work
    └── Catalina
        └── localhost
```

`tomcat-users.xml`: stores users credentials + assigned roles.

### Webroot Location

The default Tomcat root directory can vary:

- **Linux/macOS:** `/usr/local/tomcat` or `/opt/tomcat`
- **Windows:** `C:\Program Files\Apache Software Foundation\Tomcat x.x`