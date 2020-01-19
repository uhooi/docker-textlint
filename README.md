# docker-textlint

[![](http://dockeri.co/image/uhooi/textlint)](https://hub.docker.com/r/uhooi/textlint)  
[![](https://github.com/uhooi/docker-textlint/workflows/CD/badge.svg)](https://github.com/uhooi/docker-textlint/actions?query=workflow%3ACD)

Docker image for textlint.

## Usage

### Shell

##### Pull the Docker image from Docker Hub:

```bash
$ docker pull uhooi/textlint:latest
```

##### Create a container from the image and run it:

```bash
# Output textlint version
$ docker run --rm uhooi/textlint --version
v11.6.1

# Run textlint example
$ docker run --rm -v $PWD:/work uhooi/textlint --plugin review --preset preset-ja-technical-writing --fix --config .textlintrc foo.re
```

### GitHub Actions

TBD
