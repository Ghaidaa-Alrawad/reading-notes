# Class 09

## Review: High-level HTTP

1. What are the five steps in the HTTP Request Lifecycle?

- Step 1: Local Processing 
- Step 2: Resolve an IP 
- Step 3: Establish a TCP Connection 
- Step 4: Send an HTTP Request 
- Step 5: Tearing Down and Cleaning Up

2. What are the two things the client needs before it can make an HTTP Request?

- The intended hostname for the request

- An IP address corresponding to the hostname, obtained through DNS resolution

3. Explain the four way handshake and what it does.

- The client sends a FIN (Finish) packet to the server to indicate that it has finished sending data

- The server responds with an ACK (Acknowledgment) to acknowledge the client's FIN

- The server sends its own FIN packet to the client to indicate that it has also finished sending data

- The client responds with an ACK to acknowledge the server's FIN

This four-way handshake ensures that both the client and server are aware that the connection is being closed.

It helps prevent data loss and ensures that both sides have completed their data transfer before the connection is fully closed.

---

## Java HTTP Request example

1. True or False: When making an HTTP request, you MUST follow any redirect returned by the request. Back up your answer.

False

It's not required to follow redirects returned by the request. Whether we follow redirects or not depends on the specific use case and how we configure the connection.

2. Which built-in Java class can be used to perform an HTTP request?

HttpURLConnection, It's part of the java.net package and allows you to perform basic HTTP requests without the need for additional libraries.

3. What HTTP status codes represent a successful response? A redirect? A client error?

Successful Response: HTTP status codes in the range of 200 to 299 represent successful responses. For example, HTTP_OK (200) indicates that the request was successful.

Redirect: HTTP status codes 301 and 302 are used for redirects. HTTP_MOVED_PERM (301) is a permanent redirect, and HTTP_MOVED_TEMP (302) is a temporary redirect.

Client Error: HTTP status codes in the range of 400 to 499 represent client errors. For instance, HTTP_BAD_REQUEST (400) indicates that the server could not understand the request due to a client error.

---

## Things I want to know more about

- How can I handle more advanced functionalities like adding headers and authentication when using HttpURLConnection?
- What are the benefits and drawbacks of following redirects automatically versus handling them manually?
- How can I effectively handle cookies in Java when making HTTP requests?