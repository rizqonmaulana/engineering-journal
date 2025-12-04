# What Happens When You Type a URL

---

## 1. Browser Checks the Cache

Checks browser cache for DNS entries, cached HTML, CSS, JS, images, or previously loaded resources.

## 2. DNS Lookup (If Not Cached)

Browser asks OS → OS asks DNS resolver → resolver translates the domain name to an IP address.

## 3. Browser Obtains the IP Address

Received IP address is cached in the browser, OS, and DNS resolver, depending on DNS TTL.

## 4. Browser Sends an HTTP/HTTPS Request

Browser opens a TCP/QUIC connection, performs TLS handshake (if HTTPS), then sends the HTTP request.

## 5. Request Travels Through the Internet

Packet goes through modem, router, ISP, internet backbone, CDN, firewall, reverse proxy, or load balancer.

## 6. Server Receives the Request

The server (or CDN edge) accepts the connection and routes it to the correct service or application.

## 7. Server Processes the Request

Backend logic runs: routing, authentication, database queries, business logic, templates, etc.

## 8. Server Sends a Response

Server returns status code, headers, and content (HTML/JSON/assets) over the same network connection.

## 9. Browser Receives and Renders the Page

Browser builds the DOM and CSSOM, runs JavaScript, performs layout and painting, and displays the final UI.

---
