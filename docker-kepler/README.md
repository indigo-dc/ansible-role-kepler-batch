# docker-kepler
Docker image for the kepler scientific workflow engine

## Build

TO BE UPDATED

```
docker build -t docker-kepler .
```

## Run the image


```
docker run -p 2020:22 -p 5900:5900 -d docker-kepler
```

Access through ssh
```
ssh -p 2020 ubuntu@localhost
```

Run kepler
```
kepler.sh
```

## Aknowlegments

https://kepler-project.org/
