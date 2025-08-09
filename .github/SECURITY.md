# Security Policy

⚠ **PLEASE DO NOT DISCLOSE SECURITY-RELATED ISSUES PUBLICLY**



## Supported Versions

| Version | Supported |
| ------- | --------- |
| 0.29.x  | ✅ Yes    |
| < 0.29  | ❌ No     |

**Current Release:** **v0.29.3**


## Reporting Security Issues

Do **not** create public GitHub issues for security vulnerabilities.

Instead, please email us privately: **[security@wdevcli.com](mailto:security@wdevcli.com)**

### Include in Your Report

* WDev version number
* Operating system (and Docker version if relevant)
* Steps to reproduce the issue
* Description of potential impact

If the report contains sensitive proof-of-concept code, request our **PGP key** in your first email.

---

## Our Response

* We’ll acknowledge receipt as soon as possible.
* We may request additional details, logs, or reproduction steps.

---

## Security Notes

WDev is a **local development tool** designed for **trusted environments** only:

* **Not** intended for production use
* Relies on Docker container isolation
* SSL certificates are development-only

---

## Important Security Areas

Please report issues involving:

* Remote code execution
* Container escape or Docker security flaws
* SSL / certificate handling problems
* Vulnerabilities in the WDev Agent plugin
* Unauthorized file system access

---

## Low-Priority / Won’t-Fix Examples

* Issues requiring **physical access** to your development machine
* Purely theoretical attacks with **no practical exploit path**

---

## Contact

* **Security issues:** [security@wdevcli.com](mailto:security@wdevcli.com)
* **General questions:** [GitHub Issues](https://github.com/devuri/wdev-community/issues)
* **Website:** [wdevcli.com](https://wdevcli.com)

---

**Last Updated:** August 2025
