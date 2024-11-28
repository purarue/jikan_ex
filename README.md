# JikanEx [![Build Status](https://travis-ci.org/purarue/jikan_ex.svg?branch=master)](https://travis-ci.org/purarue/jikan_ex) [![Hex.pm](http://img.shields.io/hexpm/v/jikan_ex.svg?style=flat)](https://hex.pm/packages/jikan_ex) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)

# STATUS

This is defunct, both because it is old code (and I think the Telsa (HTTP lib) library has drifted too far, `ssl` no longer compiled, and its on an old version of Jikan (v3, not v4). I would only use this as example code to perhaps make a new API client.

---

A thin elixir wrapper for the [Jikan](https://github.com/jikan-me/jikan) API.

See the [documentation](https://hexdocs.pm/jikan_ex) for usage.

### Quickstart

```elixir
alias JikanEx.Request
client = JikanEx.client()
response = client |> Request.anime!(1)
IO.puts response["title"]  # Prints 'Cowboy Bebop'
```

## Installation

Add the following to your `mix.exs`:

```elixir
def deps do
  [
    {:jikan_ex, "~> 0.1.5"}
  ]
end
```
