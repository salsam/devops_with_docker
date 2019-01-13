# Commands

## Building

```bash
backend-example-docker $ docker build -t 1.6 .
```

## Running

```bash
$ docker run -d -v $(pwd)/logs.txt:/backend-example-docker/logs.txt --name=1.6 -p 8000:8000 1.6
```