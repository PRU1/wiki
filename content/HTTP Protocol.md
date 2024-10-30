- learning about this to understand [[Python Web Scraping]] a bit better
- protocol: rules that tell you how data is exchange between computers
- HTTP: hypertext transfer protocol
- client-server protocol which means that recipients start a request in their web browser.
- you fetch sub-documents for each of text, layout description, images, videos, etc.

client server communication through messages (NOT streams of data)
- *requests* and *responses* 
![[Pasted image 20240129231319.png]]
image source: [An overview of HTTP - HTTP | MDN (mozilla.org)](https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview)
proxies are intermediaries which perform operations (transform data yippie)

functions of proxies:
- caching
- filtering (i.e. antivirus)
- load balancing (let multiple servers send different requests)
- authentication
- logging

HTTP Flow
- steps for when a client wants to talk with a server
1. open TCP connection (lets you send and receive requests)
2. send an HTTP message
3. read the response from the server
4. close or reuse connection

![[Pasted image 20240129232315.png]]