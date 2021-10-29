# PSR-18: HTTP Client

This document describes a common interface for sending HTTP requests and receiving HTTP responses.

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be interpreted as described in [RFC 2119](http://tools.ietf.org/html/rfc2119).

### Definitions

* **Client** - A Client is a library that implements this specification for the purposes of sending PSR-7-compatible HTTP Request messages and returning a PSR-7-compatible HTTP Response message to a Calling library.
* **Calling Library** -  Calling Library is any code that makes use of a Client. It does not implement this specification's interfaces but consumes an object that implements them (a Client).

### Some List

1. first item
	1. first sub item
2. Second item
	- first sub item
	- second sub item

### Interfaces

**ClientInterface**

```
namespace Psr\Http\Client;

use Psr\Http\Message\RequestInterface;
use Psr\Http\Message\ResponseInterface;

interface ClientInterface
{
    /**
     * Sends a PSR-7 request and returns a PSR-7 response.
     *
     * @param RequestInterface $request
     *
     * @return ResponseInterface
     *
     * @throws \Psr\Http\Client\ClientExceptionInterface If an error happens while processing the request.
     */
    public function sendRequest(RequestInterface $request): ResponseInterface;
}
```

### Some table

first | second | third
--- | --- | ---
*name* | *Sum number* | *Somwe description*
