# Docker

## Table of Contents

- What is Docker?
- First Run with Docker
- Docker vs Virtual Machine
- Main Docker Commands
- Debug a Container
- Docker Compose
- Docker Volumes

## What is Docker?

What does an application need?
- Configuration
- Dependencies/Libraries
- Binaries

Container is a way to package(image) an application with its necessary *configuration*, *binaries* and *dependencies*.

That package(image) is:
- portable
- easily shared
- easy to transfer

Where do these packages live?
- Repositories
	- Public
	- Private

Before the container technology?
- The deployment has many steps and time wasting. Especially in a scalable environment. You would need to redo every step for each deployment.
- Installation process different for each OS.
- Many steps where something could go wrong.
- Each container has a single application and is isolated from both other containers and host machine.