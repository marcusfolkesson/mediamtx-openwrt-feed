# MediaMTX OpenWRT feed

## Description


  MediaMTX (formerly rtsp-simple-server) is a ready-to-use and
  zero-dependency real-time media server and media proxy that allows to
  publish, read, proxy, record and playback video and audio streams.

- [Website](https://github.com/bluenviron/mediamtx)

## Usage

This repository is intended to be layered on-top of an OpenWrt buildroot. If you do not have an OpenWrt buildroot installed, see the documentation at: [OpenWrt Buildroot – Installation](https://openwrt.org/docs/guide-developer/build-system/install-buildsystem) on the OpenWrt support site.

To install this feed and all its package definitions, run the following in your OpenWRT root-folder:
```
echo "src-git opencv https://github.com/marcusfolkesson/mediamtx-openwrt-feed.git" >> ./feeds.conf
echo "src-git opencv https://github.com/marcusfolkesson/libcamera-openwrt-feed.git" >> ./feeds.conf
./scripts/feeds update -a
./scripts/feeds install -a 
```

# Information

This feed is intended to be used with with the rpicamera tag, so the configuration is hard-coded into the package. 

Please feel free to modify and/or make it configurable. If you do, please consider to create a pull request.

# Patches

Please submit any patches against the mediamtx-openwrt-feed repository via pull request.


