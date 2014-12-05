#### Trace requests with Request-Ids

Include a `Request-Id` header in each API response, populated with a
UUID value. If both the server and client log these values, it will be
helpful for tracing and debugging requests.
