# WDevCli

> Pronounce it "Dub-Dev"

WDevCli is a local development environment, workflow platform, and remote operations tool for WordPress, PHP, and Laravel. It runs as a single binary, stores everything as files on disk, and is designed to get out of your way.

```bash
wdev add myblog --wp        # new local WordPress site
wdev pull production.com    # clone a remote WordPress site locally
wdev host audit staging     # security triage of a remote Linux host
wdev remote push myblog     # deploy to a staging node
```

## Status

> WDevCli is **alpha software**.
> 
> It works and is used daily by the team building it. You will encounter rough edges. Interfaces change between releases, including breaking changes at the major and minor version level.

Feedback filed here directly shapes what gets fixed and prioritized.


## What WDevCli is

WDevCli is a command-line tool for developers who work across local development, server management, and deployment, often as the same person. It handles the full workflow: spinning up a local WordPress or Laravel environment, managing SSL certificates, backing up and restoring sites, cloning remote sites locally, auditing remote hosts for security issues, provisioning staging nodes, and deploying code over SSH.

Everything it knows about your environment lives as files on disk. There is no hidden database, no locked-in state, no daemon that has to be running for your data to be accessible. Move the binary and your files to a new machine and keep working.

It ships as a single binary with minimal dependencies. No virtual environment setup. No npm install. Run it.



## The approach

Most developer tools make themselves necessary by hiding things. WDevCli is built around the opposite principle:

**Your project should stay your project. The dev environment should help, not hijack.**

In practice this means:

- Every site lives as a directory on disk with inspectable configs, not inside a proprietary database
- Backups are plain archives. Certificates are plain files. Logs are plain text.
- Moving to a new machine is a file copy, not a migration
- Linux is the ground truth. macOS and Windows are supported, but the tool thinks in Linux terms.



## What it covers

**Local development**
Create and manage WordPress, Laravel, and generic PHP sites backed by Docker. Per-site SSL certificates, automatic `.test` domain routing via a built-in nginx proxy, Xdebug, multisite support, PHP version selection, database management, and live plugin and theme development via bind mounts.

**Backup, restore, and cloning**
Full site snapshots with optional encryption. Domain-ready backups with automatic URL rewriting so a backup can be deployed directly to a new domain. Clone sites locally from remote servers. Import from archives.

**Workspace and workflow tooling**
Blueprint system for reusable site templates. Workspace management for multi-client or multi-project organization. WordPress content scraper for migrating content via REST API. WP-CLI and Artisan integration.

**Remote host operations**
SSH-based host diagnostics, security triage (read-only, seven-phase, nothing written to the remote host), traffic analysis, file transfer, and full filesystem backup with optional database dumps. All artifacts stored locally as inspectable files.

**Remote staging and deployment**
Bootstrap an Ubuntu VPS as an isolated WDevCli staging node. Provision per-site environments with isolated PHP-FPM pools, MariaDB databases, Nginx vhosts, and Let's Encrypt certificates. Deploy via atomic releases over SSH. Grant SFTP collaborator access without enabling shell login.



## Who it is for

WDevCli is built for developers who span more than one role. If you are the person who writes the code and manages the servers, or who runs a small agency where those responsibilities overlap, this tool is designed for your actual workflow rather than for a cleanly separated developer persona.

It is also useful for solo developers who want a local WordPress or PHP environment that behaves like production, can be backed up reliably, and does not require a full DevOps setup to maintain.



## Getting started

WDevCli is a premium product. Download it from [wdevcli.com](https://wdevcli.com), then follow the setup guide in the documentation.

Full installation and setup documentation is at [docs.wdevcli.com](https://docs.wdevcli.com).


## This repository

This is the public community repository for WDevCli. The main development repository is private.

Use this repository to:

- **File bug reports** using the issue tracker
- **Request features** by opening an issue with the `feature request` label
- **Ask questions** by opening a discussion

When filing a bug report, include your operating system, WDevCli version (`wdev --version`), and the relevant command output or error message.



## Links

- **Website**: [wdevcli.com](https://wdevcli.com)
- **Documentation**: [docs.wdevcli.com](https://docs.wdevcli.com)
- **Issues**: [github.com/devuri/wdevcli/issues](https://github.com/devuri/wdevcli/issues)
