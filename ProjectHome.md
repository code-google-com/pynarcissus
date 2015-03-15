Currently this is just a Javascript parser. Javascript evaluation might be a little more tricky since the Narcissus interpreter implements a bunch of stuff metacircularly.

Also, check out the original Narcissus: http://mxr.mozilla.org/mozilla/source/js/narcissus/

This project is interesting not only for the fact that a Javascript parser has been written in Python, but because the port was as direct a transliteration as possible, the Javascript Narcissus parser and this Python one make an interesting case study in the differences between Javascript and Python.

Perhaps I'll post a few interesting line by line comparisons, but in the interim time, jsparser.py is equivalent in function (and indeed incredibly similar at the source level) to Narcissus' jsdefs.js and jsparse.js. You'll have to blame Brendan Eich if you're unhappy with the overall structure and design.

There is also [a conversion routine](http://code.google.com/p/pynarcissus/source/browse/trunk/sexp.py) that turns a Javascript parse tree into rudimentary S-expressions.

**New**: Check out [pyjon](http://code.google.com/p/pyjon)!