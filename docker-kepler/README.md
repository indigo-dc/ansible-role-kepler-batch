[![License](http://img.shields.io/:license-apache-blue.svg?style=flat-square)](http://www.apache.org/licenses/LICENSE-2.0.html)
[![](https://images.microbadger.com/badges/image/indigodatacloudapps/kepler.svg)](http://microbadger.com/images/indigodatacloudapps/kepler "Get your own image badge on microbadger.com")

# docker-kepler
Docker image for the kepler scientific workflow engine

## Build

```
docker build --rm -t kepler .
```

## Run the image


```
docker run -p 2020:22 -p 5900:5900 -d kepler
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
