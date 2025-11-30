---
title: "PostgreSQL: Linux downloads (Ubuntu)"
source: "https://www.postgresql.org/download/linux/ubuntu/"
author:
  - "[[The PostgreSQL Global Development Group]]"
published:
created: 2025-11-19
description:
tags:
  - "clippings"
---
## Linux downloads (Ubuntu)

PostgreSQL is available in all Ubuntu versions by default. However, Ubuntu "snapshots" a specific version of PostgreSQL that is then supported throughout the lifetime of that Ubuntu version. The PostgreSQL project maintains an [Apt repository](https://www.postgresql.org/download/linux/ubuntu/#apt) with all supported of PostgreSQL available.

## Included in Distribution

Ubuntu includes PostgreSQL by default. To install PostgreSQL on Ubuntu, use the `apt` (or other apt-driving) command:

```
apt install postgresql
```

## PostgreSQL Apt Repository

If the version included in your version of Ubuntu is not the one you want, you can use the [PostgreSQL Apt Repository](https://apt.postgresql.org/). This repository will integrate with your normal systems and patch management, and provide automatic updates for all supported versions of PostgreSQL throughout the support [lifetime](https://www.postgresql.org/support/versioning/) of PostgreSQL.

The PostgreSQL Apt repository supports the current versions of Ubuntu:

- questing (25.10, non-LTS)
- plucky (25.04, non-LTS)
- noble (24.04, LTS)
- jammy (22.04, LTS)

on the following architectures:

- amd64
- arm64 (LTS releases only)
- ppc64el (LTS releases only)

Automated repository configuration:

To manually configure the Apt repository, follow these steps:

Install PostgreSQL: (replace "18" by the version you want)

```
sudo apt install postgresql-18
```

For more information about the apt repository, including answers to frequent questions, please see the [PostgreSQL Apt Repository wiki page](https://wiki.postgresql.org/wiki/Apt).

## Packages

The repository contains many different packages including third party addons. The most common and important packages are (substitute the version number as required):

| postgresql-client-18 | client libraries and client binaries |
| --- | --- |
| postgresql-18 | core database server |
| postgresql-doc-18 | documentation |
| libpq-dev | libraries and headers for C language frontend development |
| postgresql-server-dev-18 | libraries and headers for C language backend development |