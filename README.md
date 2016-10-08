# docker-torproxy
The torproxy container helps route traffic through the Tor network through use of a local socks proxy. Applications can be configured to forward traffic through Tor by configuring them to use a socks proxy which listens on your docker host on TCP port 9050.

Please use caution and follow Tor's guidelines when sending traffic through the proxy.
https://trac.torproject.org/projects/tor/wiki/doc/TorifyHOWTO

# Running
```
docker-compose up -d
```

# Connecting to the Tor Proxy
Configure your application to connect via a SOCKS proxy to the host running
your docker containers. The Tor SOCKS proxy is listening on TCP port 9050.

 _Please read the Tor documentation to understand how proxing works in this
 manner as it can be less secure._
