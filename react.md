# TODO

- [ ] Egghead tutorial
- [ ] official FB tutorial
- [ ] Corey House tutorial
- [ ] https://github.com/petehunt/react-howto

📍 debug tip: look to higher or lower level of abstraction --> have your debug strats, oblique dev strats, and design strats (unit testing *for design*) open in Sublime at all times

📍 project idea: little React app with canvas/SVG to make a developer version of Oblique Strategies --> move to `#projects`!

first time understanding that sources tab in dev tools is kinda like IDE (with browser also acting as runtime), as compared to more intuitive setup of Python running on your machine and in your IDE i.e. same place

deviation from habits schedule has lead to further deviation (diet)

composible = component has override-able defaults

Architecture of Open Source for mtg w/ Ariel

# 参考

https://github.com/petehunt/react-howto
https://github.com/gaearon/react-makes-you-sad

# JEST

same as Jasmine + mock dependency

# STATE

Flux --> Redux --> Unstated? MobX?
https://code-cartoons.com/a-cartoon-guide-to-flux-6157355ab207
https://courses.wesbos.com/account
https://code-cartoons.com/a-cartoon-intro-to-redux-3afb775501a6

# D3

https://hackernoon.com/how-and-why-to-use-d3-with-react-d239eb1ea274
https://medium.com/@Elijah_Meeks/interactive-applications-with-react-d3-f76f7b3ebc71 (src for this in `react`)

# THINGS FOR DESIGN.MD

__server-side rendering__: ["converting HTML files in the server into usable information for the browser"](https://medium.freecodecamp.org/what-exactly-is-client-side-rendering-and-hows-it-different-from-server-side-rendering-bd5c786b340d) 

not really sure how JAM stack is different than normal SPA

check out that Angular video on SPA, no-framework, with hashes

[server-side actually faster?](http://openmymind.net/2012/5/30/Client-Side-vs-Server-Side-Rendering/)


#THINGS FOR JS.MD

__spread operator__: give all array as args (idky diff than just giving array yet 🙃) https://github.com/wesbos/es6-articles/blob/master/28%20-%20Spread%20Operator%20Introduction.md

__destructuring__: extract obj properties into new var http://wesbos.com/destructuring-objects/

come back to this later --> https://github.com/zachvalenta/tutorial_react_egghead.io/commit/2a84f7d86f460369b6c64cb577fc2f56c95254ee

## REMOVE EL FROM ARRAY LODASH

var array = [1, 2, 3, 4];
var evens3 = _.remove(array, function(n) {return n != 2;});

var array1 = [1, 2, 3, 4];
var evens1 = _.remove(array, (n) => return n == 2;});

indexOf = where does something show up for the first time

# EGGHEAD TUTORIAL

https://github.com/eggheadio-projects/the-beginner-s-guide-to-reactjs

braces are not just string interpolation but any valid JS expression

# FB TUTORIAL

## https://reactjs.org/tutorial/tutorial.html#what-is-react

__component__: class/type
__props__: args to component
__element__: return from component via render(); is JS obj

📝 createElement() is non-JSX equivalent to what the tutorial is doing

📝 HTML file not mentioned in the tutorial but you need it; get it [here](https://codepen.io/gaearon/pen/oWWQNa?editors=1000)

## https://reactjs.org/tutorial/tutorial.html#passing-data-through-props

this.renderSquare(#) --> Square value = # --> class Square this.props.value

## big picture

2011: created
2013: open-sourced
2015: open-sourced React Native
2016: move to semvar w/ React 15

lib, not framework
how are React components rendered: react-dom (web) react-native () react-vr ()
fake JS in HTML (ngFor, v-for) vs. fake HTML in JS (React)
when FB releases breaking change to React will publish codemod (run against your codebase and will automatically translate to newest spec)
JS is fast, the DOM is slow = virtual DOM
layout thrashing: rest of DOM load hindered by update to small piece of DOM
testing: apparently built-in with create-react-app, can test in memory w/ Node vs. having to use the browser, easier bc functions are pure (deterministic, no side effects)
JS syntax (React) vs. template (Angular, Vue) = better at JS, which is exportable from React