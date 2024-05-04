# React Foundation

## Why do we need `React`

For dynamic website, these libraries make it easier to do DOM manipulation

> React is just an easier way to write normal HTML/CSS/JS.
> It's a new syntax, that under the hood gets converted to HTML/CSS/JS

### Why React?

* People realised it's harder to do DOM manipulation the conventional way
* There were libraries like `JQuery`, but still hard for a very big app
* Eventually, VueJS/React created a new syntax to do frontends
* Under the hood, the React compiler convert your code to HTML/CSS

#### Example:
```html
<!DOCTYPE html>
<html>
<script>
    function onButtonPress() {
        const currentValue = document.getElementById("btn").innerHTML;
        console.log(currentValue.split(" "))
        const currentCounter = currentValue.split(" ")[1];
        const newCounter = parseInt(currentCounter) + 1;
        document.getElementById("btn").innerHTML = "Counter " + newCounter;
    }
</script>

<body>
<button onclick="onButtonPress()" id="btn">Counter 0</button>
</body>

</html>
```
#### Problem with this approach
1. Too much code you have to write as the developer
2. As your app scales (todo app for eg), this gets
   harder and harder.

### Some React Jargon
To create a React app, you usually need to worry about three things
1. Components
2. State
3. Re-rendering
> Note: Creators of frontend frameworks realised that all websites can effectively be divided into two parts `State` and `Components`

#### State
* An object that represents the current `state` of the app.
* It represents the dynamic things in your app (things that change)
* For example, the value of the counter.
```javascript
  {
    count: 1
  }
```

#### Components
* How a DOM element should render, given a state.
* It is a re-usable, dynamic, HTML snippet that changes given the state. 