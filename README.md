# browsersync
[![Build Status](https://img.shields.io/travis/demyxco/browsersync?style=flat)](https://travis-ci.org/demyxco/browsersync)
[![Docker Pulls](https://img.shields.io/docker/pulls/demyx/browsersync?style=flat&color=blue)](https://hub.docker.com/r/demyx/browsersync)
[![Docker Layers](https://img.shields.io/microbadger/layers/demyx/browsersync?style=flat&color=blue)](https://hub.docker.com/r/demyx/browsersync)
[![Docker Image Size](https://img.shields.io/microbadger/image-size/demyx/browsersync?style=flat&color=blue)](https://hub.docker.com/r/demyx/browsersync)
[![Architecture](https://img.shields.io/badge/linux-amd64-important?style=flat&color=blue)](https://hub.docker.com/r/demyx/browsersync)
[![Alpine](https://img.shields.io/badge/alpine-latest-informational?style=flat&color=blue)](https://hub.docker.com/r/demyx/browsersync)
[![Node](https://img.shields.io/badge/node-latest-informational?style=flat&color=blue)](https://hub.docker.com/r/demyx/browsersync)
[![BrowserSync](https://img.shields.io/badge/browsersync-latest-informational?style=flat&color=blue)](https://hub.docker.com/r/demyx/browsersync)

With each web page, device and browser, testing time grows exponentially. From live reloads to URL pushing, form replication to click mirroring, Browsersync cuts out repetitive manual tasks. It’s like an extra pair of hands. Customise an array of sync settings from the UI or command line to create a personalised test environment. Need more control? Browsersync is easily integrated with your web platform, build tools, and other Node.js projects. https://www.browsersync.io/

TITLE | DESCRIPTION
--- | ---
ENTRYPOINT | dumb-init browsersync
WORKDIR | /var/www/html
PORT | 3000

# Updates
[![Code Size](https://img.shields.io/github/languages/code-size/demyxco/browsersync?style=flat&color=blue)](https://github.com/demyxco/browsersync)
[![Repository Size](https://img.shields.io/github/repo-size/demyxco/browsersync?style=flat&color=blue)](https://github.com/demyxco/browsersync)
[![Watches](https://img.shields.io/github/watchers/demyxco/browsersync?style=flat&color=blue)](https://github.com/demyxco/browsersync)
[![Stars](https://img.shields.io/github/stars/demyxco/browsersync?style=flat&color=blue)](https://github.com/demyxco/browsersync)
[![Forks](https://img.shields.io/github/forks/demyxco/browsersync?style=flat&color=blue)](https://github.com/demyxco/browsersync)

* Auto built weekly on Sundays (America/Los_Angeles)
* Rolling release updates

# Usage
```
docker run -dt --rm \
--name browsersync \
--net demyx \
--volumes-from example_container \
-p 3000:3000 \
-p 3001:3001 \
demyx/browsersync start --proxy example_container --files "/var/www/html/**/*" --host domain.tld --port 3000 --ui-port 3001
```