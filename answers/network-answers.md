# Network Questions

#### Traditionally, why has it been better to serve site assets from multiple domains?

Browsers usually have a limit on the number of concurrent downloads they can
handle from a single domain at any given moment. Serving assets from multiple
domains helps increase the concurrency level, allowing users' browsers to fetch,
cache, and use more things at once.

#### Do your best to describe the process from the time you type in a website's URL to it finishing loading on your screen.

When I type a website's URL into my browser, it asks a local DNS server the IP
address of the URL I give it. We know the local DNS server's IP address from the (DHCP)[https://en.wikipedia.org/wiki/Dynamic_Host_Configuration_Protocol].

The server fetches my IP by three-way handshake, and my browser tries to
establish a TCP/UDP connection. If successful, my browser forms an HTTP request
containing a header and body and sends it to the server -- the server returns an
HTTP code and response. My browser will parse this response's head and body, and
renders the website from that information. If the website's document contains
additional asset links, my browser will send subsequent HTTP requests to the
asset domains and send them in the same way as the server above.

#### What are the differences between Long-Polling, Websockets and Server-Sent Events?

- **Long-Polling**: Clients request webpages from servers using HTTP requests --
  requested webpages execute JavaScript, which request subsequent files from the
  server. Servers wait until new information is available before sending it back
  to the client. Clients then receive this new information and immediately send
  new requests to the server, restarting the process.
- **Server-Sent Events** (SSEs): Clients request webpages from servers using
  HTTP requests (like in long-polling), which execute JavaScript and open
  connections to a server. Clients receive automatic updates from the server,
  and don't have to continually poll the server for new updates.
- **WebSockets**: In contrast to Server-Sent Events, WebSocket connections can
  both send *and* receive data from an application.

#### Explain the following request and response headers:

 * Diff. between Expires, Date, Age and If-Modified-...
  * Do Not Track
  * Cache-Control
  * Transfer-Encoding
  * ETag
  * X-Frame-Options

#### What are HTTP actions? List all HTTP actions that you know, and explain them.
