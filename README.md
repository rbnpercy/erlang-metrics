erlang-metrics
=======

Just a couple of ways of interacting with Erlang metrics.  Exometer and folsom.

Example:
--------

```erlang


%% initialize an engine
Engine = metrics:init(metrics_exometer),

%% create a counter named TestCounter
ok = metrics:new(Engine, counter, TestCounter),

%% Increment the counter

metrics:increment_counter(Engine, TestCounter).
```


## Build

```
$ rebar3 compile
```