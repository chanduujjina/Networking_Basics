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
   
  ✅ 3. URL and URI Structure
    - Servlet mappings are based on URL patterns.
  
  ```bash
      http://localhost:8080/MyApp/hello
 ```
 - http: Protocol
 - localhost: Host (server)
 - 8080: Port
 - MyApp: Web application name
 - /hello: Servlet mapping

✅ 4. Ports and IP Address
- Web servers run on IP addresses and ports.
- localhost:8080 means your servlet is being accessed on:
  - IP: 127.0.0.1
  - Port: 8080 (default for Tomcat)

✅ 5. TCP/IP Protocol Suite
- HTTP runs over TCP/IP.

- TCP provides:

 - Reliable delivery (no data loss)

 - Connection-based communication

- IP handles:
 - Addressing and routing between client and server.
