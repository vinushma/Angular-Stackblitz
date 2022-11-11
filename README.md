# Angular

# Pure Pipes vs Impure Pipes
<pre>
Pure Pipes:

A pure pipe is only called when Angular detects a change in the value or the parameters passed to a pipe.

Impure Pipes:

An impure pipe is called for every change detection cycle no matter whether the value or parameter(s) changes.
Async is an example of an impure pipe. It is always checking for new input data. Pure will be true if not specified. The pure property tells Angular whether or not the value should be recomputed when its input changes.

</pre>
