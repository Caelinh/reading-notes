# HTTP Request and response cycle

## Steps of an htttp request

1. The browser breaks apart the web address into its respective queries and properties.
2. Once it has the hostname it resolves the ip address and checks for any recently used urls or dns servers in the local cache.
3. If nothing is found in the cache a dns request is sentusing udp. 
4. Once a dns address is found a TCP request is sent. Which is the  transport layer protocol.
5. After connecting to the TCP the HTTP request is sent at last. And a response can be received.
6. when disconnecting the client and server send a 4 way handshake fin ack fin ack.

### Reading material

[Review: High-level HTTP](https://dev.to/dangolant/things-i-brushed-up-on-this-week-the-http-request-lifecycle-)

[Java HTTP Request example](https://www.baeldung.com/java-http-request)
