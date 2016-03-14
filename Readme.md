# Docker orchestration for EEA Jenkins Workers (Docker-in-Docker)

Docker orchestration for EEA Jenkins workers able to run Docker related jobs

## Changes

 - [CHANGELOG.md](https://github.com/eea/eea.docker.jenkins.dind/blob/master/CHANGELOG.md)


## Installation

1. Install [Docker](https://www.docker.com/).

2. Install [Docker Compose](https://docs.docker.com/compose/).


## Usage

    $ git clone https://github.com/eea/eea.docker.jenkins.dind.git
    $ cd eea.docker.jenkins.dind

Add master, user and password to connect jenkins slaves to jenkins master

    $ cp .secret.example .secret
    $ vi .secret

Start

    $ sudo docker-compose up -d

Check that everything started as expected and the slave successfully connected to master

    $ sudo docker-compose logs


## Upgrade

    $ sudo docker-compose pull
    $ sudo docker-compose up -d


## Copyright and license

The Initial Owner of the Original Code is European Environment Agency (EEA).
All Rights Reserved.

The Original Code is free software;
you can redistribute it and/or modify it under the terms of the GNU
General Public License as published by the Free Software Foundation;
either version 2 of the License, or (at your option) any later
version.


## Funding

[European Environment Agency (EU)](http://eea.europa.eu)
