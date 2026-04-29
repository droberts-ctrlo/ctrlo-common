# @ctrlo/Common

[![Test with Yarn](https://github.com/droberts-ctrlo/ctrlo-common/actions/workflows/nodejs-tests.yml/badge.svg)](https://github.com/droberts-ctrlo/ctrlo-common/actions/workflows/nodejs-tests.yml)

Common module used in some CtrlO libraries

## functions

```javascript
hideElement(el);
```

Hides the element defined in the variable `el` - this has the advantage over JQuery's `hide()` function as it also adds `aria-hidden` to the element

```javascript
showElement(el);
```

Shows the element defined the variable `el` - this has the advantage over JQuery's `show()` function as it also removes the `aria-hidden` attribute from the element should it be present

```javascript
fromJson(item)
```

Converts an item from a string to an object - when the input is unknown (i.e. may be an object or a string) and an object is passed in the function returns the original object. Should there be an error in parsing the object, it will return an empty object.

```javascript
coerceError(item)
```

This function can receive a string or an Error object and is designed for when it is unknown which will be received. It will return the error message, or the original string object, if one is passed in.
