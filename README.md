# Example Next.js with GitHub Registry

## Usage

```
$ docker run docker.pkg.github.com/murajun1978/example-github-registry-next-docker/example-next:latest
```

## Development

Clone the repository:

```
$ git clone https://github.com/murajun1978/example-github-registry-next-docker.git
$ cd example-github-registry-next-docker
```

Run server container:

```
$ docker-compose up
```

Run development container:

```
$ docker-compose run --rm runner
```

## Docker build for Production

```
$ docker build -f docker/production/Dockerfile .
```
