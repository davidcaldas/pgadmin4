# Brothers in ARMs' PGAdmin4 docker image![GitHub release (latest by date)](https://img.shields.io/github/v/release/biarms/pgadmin4?label=Latest%20Github%20release&logo=Github)![GitHub release (latest SemVer including pre-releases)](https://img.shields.io/github/v/release/biarms/pgadmin4?include_prereleases&label=Highest%20GitHub%20release&logo=Github&sort=semver)[![TravisCI build status image](https://img.shields.io/travis/biarms/pgadmin4/master?label=Travis%20build&logo=Travis)](https://travis-ci.org/biarms/pgadmin4)[![CircleCI build status image](https://img.shields.io/circleci/build/gh/biarms/pgadmin4/master?label=CircleCI%20build&logo=CircleCI)](https://circleci.com/gh/biarms/pgadmin4)[![Docker Pulls image](https://img.shields.io/docker/pulls/biarms/pgadmin4?logo=Docker)](https://hub.docker.com/r/biarms/pgadmin4)[![Docker Stars image](https://img.shields.io/docker/stars/biarms/pgadmin4?logo=Docker)](https://hub.docker.com/r/biarms/pgadmin4)[![Highest Docker release](https://img.shields.io/docker/v/biarms/pgadmin4?label=docker%20release&logo=Docker&sort=semver)](https://hub.docker.com/r/biarms/pgadmin4)<!--[![build status](https://api.travis-ci.org/biarms/pgadmin4.svg?branch=master)](https://travis-ci.org/biarms/pgadmin4)-->## Overview[PGAdmin](https://pgadmin.org) is an web-based UI administration plateform for PostgreSQL open source database.This git repo build a docker image for running [PGAdmin](https://pgadmin.org) on an arm(hf) based system.Once done, the result will be pushed on [dockerhub](https://hub.docker.com/r/biarms/pgadmin4/).Inspired from [thaJeztah pgadmin4 image](https://github.com/thaJeztah/pgadmin4-docker).Currently tested on a Odroid XU4 and Raspberry Pi 3 running respectively Ubuntu and Raspbian stretch.## UsageSince 4.22: see https://www.pgadmin.org/docs/pgadmin4/latest/container_deployment.html.Before 4.22: see [thaJeztah's pgadmin4 image](https://github.com/thaJeztah/pgadmin4-docker).## How to build locally1. Option 1: with CircleCI Local CLI:   - Install [CircleCI Local CLI](https://circleci.com/docs/2.0/local-cli/)   - Call `circleci local execute`2. Option 2: with make:   - Install [GNU make](https://www.gnu.org/software/make/manual/make.html). Version 3.81 (which came out-of-the-box on MacOS) should be OK.   - Call `make build`## Releases### 4.22 !!! Caution - non-backward compatible changes !!! - Upgrade PGAdmin version from 4.21 to 4.22- Upgrade python from v2 to v3- Change Docker entrypoint to match 'official PGAdmin4 docker image' instead of 'thaJeztah' PGAdmin4 docker images.### 4.21- Upgrade PGAdmin version from 2.1 to 4.21- Upgrade Alpine from 3.6 to 3.11- Huge refactoring of the build (based on docker 19.03.8), including (Travis and) CircleCI integration- Improve the README.md documentation, including shields.io images