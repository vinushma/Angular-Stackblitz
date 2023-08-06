# Angular

# Pure Pipes vs Impure Pipes
<pre>
Pure Pipes:

A pure pipe is only called when Angular detects a change in the value or the parameters passed to a pipe.

Impure Pipes:

An impure pipe is called for every change detection cycle no matter whether the value or parameter(s) changes.
Async is an example of an impure pipe. It is always checking for new input data. Pure will be true if not specified. The pure property tells Angular whether or not the value should be recomputed when its input changes.

</pre>
# Routes & Gaurds
<pre>
<a target='_blank' href='https://stackblitz.com/edit/angular-empty-project-p8212j?file=app%2Fapp.module.ts,app%2Fapp.component.html,app%2Fapp.component.ts,app%2Fapp.component.css,app%2Fpagenotfound%2Fpagenotfound.component.html,app%2Fauth.guard.ts,app%2Fproducts%2Fproducts.component.ts'>My Stack</a>
</pre>
# Filters
<pre>
<a target='_blank' href='https://stackblitz.com/edit/angular-empty-project-fv3fxk?file=app%2Fapp.component.html,app%2Fapp.component.ts,app%2Fapp.module.ts,app%2Ffilter-fruits.pipe.ts,app%2Fmaster.service.ts'>My StackBlitz</a>
<a target='_blank' href='https://stackblitz.com/edit/angular-ivy-yumqp5?file=src%2Fapp%2Fapp.component.ts,src%2Fapp%2Fapp.component.html,src%2Fapp%2Fapp.module.ts,src%2Fapp%2Ffilter.pipe.ts,src%2Fapp%2Fjson.service.ts'>My Stack</a>
</pre>
# Reactive Froms
<pre>
<a target='_blank' href='https://stackblitz.com/edit/angular-hello-world-cpzlgd?file=app%2Fapp.component.html,app%2Fapp.module.ts,app%2Fapp.component.ts'>Reactive form My StackBlitz</a>

Reference:
<a target='_blank' href='https://jasonwatmore.com/post/2022/12/23/angular-14-dynamic-reactive-forms-example#:~:text=Dynamic%20Reactive%20Forms%20Component&text=The%20dynamic%20form%20FormGroup%20contains,directive%20formControlName%3D%22numberOfTickets%22%20.'>Reference</a>
</pre>
# RxJs Operators
<pre>
Switch Map:
<a target='_blank' href='https://stackblitz.com/edit/angular-rxjs-switchmap-merge-results-multiple-http-requests?file=src%2Fapp%2Fapp.component.ts
'>My StackBlitz</a>  
<a target='_blank' href='https://stackblitz.com/edit/angular-ivy-yumqp5?file=src%2Fapp%2Fapp.component.ts,src%2Fapp%2Fapp.component.html'> My StackBlitz</a>  
<a target='_blank' href='https://stackblitz.com/edit/my-rxjs-switchmap?file=src%2Fapp%2Fapp.component.ts,src%2Fapp%2Fapp.module.ts'> My StackBlitz</a> 
<a target='_blank' href='https://stackblitz.com/edit/angular-rxjs-switchmap-merge-results-multiple-htt-bfrmd4?file=src%2Fapp%2Fapp.component.ts
'> My StackBlitz</a>  

ForkJoin:
<a target='_blank' href='https://stackblitz.com/edit/rxjs-concat-forkjoin-ax4tvk?file=index.ts'>My Stack</a>
</pre>
