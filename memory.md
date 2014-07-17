### On Relaxed Memory Model ###

We are familiar with strongly consistent (*SC*) memory models, in
which there is *the* shared global memory, where writes are strictly
ordered, and the writes are instantly visible to all the processors
simultaneously. This memory model is easy to reason about, but
unfortunately, the model is *wrong* for modern architectures. Thus,
for a faithful semantics, we have to model *relaxed* memory model in
which SC behavior is not expected.

## Example ##

TODO

## Two Ways of Modeling ##

There are two ways to describe a relaxed memory model: *axiomatic*
approach and *operational* approach.

C11/C++11 memory model is described in axiomatic way; on the other
hand, architectures' memory models are typically described in
operational way. In this sense, axiomatic way is a little more
"abstract" than operational way.

# Axiomatic Relaxed Memory Model #

In this kind of model, memory behavior is axiomatized. Basically, an
axiom says something like "If thread B can see an write a2 of thread
A, then B must see the write a1 of A, which is sequenced before a2 in
A". For more details, read
[Mathematizing C++ Concurrency](http://www.cl.cam.ac.uk/~pes20/cpp/popl085ap-sewell.pdf).

# Operational Relaxed Memory Model #

In this kind of model, memory is defined as an abstract machine, on
which operations are defined as a function or a well-defined
relation. [x86-TSO](http://www.cl.cam.ac.uk/~pes20/weakmemory/cacm.pdf)
model is an excellent example.

## Issues ##

We have to decide how to formalize *our semantics model*: in axiomatic
or operational way? Or, even we may have to define in both styles.
