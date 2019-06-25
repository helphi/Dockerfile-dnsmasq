# Dnsmasq Docker images

## Tags

- `2.76`
- `2.80`

## Usage

```bash
echo "user=root" > /etc/dnsmasq.d/dnsmasq.conf

docker run -d --name=dnsmasq \
  -p 53:53 \
  -p 53:53/udp \
  -p 67:67/udp \
  -p 68:68/udp \
  -v /etc/dnsmasq.d:/etc/dnsmasq.d \
  helphi/dnsmasq:2.80
```

> [Dnsmasq official documents](http://www.thekelleys.org.uk/dnsmasq/doc.html)
