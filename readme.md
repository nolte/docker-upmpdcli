# upmpdcli as container

[![Build Status](https://travis-ci.org/nolte/docker-upmpdcli.svg?branch=master)](https://travis-ci.org/nolte/docker-upmpdcli)

Run [upmpdcli](http://www.lesbonscomptes.com/upmpdcli/) as docker container, used as [Mopdiy UPnP client](https://docs.mopidy.com/en/latest/clients/upnp/).   
This Containers allows Applications like [BubbleUPnP](https://play.google.com/store/apps/details?id=com.bubblesoft.android.bubbleupnp) connect to your [mopidy](https://docs.mopidy.com/en/latest/clients/upnp/) instance.

*start*

```
docker run --network="host" nolte/upmpdcli -h [mpdhost] -p 6600 -f [UpnpFrindly Name]
```


**amd64 Images**  
[![Docker Pulls](https://img.shields.io/docker/pulls/nolte/upmpdcli.svg)](https://hub.docker.com/r/nolte/upmpdcli/)
[![Docker Build Statu](https://img.shields.io/docker/build/nolte/upmpdcli.svg)](https://hub.docker.com/r/nolte/upmpdcli/)
[![](https://images.microbadger.com/badges/image/nolte/upmpdcli.svg)](https://microbadger.com/images/nolte/upmpdcli "Get your own image badge on microbadger.com")  [![](https://images.microbadger.com/badges/version/nolte/upmpdcli.svg)](https://microbadger.com/images/nolte/upmpdcli "Get your own version badge on microbadger.com")

*build*

```
 docker build -t nolte/upmpdcli:development -f Dockerfile .
```

**armhf Images**   
[![Docker Pulls](https://img.shields.io/docker/pulls/nolte/rpi-upmpdcli.svg)](https://hub.docker.com/r/nolte/rpi-upmpdcli/)
[![](https://images.microbadger.com/badges/image/nolte/rpi-upmpdcli.svg)](https://microbadger.com/images/nolte/rpi-upmpdcli "Get your own image badge on microbadger.com")  [![](https://images.microbadger.com/badges/version/nolte/rpi-upmpdcli.svg)](https://microbadger.com/images/nolte/rpi-upmpdcli "Get your own version badge on microbadger.com")

*build*

```
 docker build -t nolte/rpi-upmpdcli:development -f DockerfileRPI .
```
