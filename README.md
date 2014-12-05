# HTTP API 設計指南

## Introduction

This guide describes a set of HTTP+JSON API design practices, originally
extracted from work on the [Heroku Platform API](https://devcenter.heroku.com/articles/platform-api-reference).

This guide informs additions to that API and also guides new internal
APIs at Heroku. We hope it’s also of interest to API designers
outside of Heroku.

Our goals here are consistency and focusing on business logic while
avoiding design bikeshedding. We’re looking for _a good, consistent,
well-documented way_ to design APIs, not necessarily _the only/ideal
way_.

We assume you’re familiar with the basics of HTTP+JSON APIs and won’t
cover all of the fundamentals of those in this guide.

We welcome [contributions](CONTRIBUTING.md) to this guide.

