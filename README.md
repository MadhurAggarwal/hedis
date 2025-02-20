# My Work At Juspay's Hedis Fork

Hi! This is a fork of Redis Client library for Haskell, where Juspay Contributes publically.
<br>
I worked on performance measurements, by adding the command:
```
WAIT n/2 50
```
on MultiExec, to improve consistency of critical writes, effectively testing a more CP-oriented system for critical writes and the standard AP-oriented system for normal writes.
<br>
Ask me for the Perf-measurements results!

<hr>

# Welcome to hedis

[![Build Status](https://travis-ci.org/informatikr/hedis.svg?branch=master)](https://travis-ci.org/informatikr/hedis)

This is a Redis client library for the Haskell programming language. Please consult the library's [Hackage page](http://hackage.haskell.org/package/hedis) for documentation.

# Testimonials

Ben Gamari
[writes](https://groups.google.com/forum/?fromgroups#!topic/redis-db/uJSp7ZcQTew):

> Having evaluated the options in this space, [Hedis] is in my opinion the best
> of the bunch with an active maintainer, a simple interface, excellent 
> documentation, and superb performance.

Email from a user, regarding the 0.5 release (10.05.2012):

> The new multiExec function is really great. [...] We are using it in our
> commercial product at Janrain and are very happy!

Andrew Frederick Cowie [mentioned hedis](http://research.operationaldynamics.com/~andrew/talks/TheWebProblem,SolvingItInHaskell/TheWebProblem.html#Redirector introduction) in a talk:

> _Nice_ Haskell bindings.

# Join in!

We are happy to receive bug reports, fixes, documentation enhancements, and other improvements.

Please report bugs via the [github issue tracker](http://github.com/informatikr/hedis/issues).

Master [git repository](http://github.com/informatikr/hedis):

    git clone git://github.com/informatikr/hedis.git

# Authors

This library is written by Falko Peters <falko.peters@gmail.com>.
Currently maintainer by Kostiantyn Rybnikov <k-bx@k-bx.com>.


## Getting started
### Development
#### Services
You can start a redis server using flakes.
```
nix run .#redis-service
```
This will start a redis server in standalone and clustered modes in your system.

#### DevShell
```
nix develop
```

### Build
```
nix build
```



