# Whereami

Ipinfo service, with basic memory cache

## Implementations

- Ruby
- Elixir

## Benchmarks

### Ruby

```
ruby[master] $ wrk http://localhost:9292/\?ip\=8.8.8.8
Running 10s test @ http://localhost:9292/?ip=8.8.8.8
  2 threads and 10 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency    14.12ms  100.71ms   1.56s    97.62%
    Req/Sec     3.72k   698.94     7.46k    83.16%
  72714 requests in 10.10s, 16.57MB read
Requests/sec:   7196.46
Transfer/sec:      1.64MB
```

### Elixir

```
elixir[master] $ wrk http://localhost:4000/\?ip\=8.8.8.8
Running 10s test @ http://localhost:4000/?ip=8.8.8.8
  2 threads and 10 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency   606.48us  151.92us   3.96ms   76.80%
    Req/Sec     8.19k   540.42     9.26k    72.77%
  164625 requests in 10.10s, 56.37MB read
Requests/sec:  16299.70
Transfer/sec:      5.58MB
```
