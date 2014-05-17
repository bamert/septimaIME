Septima Javascript IME
=====================

This library is still in dev (hence not minified or otherwise finalized yet). A preliminary demo is however available at http://ime.ndb.io
Septima is thought to be used client-sided to enable or force languages or specific keyboard layouts in certain environments.

Planned for the future is to split the input key filter and transformation function (or in case of more complicated IMEs, the statemachine)
in two seperate modules, so as to keep Septima modular and easily extendible by other keyboard layouts.

For now this just serves as an input method of Korean Hangul on my Nokia S60 which otherwise wouldn't support the input of Korean characters (only display). 

Dependencies
-------------

There are no dependencies required, Septima runs stand-alone without any other Javascript Framework or library.

Usage
-----

Instantiating the IME is so far as simple as calling the init method with the argument being the id of a textarea or input field.
As of now it is only possible to attach the IME to one dom element.

JS:
```javascript
window.onload = function(e){
	hangul.init("krinput");
};
```
HTML:
```html
 <textarea id="krinput"></textarea>
```

Demo:

http://ime.ndb.io
