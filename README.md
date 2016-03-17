#Angular Highlight

This is a notepad contains some useful link about some issues should be highlight in AngularJS

- $evalAsync execution order

> To summarize:
>
> - if code is queued using $evalAsync from a directive, it should run **after** the DOM has been manipulated by Angular, but **before** the browser renders
> - if code is queued using $evalAsync from a controller, it should run **before** the DOM has been manipulated by Angular (and **before** the browser renders) -- rarely do you want this
> - if code is queued using $timeout, it should run **after** the DOM has been manipulated by Angular, and **after** the browser renders (which may cause flicker in some cases)

- [ ] TODO: use table to easy compare 3 cases

Link: 
http://stackoverflow.com/questions/17301572/angularjs-evalasync-vs-timeout
