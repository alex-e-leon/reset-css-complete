# reset-css-complete

[Look ma no styles!][1]

## How to use it, or how I learned to stop worrying and install css from npm

`npm i reset-css-complete`

### If using webpack or some other css loader
You can import the css file into your JS directly: `import reset from 'reset-css-complete';`
or you can import it through webpack into your css files with: `@import '~reset-css-complete/reset.css';`

### If not using webpack
You can either reference the css file at `./node-modules/reset-css-complete/reset.css`,
write a script to move it into a new location, or just copy-paste it from this repository

*Note that reset-css-complete doesn't define any typography rules (all elements are set to inherit)
or other global styles so after including reset-css-complete you'll likely also want to define your own
`font:` rules and globals - (I define mine in a second stylesheet with `:root {}`)*

## Why build another reset.css?

Most reset.css files don't actually completely reset all elements.
The most popular reset.css file (Eric Meyer's - which this reset is based on),
doesn't completely reset many elements - including buttons, inputs, links, and more.

So this reset.css takes it up a notch and resets everything it can to plain text
(some funky input elements like color, radio and file can't be completely restyled)

## Why would you want to reset everything?

Resetting everything to a consistent baseline means that you can
__build your styles from the ground up__ and you __never need to reset elements again__.
Not resetting elements globally means you often end up having to reset
buttons or link elements multiple times in different places.
A complete reset.css allows you to use html semantically without worrying whether an element will add any styles.

## What about normalize.css?

normalize.css is another popular baseline css file. Unlike a reset css file,
normalize only attempts to make elements consistent between browsers, but keeps them styled.
If you want h1's to still be larger than h2's or inputs to still look like inputs then normalize might be a good choice.

## Browser support

reset-css-complete has been tested on the latest versions of Chrome, Firefox, Safari, and IE Edge and 11.
It probably works on older browsers too.
If you've tested on an older browser or find an un-reset element, let me know - contributions are also welcome!

Test it yourself or take a look at the beautiful minimilism you'll get at the reset-css-complete
[test page][1].

[1]: https://alex-e-leon.github.io/reset-css-complete/test/

## Thanks

This project was heavily inspired by (and modified from) Eric Meyer's reset.css file
https://meyerweb.com/eric/tools/css/reset/
