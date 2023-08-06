# Angular

# Pure Pipes vs Impure Pipes
<pre>
Pure Pipes:

A pure pipe is only called when Angular detects a change in the value or the parameters passed to a pipe.

Impure Pipes:

An impure pipe is called for every change detection cycle no matter whether the value or parameter(s) changes.
Async is an example of an impure pipe. It is always checking for new input data. Pure will be true if not specified. The pure property tells Angular whether or not the value should be recomputed when its input changes.

</pre>
# Reactive Froms
<pre>
<a href='https://stackblitz.com/edit/angular-hello-world-nc213h?file=app%2Fapp.component.html,app%2Fapp.module.ts,app%2Fapp.component.ts'>StackBlitz</a>

Reference:
https://jasonwatmore.com/post/2022/12/23/angular-14-dynamic-reactive-forms-example#:~:text=Dynamic%20Reactive%20Forms%20Component&text=The%20dynamic%20form%20FormGroup%20contains,directive%20formControlName%3D%22numberOfTickets%22%20.
</pre>
