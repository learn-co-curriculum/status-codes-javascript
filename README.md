# Status Codes

Status codes are a integral component of a server response. They are a 3-digit integer where the first digit represents the class of the response, and the remaining two digits represent a specific status. There are 5 primary values for the first digit.

### Status Code Chart
Status Number | Code/Description
--|--------------------------
1             | 1xx: Informational (request recieved and continuing process)
2             | 2xx: Success (request successfully recieved, understood, and accepted)
3             | 3xx: Redirection (further action must be taken to complete request)
4             | 4xx: Client Error (request contains bad syntax and can't be completed)
5             | 5xx: Server Error (server couldn't complete request)

### Relation to Rack

In Rack, a status code makes up the first component of the `triplet`, which is the Rack application response that contains the status code, headers, and body. Rack applications are objects that respond to a `call` method. The returned object must be a `triplet`. For example, this is what a triplet looks like:

```ruby
class HelloWorld
  def response
    [200, {}, 'Hello World']
  end
end
```

The first portion of the triplet is the status code, `200`.

### Resources
- [More on Status Codes](http://www.tutorialspoint.com/http/http_status_codes.htm)
