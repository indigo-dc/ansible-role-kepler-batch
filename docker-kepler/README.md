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
docker run -p 5900:5900 -it kepler
```

Access through VNC
```
vncviewer localhost:15900
```

## Aknowlegments

https://kepler-project.org/
