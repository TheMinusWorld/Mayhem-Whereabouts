# Mayhem Wherabouts Platform

This directory contains tools and configuration relevant to the platform
Mayhem Whereabouts will run on.

## Overview

The Mayhem Whereabouts platform will be on production a VM in the cloud and
for local development a docker container configured with ansible. They should
be based on the same linux distribution to mimic the production environment
for local development.

## Deploying on local

Following these instructions should get a local deployment of Mayhem
Whereabouts up and running .

If there are any issues, please report them on our [issue
tracker](https://github.com/TheMinusWorld/Mayhem-Whereabouts/issues) or check
if an issue is a known issue.

### Prerequesites

- [Docker](https://docs.docker.com/install/) (or a compatible tool such as
  [Podman](https://podman.io/getting-started/)) is required for setting this
  up.
- A [POSIX](https://en.wikipedia.org/wiki/POSIX)-compatible environment with
  standard tools such as `make` and `sh`. A native Windows environment is not
  supported at this time (but will be)- feel free to use cygwin or Windows
  Subsystem for Linux until that's sorted out.

## Deploying

Build an image with:

```sh
make build
```
