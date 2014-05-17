Septima Javascript IME
=====================

This library is still in dev (hence not minified or otherwise finalized yet). A preliminary demo is however available at http://ime.ndb.io
Septima is thought to be used client-sided to enable or force languages or specific keyboard layouts in certain environments.

Planned for the future is to split the input key filter and transformation function (or in case of more complicated IMEs, the statemachine)
in two seperate modules, so as to keep Septima modular and easily extendible by other layouts.

For now this serves as an input method of Korean Hangul on my Nokia S60 which otherwise wouldn't support the input of Korean characters (only display). 

Dependendcies
-------------

There are no dependencies required, Septima runs stand-alone without any other Javascript Framework or library.

Usage
-----

Instantiating the ime is so far as simple as 

JS:
	<script>
		window.onload = function(e){
			hangul.init("krinput");
		};
	</script>

HTML:

	 <textarea id="krinput"></textarea>
 

Demo:

http://ime.ndb.io
