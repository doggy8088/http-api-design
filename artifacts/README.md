### Artifacts

#### Provide machine-readable JSON schema

Provide a machine-readable schema to exactly specify your API. Use
[prmd](https://github.com/interagent/prmd) to manage your schema, and ensure
it validates with `prmd verify`.

#### Provide human-readable docs

Provide human-readable documentation that client developers can use to
understand your API.

If you create a schema with prmd as described above, you can easily
generate Markdown docs for all endpoints with with `prmd doc`.

In addition to endpoint details, provide an API overview with
information about:

* Authentication, including acquiring and using authentication tokens.
* API stability and versioning, including how to select the desired API
  version.
* Common request and response headers.
* Error serialization format.
* Examples of using the API with clients in different languages.

#### Provide executable examples

Provide executable examples that users can type directly into their
terminals to see working API calls. To the greatest extent possible,
these examples should be usable verbatim, to minimize the amount of
work a user needs to do to try the API, e.g.:

```bash
$ export TOKEN=... # acquire from dashboard
$ curl -is https://$TOKEN@service.com/users
```

If you use [prmd](https://github.com/interagent/prmd) to generate Markdown
docs, you will get examples for each endpoint for free.

#### Describe stability

Describe the stability of your API or its various endpoints according to
its maturity and stability, e.g. with prototype/development/production
flags.

See the [Heroku API compatibility policy](https://devcenter.heroku.com/articles/api-compatibility-policy)
for a possible stability and change management approach.

Once your API is declared production-ready and stable, do not make
backwards incompatible changes within that API version. If you need to
make backwards-incompatible changes, create a new API with an
incremented version number.

