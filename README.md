<!--
 ___ _            _ _    _ _    __
/ __(_)_ __  _ __| (_)__(_) |_ /_/
\__ \ | '  \| '_ \ | / _| |  _/ -_)
|___/_|_|_|_| .__/_|_\__|_|\__\___|
            |_| 
-->
![](https://docs.simplicite.io//logos/logo250.png)
* * *

`SimSecure` module definition
=============================

Secure parameters for Simplicité
====================

This modules does the following changes to system parameters for improved security:
- improve passwords: MD5 -> salted SHA-512
- improve default HTTP headers
- imposes a max upload size on files
- deactivates user impersonation feature
- closes optional endpoints:
  - /api (and tester)
  - /io (and tester)
  - /git
  - /maven
  - /health

The change in hashing algorithm will render all current passwords unusable. After importing and **before** clearing the cache, you should import the associated dataset to update designer's password to `Ch4ngePassw0rd!`

**NB: Correct system parameters configuration is one of the aspects of Simplicité's security, the other aspects are just as important, please check the [security documentation](https://docs.simplicite.io/documentation/security.md).**

