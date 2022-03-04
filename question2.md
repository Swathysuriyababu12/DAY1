 Write a blog on Difference between HTTP1.1 vs HTTP2

HTTP HYPER TEXT TRANSFER PROTOCOL
HTTP is a network delay protocol.

HTTP1(1991)
1.For every TCP connection there is only one request and one response.
2.STATUS CODE-16

HTTP 1.1(1997)
1.SLOWER
It loads a request for every TCP connection.Hence slower.
It supports connection reuse i.e. for every TCP connection there could be multiple requests and responses, and pipelining where the client can request several resources from the server at once. However, pipelining was hard to implement due to issues such as head-of-line blocking and was not a feasible solution.
2.STATUS CODE-24
3.HTTP/1.1 provides faster delivery of web pages and reduces web traffic as compared to HTTP/1.0. However, TCP starts slowly and with domain sharding (resources can be downloaded simultaneously by using multiple domains), connection reuse and pipelining, there is an increased risk of network congestion.


HTTP2()
1.FASTER
Uses multiplexing, where over a single TCP connection resources to be delivered are interleaved and arrive at the client almost at the same time. It is done using streams which can be prioritized, can have dependencies and individual flow control. It also provides a feature called server push that allows the server to send data that the client will need but has not yet requested.
2.STATUS CODE-24 SAME
3.HTTP/2 utilizes multiplexing and server push to effectively reduce the page load time by a greater margin along with being less sensitive to network delays


