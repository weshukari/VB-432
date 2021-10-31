# 1. Specification
### 1.1 Basics
* The `LoggerInterface` exposes eight methods to write logs to the eight [RFC 5424](http://tools.ietf.org/html/rfc5424) levels (debug, info, notice, warning, error, critical, alert, emergency).

### 1.2 Message
* Every method accepts a string as the message, or an object with a `__toString()` method. Implementors MAY have special handling for the passed objects. If that is not the case, implementors MUST cast it to a string.