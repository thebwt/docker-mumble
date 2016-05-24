# Mumble and Mumble-Django with Docker

## Introduction

This guide is going to explain how to create and (hopefully) maintain a mumble server running on Docker, along with a web admin interface.

Components in play:

* [Docker](https://docker.io)
* [Docker-Compose](https://docs.docker.com/compose/)
* [Mumble-Server (Murmurd)](http://mumble.info)
* [Django](https://www.djangoproject.com/)
* [Django-Mumble](https://bitbucket.org/Svedrin/mumble-django/wiki/Home)

## Getting the repo

Go ahead and clone my repo at <https://github.com/thebwt/docker-mumble>

* `git clone git@github.com:thebwt/docker-mumble.git`
* You can see the dockerfiles I've written and confirm it's all on the level ;)

There are three images we'll be using:

1. **mumble-volume** - A volume container just there to hold our ini and sqlite file.
2. **mumble-head** - The actual mumble endpoint, this hardly ever changes.
3. **mumble-web** - The Mumble-Django endpoint, we'll need to bootstrap this manually.

Finally, there is a *docker-compose.yml* that should be doing the heavy lifting for us.

## Fire it up

Alright, let's put that docker-compose.yml to work.

* `cd docker-mumble`
* `docker-compose up -d`

[1]: http://docker.io
[2]: http://mumble.info
[3]: https://bitbucket.org/Svedrin/mumble-django/wiki/Home
[4]: https://www.djangoproject.com/
