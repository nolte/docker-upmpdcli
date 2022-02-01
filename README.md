# upmpdcli as container

[![Docker Image CI](https://github.com/nolte/docker-upmpdcli/actions/workflows/release-build-push-container.yaml/badge.svg)](https://github.com/nolte/docker-upmpdcli/actions/workflows/release-build-push-container.yaml) [![Docker Pulls](https://img.shields.io/docker/pulls/nolte/upmpdcli.svg)](https://hub.docker.com/r/nolte/upmpdcli/)

----

Run [upmpdcli](http://www.lesbonscomptes.com/upmpdcli/) as docker container, used as [Mopdiy UPnP client](https://docs.mopidy.com/en/latest/clients/upnp/).   
This Containers allows Applications like [BubbleUPnP](https://play.google.com/store/apps/details?id=com.bubblesoft.android.bubbleupnp) connect to your [mopidy](https://docs.mopidy.com/en/latest/clients/upnp/) instance.

*start*

```
docker run --network="host" nolte/upmpdcli -h [mpdhost] -p 6600 -f [UpnpFrindly Name]
```

## Build

```bash
docker buildx build \
    --platform \
        linux/amd64,linux/arm/v7 \
    -t nolte/upmpdcli:dirty -f Dockerfile .
```
