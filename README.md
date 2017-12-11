# Dnsmasq Docker images

> [Dnsmasq official documents](http://www.thekelleys.org.uk/dnsmasq/doc.html)

Tag | Dockerfile | Image Layers
----|------------|-------------
`2.76` | [Dockerfile](https://github.com/helphi/Dockerfile-dnsmasq/blob/master/2.76/Dockerfile) | [![](https://images.microbadger.com/badges/image/helphi/dnsmasq:2.76.svg)](https://microbadger.com/images/helphi/dnsmasq:2.76 "Get your own image badge on microbadger.com")

# How to use

```sh
docker run -d --name=dnsmasq \
  -p 53:53 \
  -p 53:53/udp \
  -p 67:67/udp \
  -p 68:68/udp \
  -v /etc/dnsmasq.d:/etc/dnsmasq.d \
  helphi/dnsmasq:2.76
```