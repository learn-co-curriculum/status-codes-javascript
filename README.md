# HTTP Status Codes

## Objectives

1. Define status codes and what they communicate to a client
2. Describe the structure and various categories of status codes

## Why Status Codes are Important for the Client

Status codes allow your server to tell something special to the client. The responses you send need to be effective to both a human user and to the browser itself. That means that  response messages like `File Not Found` or `Item isn't in the cart` work if there is a human to read the English. Browsers also want to know the status of the response. To get that response, the HTTP protocol has an agreed upon contract for different "status codes". A status code is a 3-digit integer where the first digit represents the class of the response, and the remaining two digits represent a specific status. There are 5 primary values that the first digit can take.  

### Status Code Chart

Status Number | Code/Description
--------------|--------------------------
1             | 1xx: Informational (request received and continuing process)
2             | 2xx: Success (request successfully received, understood, and accepted)
3             | 3xx: Redirection (further action must be taken to complete request)
4             | 4xx: Client Error (request contains bad syntax and can't be completed)
5             | 5xx: Server Error (server couldn't complete request)

You've probably seen a bunch of these before, the most common being `404`. This means that the server couldn't find the route you requested.

## Video Reviews

* [How the Web Works, Part 1](https://www.youtube.com/watch?v=gI9wqEDPiY0)

* [How the Web Works, Part 2](https://www.youtube.com/watch?v=LSUevS1PRTg)

### Resources
* [More on Status Codes](http://www.tutorialspoint.com/http/http_status_codes.htm)
