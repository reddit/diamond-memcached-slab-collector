# diamond-memcached-slab-collector

A [diamond](https://github.com/python-diamond/Diamond) collector for
collecting statistics on memcached slabs.

## Description

The memcached slab collector will gather all of the statistics output by
`stats slabs`.  By default, you can find the resulting stats in
`servers.[hostname].memcached_slab.*`.

## Installation

Simply drop the collector into `/usr/share/diamond/collectors` and activate
them in your config:

```
[[MemcachedSlabCollector]]
enabled = True
host = localhost  # optional
port = 11211  # optional
```
