# Marine

Contents writer application for [track](https://tracks.run/)

You can make all of following contents with it.

- Challenge
- Quiz
- Book

## Prerequisite

- docker
- docker-compose

## Start

```
docker-compose up -d
```

After the application started, you can access the app via `http://localhost:39000`

## Stop

```
docker-compose down
```

## How to use
Following directory names are listed in dropdown on header.

- under the `contents` directory
- which has `book.yml` file

Choose 1 of them.

## How to update application
Using docker image is published in [DockerHub](https://hub.docker.com/r/givery/marine/)

What you have to do is only pull latest version.

```
# Publishing version for the real customer
docker pull givery/marine:latest

# Internal beta version for the development/testing
docker pull givery/marine:internal
```

## About contents directory
This directory is shared with docker container.
Marine will sarech contents from this directory.

Checkout your content repository in this directory.
