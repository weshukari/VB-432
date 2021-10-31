# 1.Specification
### 1.1 Request Handlers


A request handler is an individual component that processes a request and produces a response, as defined by PSR-7.


A request handler MAY throw an exception if request conditions prevent it from producing a response. The type of exception is not defined.



* `Psr\Http\Server\RequestHandlerInterface`


The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be interpreted as described in [RFC 2119](https://datatracker.ietf.org/doc/html/rfc2119).