
# Cheat Sheet #

## Declaring a font-size ##

* We should use ```rem```.
* We should use ```rem``` because those units adapt to the user's system and browser preferences.
* It uses the root font size and scales from that accroding to the factor.

## Setting a width ##

* On most elements we should use ```%```, as well as max-width.
* ```vw``` is a good fit, but you should be careful with it as it my cause some issues.
* ```ch``` is a width of a character of a given font. It's useful as a max-width on a paragraph. A good max-width is ```45ch```.

## Setting a height ##

* Setting a height should be used sparringly.
* Even if a height is needed, set a min-height.
* You should use ```%```, ```rem``` or ```vh```.

## Setting a padding or margin ##

* ```em``` or ```rem``` should be used.
  * ```rem``` units are based on the font-size of the html element.
  * ```em``` units are based on the font-size of the element they are used on.
  * Padding on buttons usually uses ```em``` units.
  * You can set margin-top of all text elements to ```1rem``` and it will be consistent in the entire document.
    * You can change that to ```em``` and the headers will have more spacing as they have a bigger font-size.
