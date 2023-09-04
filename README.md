# Angular

# Pure Pipes vs Impure Pipes
<pre>
<h3>Pure Pipes:</h3>
A pure pipe is only called when Angular detects a change in the value or the parameters passed to a pipe.

<h3>Impure Pipes:</h3>
An impure pipe is called for every change detection cycle no matter whether the value or parameter(s) changes.
Async is an example of an impure pipe. It is always checking for new input data. 
Pure will be true if not specified. The pure property tells Angular whether or not the value should be recomputed when its input changes.

</pre>
# @ViewChild & @ViewChildren
<pre>
<h3>@ViewChildren —</h3>
component - Returns the specified elements or directives from the view DOM as QueryList
When the parameter is the name of a template variable, the return value will be a reference to the native element.

<h3>ViewChildren vs ContentChildren —</h3>
ViewChildren don’t include elements that exist within the ng-content tag.

ContentChildren includes only elements that exists within the ng-content tag.

<h3>@ContentChildren —</h3>
Returns the specified elements or directives from the content DOM as QueryList
</pre>
Reference: <a href="https://www.youtube.com/watch?v=NJFIEp2RDBM">Reference video</a>

ViewChild & COntentChild Example: <a href="https://stackblitz.com/edit/angular-8-viewchild-example-9uvqjl?file=src%2Fapp%2Fapp.module.ts,src%2Fapp%2Fapp.component.html,src%2Fapp%2Fchild%2Fchild.component.ts,src%2Fapp%2Fapp.component.ts,src%2Fapp%2Fchild%2Fchild.component.html,src%2Findex.html,src%2Fapp%2Fapp.component.css">ViewChild & COntentChild</a>
# Encasuplation:
<pre>
The valid values for this config property are:
ViewEncapsulation.ShadowDom
ViewEncapsulation.Emulated
ViewEncapsulation.None
The default value is <h3>ViewEncapsulation.Emulated</h3>
<h3>In ViewEncapsulation.None:</h3>
There is no shadow DOM.
Style is not scoped to the component.2
ViewEncapsulation.None: If we don’t want to have any encapsulation at all, we can use ViewEncapsulation.None.

If we don't encapsulate anything, the style we defined in the component will leak out and started affecting the other components.

<h3>ViewEncapsulation.Emulated:</h3>
Angular changes our generic css class selector to one that target just a single component type by using automatically generated attributes.

Any styles we define on a component don’t leak out to the rest of the application but with ViewEncapsulation.
Emulated our component still inherits global styles.

<h3>ViewEncapsulation.ShadowDom</h3>
Shadow DOM allows a component to have its own DOM tree which is connected to the element but separated from the children.
It can’t be accessed from the main document and here comes the great advantage. The Component can have its own local style rules.

<h3>ViewEncapsulation.Native:</h3>
If we want Angular to use the shadow DOM we can set the encapsulation parameter to use ViewEncapsulation.Native

With ViewEncapsulation.Native styles we set on a component do not leak outside of the components scope.

This is great if we are defining a 3rd party component which we want people to use in isolation. 
We can describe the look for our component using css styles without any fear that our styles are going
to leak out and affect the rest of the application.
</pre>
# Assignments
<pre>
<a target="_blank" href="https://stackblitz.com/edit/angular-ivy-g6j5pq?file=src%2Fapp%2Fparent.component.ts,src%2Fapp%2Fapp.module.ts,src%2Fapp%2Fparent.component.html,src%2Fapp%2Fapp.component.html,src%2Fapp%2Fchild.component.ts,src%2Fapp%2Fchild.component.html">Get the Data from API and display response</a>
Readymade API - Director List: https://swapi.dev/api/films/
Get Posts: https://jsonplaceholder.typicode.com/posts
Get Posts By Id: https://jsonplaceholder.typicode.com/posts/${postId}
Get User List: https://jsonplaceholder.typicode.com/users
Get User BY Id : https://jsonplaceholder.typicode.com/todos?userId=${post.userId}
  
</pre>
# Angular Hook Methods
<pre>
<a target="_blank" href='https://stackblitz.com/edit/angular-empty-project-t5pppk?file=app%2Fapp.component.html,app%2Fapp.module.ts,app%2Fparent%2Fparent.component.html,app%2Fparent%2Fparent.component.ts,app%2Fchild%2Fchild.component.ts,app%2Fchild%2Fchild.component.html,app%2Fchild%2Fchild.component.css'>My Stack</a>
</pre>
# Encapsulation
<pre>
<a target="_blank" href='https://stackblitz.com/edit/angular-empty-project-omq2fh?file=app%2Fapp.component.html,app%2Fapp.module.ts,app%2Fbottom%2Fbottom.component.html,app%2Fbottom%2Fbottom.component.ts,app%2Ffilter.pipe.ts,app%2Fresult.pipe.ts,app%2Ftop%2Ftop.component.html,app%2Ftop%2Ftop.component.ts,app%2Fbottom%2Fbottom.component.css,app%2Ftop%2Ftop.component.css,styles.css'>My Stack</a>
</pre>
# Routes & Gaurds
<pre>
<a target="_blank" href='https://stackblitz.com/edit/angular-empty-project-p8212j?file=app%2Fapp.module.ts,app%2Fapp.component.html,app%2Fapp.component.ts,app%2Fapp.component.css,app%2Fpagenotfound%2Fpagenotfound.component.html,app%2Fauth.guard.ts,app%2Fproducts%2Fproducts.component.ts'>My Stack</a>
</pre>
# Routing, RouterLink, Route.navigate, Route.navigateByURL
<pre>
<a target="_blank" href='https://stackblitz.com/edit/angular-routing-query-params-ckc5sq?file=src%2Fapp%2Fapp.component.html,src%2Fapp%2Fapp.module.ts,src%2Fapp%2Fapp.component.ts,src%2Fapp%2Fproducts%2Fproducts.component.html'>My Stack</a>
</pre>
# Directives
<pre>
<a target='_blank' href='https://stackblitz.com/edit/angular-hello-world?file=app%2Fhighlight.directive.ts,app%2Fapp.module.ts,app%2Fapp.component.html,app%2Fapp.component.ts'>My StackBlitz</a>
</pre>
# Input&Output Decorator:
<pre>
<a target='_blank' href='https://stackblitz.com/edit/angular-input-output-parent-child-components-example?file=src%2Fapp%2Fchild%2Fchild.component.ts'>My StackBlitz</a>

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
<a href="https://stackblitz.com/edit/switchmap?file=app%2Fapp.component.ts"></a>
<a target='_blank' href='https://stackblitz.com/edit/angular-ivy-yumqp5?file=src%2Fapp%2Fapp.component.ts,src%2Fapp%2Fapp.component.html'> My StackBlitz</a>  
<a target='_blank' href='https://stackblitz.com/edit/my-rxjs-switchmap?file=src%2Fapp%2Fapp.component.ts,src%2Fapp%2Fapp.module.ts'> My StackBlitz</a> 
<a target='_blank' href='https://stackblitz.com/edit/angular-rxjs-switchmap-merge-results-multiple-htt-bfrmd4?file=src%2Fapp%2Fapp.component.ts
'> My StackBlitz</a>  
<a target='_blank' href='https://stackblitz.com/edit/angular-switchmap-rxjs?file=src%2Fapp%2Fapp.component.ts,src%2Fapp%2Fsearch.service.ts'>My SwitchMap Example with http search</a> 
ForkJoin:
<a target='_blank' href='https://stackblitz.com/edit/rxjs-concat-forkjoin-ax4tvk?file=index.ts'>My Stack</a>
</pre>
