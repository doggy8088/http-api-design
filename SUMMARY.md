## Summary

* [基礎](foundations/README.md)
  *  [要求使用 TLS](foundations/require-tls.md)
  *  [以 Accept 標頭做版本控管](foundations/version-with-accepts-header.md)
  *  [以 ETag 支援快取](foundations/support-caching-with-etags.md)
  *  [以 Request-Id 追蹤需求](foundations/trace-requests-with-request-ids.md)
  *  [以 Range 分頁](foundations/paginate-with-ranges.md)
* [需求](requests/README.md)
  *  [Return appropriate status codes](requests/return-appropriate-status-codes.md)
  *  [Provide full resources where available](requests/provide-full-resources-where-available.md)
  *  [Accept serialized JSON in request bodies](requests/accept-serialized-json-in-request-bodies.md)
  *  [Use consistent path formats](requests/use-consistent-path-formats).
  *  [Downcase paths and attributes](requests/downcase-paths-and-attributes).
  *  [Support non-id dereferencing for convenience](requests/support-non-id-dereferencing-for-convenience).
  *  [Minimize path nesting](requests/minimize-path-nesting.md)
* [回應](responses/README.md)
  *  [Provide resource (UU)IDs](responses/provide-resource-uuids.md)
  *  [Provide standard timestamps](responses/provide-standard-timestamps.md)
  *  [Use UTC times formatted in ISO8601](responses/use-utc-times-formatted-in-iso8601.md)
  *  [Nest foreign key relations](responses/nest-foreign-key-relations.md)
  *  [Generate structured errors](responses/generate-structured-errors.md)
  *  [Show rate limit status](responses/show-rate-limit-status.md)
  *  [Keep JSON minified in all responses](responses/keep-json-minified-in-all-responses.md)
* [產物](artifacts/README.md)
  *  [提供機器可讀的 JSON 大綱](artifacts/provide-machine-readable-json-schema.md)
  *  [提供一般人可讀的文件](artifacts/provide-human-readable-docs.md)
  *  [提供執行範例](artifacts/provide-executable-examples.md)
  *  [描述穩定性](artifacts/describe-stability.md)

