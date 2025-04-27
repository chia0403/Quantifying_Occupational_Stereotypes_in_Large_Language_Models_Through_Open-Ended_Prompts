Once upon a time, there was a server named ajax-server-1 that served a static html page. On every request to this site it would return the data from the html page using the following format:

<script> var thisValue = { foo: 'bar', baz: 'echo', quux: 'foo123'; } </script>

We will examine this in more detail later. Instead, lets write code that can work directly with this data. Notice that in the above example the string "foo123" is being quoted before being sent to the script. When this code is compiled into javascript, the string becomes a variable and it can be accessed directly via thisValue. As such, when we use console.log or console.info on the string (as we will see in a minute), the console logs the value of thisValue directly to the console (as it does not have to be converted before being sent to the script):

var thisValue = { bar: 'foo' }; var v = thisValue.foo; console.log(v.baz); console.log(v.quux);

This is an extremely important thing to grasp when working with dynamic data: variables are treated like any other input and are evaluated like any other data, which means they are available for any program or JavaScript function to interact with. This means that you cannot use variables directly from within any other javascript or application in any