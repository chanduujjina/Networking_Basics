# Networking_Basics

## ✅ 1. Client-Server Architecture

- Client: Browser or any HTTP client (like Postman) sends requests.
- Server: A web server (like Apache Tomcat) hosts the Servlet, processes the request, and returns a response.
- Servlet runs on the server and responds to client HTTP requests.

## ✅ 2. HTTP Protocol (HyperText Transfer Protocol)

- Understanding HTTP is critical because Servlets are HTTP-based.

  Request Methods:
  - GET: To fetch data

  - POST: To submit form/data

  - PUT, DELETE, HEAD, etc.
 
  ## Request-Response Cycle:
  - Client sends a request: URL, headers, body
  - Server (Servlet) processes and returns a response with:
    - Status code (200, 404, 500, etc.)
    - Headers
    - Body (HTML, JSON, etc.)
   
  ## ✅ 3. URL and URI Structure
    - Servlet mappings are based on URL patterns.
  
```bash
      http://localhost:8080/MyApp/hello
 ```

 - http: Protocol
 - localhost: Host (server)
 - 8080: Port
 - MyApp: Web application name
 - /hello: Servlet mapping

## ✅ 4. Ports and IP Address
- Web servers run on IP addresses and ports.
- localhost:8080 means your servlet is being accessed on:
  - IP: 127.0.0.1
  - Port: 8080 (default for Tomcat)

## ✅ 5. TCP/IP Protocol Suite
- HTTP runs over TCP/IP.

- TCP provides:

 - Reliable delivery (no data loss)

 - Connection-based communication

- IP handles:
 - Addressing and routing between client and server.

## ✅ 6. Statelessness of HTTP
 - HTTP is stateless — server doesn't remember clients between requests.
 - Servlets use Session Management to maintain state:
    - Cookies
    - URL Rewriting
    - HttpSession objects
    - 
## ✅ 7. DNS (Domain Name System)
 - Converts domain names (e.g., www.google.com) into IP addresses.
 - Useful when deploying servlet apps to the internet using domains instead of IPs.
 - 
## ✅ 8. Firewall & Security Basics
- Understand how firewalls, proxies, and HTTPS affect servlet access.
- Web apps often run behind a firewall; you must know allowed ports, IPs, and secure headers.
  
## ✅ 9. Request Headers and Response Headers
- These are part of HTTP networking:
- Request Headers:
   - User-Agent, Accept, Host, Cookie, etc.
- Response Headers:
  - Content-Type, Set-Cookie, Cache-Control, Location, etc.
## ✅ 10. Network Latency and Timeouts
- Servlet developers should handle:
  - Slow clients
  - Timeouts
  - Retry logic for backend API/database calls
 
## ✅ Summary Table
| Concept                  | Importance in Servlet Apps                    |
| ------------------------ | --------------------------------------------- |
| Client-Server            | Servlet is server-side, client sends requests |
| HTTP Protocol            | Servlet handles HTTP requests & responses     |
| URL/URI & Port           | Servlet mapping and access                    |
| TCP/IP                   | Underlying network transport                  |
| Statelessness            | Requires session handling in Servlets         |
| DNS                      | Domain name resolution                        |
| Request/Response Headers | Critical for security, cookies, and metadata  |

