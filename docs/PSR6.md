### PSR-6: Caching Interface Zakiev VB-432
## Goal
The goal of this PSR is to allow developers to create cache-aware libraries that can be integrated into existing frameworks and systems without the need for custom development.
# Definitions
- **Calling Library** - The library or code that actually needs the cache services. This library will utilize caching services that implement this standard's interfaces, but will otherwise have no knowledge of the implementation of those caching services.
- **Implementing Library** - This library is responsible for implementing this standard in order to provide caching services to any Calling Library. The Implementing Library MUST provide classes which implement the Cache\CacheItemPoolInterface and Cache\CacheItemInterface interfaces. Implementing Libraries MUST support at minimum TTL functionality as described below with whole-second granularity.
- **Expiration** - The actual time when an item is set to go stale. This is typically calculated by adding the TTL to the time when an object is stored, but may also be explicitly set with DateTime object. An item with a 300 second TTL stored at 1:30:00 will have an expiration of 1:35:00. Implementing Libraries MAY expire an item before its requested Expiration Time, but MUST treat an item as expired once its Expiration Time is reached. If a calling library asks for an item to be saved but does not specify an expiration time, or specifies a null expiration time or TTL, an Implementing Library MAY use a configured default duration. If no default duration has been set, the Implementing Library MUST interpret that as a request to cache the item forever, or for as long as the underlying implementation supports.
# Data
Strings | Integers | Floats
Character strings of arbitrary size in any PHP-compatible encoding. | All integers of any size supported by PHP, up to 64-bit signed. | All signed floating point values.
PSR6 more info [link](https://www.php-fig.org/psr/psr-6/)