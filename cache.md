##Reference
```docker run --name lancache -p 192.168.1.150:80:80 steamcache/generic:latest```

```docker run --name steamcache-dns -p 192.168.1.150:53:53/udp -e STEAMCACHE_IP=192.168.1.150 -e USE_GENERIC_CACHE=true -e LANCACHE_IP=192.168.1.150 steamcache/steamcache-dns:latest```