FROM alpine:3.6

RUN apk --no-cache add dnsmasq=2.76-r4

VOLUME /etc/dnsmasq.d

EXPOSE 53 53/udp 67/udp 68/udp

CMD ["dnsmasq", "-k"]