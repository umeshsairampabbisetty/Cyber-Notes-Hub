-the two steps of sending and receiving information through the http protocol-

1st - the request
    GET / HTTP/1.1
    Host: tryhackme.com
    User-Agent: Mozilla/5.0 Firefox/87.0
    Referer: https://tryhackme.com/
    
2nd - the response
    HTTP/1.1 200 OK
    Server: nginx/1.15.8
    Date: Fri, 09 Apr 2021 13:34:03 GMT
    Content-Type: text/html
    Content-Length: 98

    <html>
    <head>
        <title>TryHackMe</title>
    </head>
    <body>
        Welcome To TryHackMe.com
    </body>
    </html>

- Purpose: HTTP methods define the client's intended action when making a request.
• GET: Retrieves information from a web server.
• POST: Submits data to the web server, often used to create new records.
• PUT: Submits data to update existing information on the web server.
• DELETE: Removes information or records from a web server.
