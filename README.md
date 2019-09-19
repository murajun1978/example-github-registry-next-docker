# Example Next.js with GitHub Registry

## Usage

```
$ docker run --rm -p 3000:3000 docker.pkg.github.com/murajun1978/example-github-registry-next-docker/example-next:0.0.2
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

## Push to GitHub Registry

```
$ docker push docker.pkg.github.com/murajun1978/example-github-registry-next-docker/example-next:[:TAG]
```
