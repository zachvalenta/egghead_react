# TODO

Egghead tutorial

# 参考

https://code-cartoons.com/a-cartoon-guide-to-flux-6157355ab207
https://courses.wesbos.com/account
https://code-cartoons.com/a-cartoon-intro-to-redux-3afb775501a6

# D3

https://hackernoon.com/how-and-why-to-use-d3-with-react-d239eb1ea274
https://medium.com/@Elijah_Meeks/interactive-applications-with-react-d3-f76f7b3ebc71 (src for this in `react`)

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