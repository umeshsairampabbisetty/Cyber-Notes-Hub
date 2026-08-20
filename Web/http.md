What is HTTP? (HyperText Transfer Protocol) -> set of rules used while communicating with servers

What is a URL? (Uniform Resource Locator)
• Scheme: Protocol used to access the resource (e.g., HTTP, HTTPS, FTP).
• User: Optional username and password embedded in the URL for authentication.
• Host: Server's domain name or IP address.
• Port: Connection port number (typically 80 for HTTP, 443 for HTTPS; range is 1 to 65535).
• Path: Specific file name or resource location on the server.
• Query String: Additional data sent to the path (e.g., ?id=1).
• Fragment: Reference to a specific section or anchor location on the page.


-the two steps of sending and receiving information through the http protocol-

1st - the request
    GET / HTTP/1.1
    Host: website.com
    User-Agent: Mozilla/5.0 Firefox/87.0
    Referer: https://website.com/
    
2nd - the response
    HTTP/1.1 200 OK
    Server: nginx/1.15.8
    Date: Fri, 09 Apr 2021 13:34:03 GMT
    Content-Type: text/html
    Content-Length: 98

    <html>
    <head>
        <title>hello</title>
    </head>
    <body>
        Welcome To my home page
    </body>
    </html>

- Purpose: HTTP methods define the client's intended action when making a request.
• GET: Retrieves information from a web server.
• POST: Submits data to the web server, often used to create new records.
• PUT: Submits data to update existing information on the web server.
• DELETE: Removes information or records from a web server.

- HTTP Status Code Ranges
• 1xx (Informational): Request received, continue processing.
• 2xx (Success): Request successfully completed.
• 3xx (Redirection): Further action required to complete request.
• 4xx (Client Error): Bad request or unauthorized/forbidden access.
• 5xx (Server Error): Server failed to fulfill a valid request.
Common HTTP Status Codes
• 200 OK: Request completed successfully.
• 201 Created: New resource successfully created.
• 301 Moved Permanently: Resource permanently moved to a new URL.
• 302 Found: Temporary redirect to a different URL.
• 400 Bad Request: Invalid or malformed request.
• 401 Unauthorized: Authentication required.
• 403 Forbidden: Access denied regardless of login state.
• 404 Not Found: Requested resource does not exist.
• 405 Method Not Allowed: HTTP method not supported for this resource.
• 500 Internal Server Error: Generic server-side error.
• 503 Service Unavailable: Server overloaded or down for maintenance.
