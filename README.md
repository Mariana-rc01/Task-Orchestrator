# SO-TP

## Grade: 19/20 :star:

## Building

### Dependencies

 - GNU Make (build-time)
 - GCC (build-time)
 - Doxygen (optional, build-time)

### Building

A release build is achieved with:

``` console
$ make
```

To perform a debug build (no optimizations, debug symbols enabled):

``` console
$ DEBUG=1 make
```

To generate documentation (Doxygen is required):

``` console
$ make docs
```

To remove files generated by a build, run:

``` console
$ make clean
```

To run the orchestrator, run:

``` console
$ cd bin/
$ ./orchestrator <output-folder> N sched-policy
```

To run the client, run:

To run the orchestrator, run:

``` console
$ cd bin/
$ ./client execute time -u "prog-a [args]"
```

or

``` console
$ ./client execute time -p "prog-a [args] | prog-b [args] | prog-c [args]"
```

or

``` console
$ ./client status
```

To run a few tests, run:
(Make sure you have the executables "hello" and "void" in bin/)

``` console
$ bash testScript.sh
```

or

``` console
$ bash smallScript.sh
```

or

``` console
$ bash bigScript.sh
```
