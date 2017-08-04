# Coding Style

# Style Guides

*I happen to be font of the [airbnb style guide](https://github.com/airbnb/javascript).*

JS style/quality guides:
- https://github.com/airbnb/javascript
- https://github.com/rwaldron/idiomatic.js
- https://developer.mozilla.org/en-US/docs/Mozilla/Developer_guide/Coding_Style
- https://standardjs.com
- https://github.com/bevacqua/js
- https://ponyfoo.com/articles/javascript-quality-guide
- http://eloquentjavascript.net/

# Linting

Regarding javascript style and linting: if you haven’t already I suggest you set up your development environment (Atom, Sublime, vim, emacs…) with a linting plugin, and configure it to use the airbnb javascript style. This is a very helpful step to prepare you for contributing to large shared codebases.

This has a lot of benefits. It helps you to write good javascript with uniform style. It helps you to catch syntactical errors in your code right away. And the IDE plugins allow you to see the linting errors (or warnings) right in the code (linters can also be run from the command line, and print out a list of errors — then you need to go back to your code and find the error).

This is a good guide for getting linting setup in Atom: http://www.acuriousanimal.com/2016/08/14/configuring-atom-with-eslint.html

To get interactive linting you’ll install some plugins for your IDE, but note that you’ll almost always be setting up the actual linting configuration on a project-by-project basis. Each project will have a .eslintrc file that defines what style you want to use, and any specific rules you want to check for or ignore.

Take a look at the guide, and let me know if you have any questions!
