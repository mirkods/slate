---
title: API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - Shell
  
toc_footers:
  - <a mailto="digital@talentgarden.org">Get an API key</a>

includes:
  - enrichment
  - errors

search: true
---

# Introduction

Welcome to the Talent Garden API! You can use our API endpoints, which can offer to you a set of tools that you can use to build new products.

We have language bindings in Shell and you can view code examples in the dark area to the right.

# Authentication

> To authorize, use this code:

```shell
# With shell, you can just pass the correct header with each request
curl "api_endpoint_here"
  -H "Authorization: YOUR_API_KEY"
```

> Make sure to replace `YOUR_API_KEY` with your API key.

Talent Garden uses API keys to allow access to the API. You can have an API key <a mailto="digital@talentgarden.org">getting in touch with us</a>.

Talent Garden expects for the API key to be included in all API requests to the server in a header that looks like the following:

`Authorization: YOUR_API_KEY`

<aside class="notice">
You must replace <code>YOUR_API_KEY</code> with your personal API key.
</aside>

