# reset-css-complete

[Look ma no styles!][1]

## Why build another reset.css?

Most reset.css files don't actually completely reset all elements.
The most popular reset.css file (Eric Meyer's - which this reset is based on),
doesn't completely reset many elements - including buttons, inputs, links, and more.

So this reset.css takes it up a notch and resets everything it can to plain text
(some funky input elements like color, radio and file can't be completely restyled)

## Why would you want to reset everything?

Resetting everything to a consistent baseline means that you can build your styles from the ground up.
Any elements you don't reset globally that you want to customize requires you to reset them inside the styles you write.
This means you often end up having to reset buttons or link elements multiple times.
A complete reset.css means that you can use html semantically without worrying about adding unwanted styles.

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
