# Cheat Sheet #

# HTML #

## Headings ##

* We have 6 types of headings.
* The biggest heading is ```<h1>```.
  * The second biggest heading is ```<h2>``` and so on until ```<h6>```.
 
## Paragraphs ##

* The ```<p>``` element will just show plain text.

## White Space Collapsing ##

* HTML ignores wide empty spaces.
 
## Image Basics ##

* ```<img src="" alt="">``` the ```src``` attribute is where you type the location of the picture. The ```alt``` attribute is a text which appears when hovering over the image. ```alt``` is very important for blind users as they hear the text via 3rd party softwares.
 * Attributes describe HTML elements.

## Multiple Images ##

* When referencing a ```src```, proper syntax is ```src="./image.png"``` or ```src="./folder/image.png"```.
 * We have the ```./``` because we would like to state it as a relative path for future React or Angular usage.

## External Images ##

* For external images (images which are imported from the web) you need to paste the image URL in the ```src``` attribute.

## Nice Images ##

* For commercial use, we must use allowed photos from various websites like [pexels.com](https://www.pexels.com/), [pixabay.com](https://pixabay.com/) and [gratisography.com](https://gratisography.com/)

## Width and Height (Through HTML) ##

* When setting the ```width```, we also setting the ```height``` (HTML calculates appropriate height by correct ratio).
* We should use images that have the smallest possible dimensions in order to make HTML more efficient.

## External Links ##

* ```<a href="">TEXT HERE</a>``` is the element of links.
 * The ```href``` attribute is the link to the external resource.
 * You can have the ```target``` attribute set to ```_blank``` in order to open the resource in a different tab.

## Internal Links ##

* Same ```<a>``` element, but the ```href``` attribute is an html page/file.

## Same Page Links ##

* We add the ```id``` attribute to an HTML element, and in the ```href``` value we put ```#ID VALUE```

## Images as Links ##

* We use a regular ```<a>``` element and instead of text we put an ```<img>``` element.

## Sup and Sub Elements ##

* Just type the following code in order to see effect:
 * ```<h1>Hello <sup>1st</sup> I'm all <sub>right</sub></h1>```.

## Strong and Em Elements ##

* We should use the ```<strong>``` tag and ```<em>``` in order to make a text bold or italic.
 * If you use it for pure aesthetics, you should do it through css as will be shown later.

## Special Characters ##

* Just google it.

## Ul (Unordered List) and Ol (Ordered List) ##

* ```<ul>``` creates an unordered list (bullets).
 * Then, to make items in the list you should use the tag ```<li>``` (list item).
* ```<ol>``` creates an ordered list (numbered).
* You can nest lists.

## Tables ##

* Use the ```<table>``` tag to create the element.
 * it has 3 sub elements:
  * ```<tr>``` which stands for table row.
  * ```<td>``` which stands for table column.
  * ```<th>``` which stands for table heading.
   * ```<th>``` replaces the ```<td>``` element, and makes the text appear in bold form.

## Forms ##

* ```<form action="" method="">```
 * ```action``` is an attribute which is used to specify where the data will be sent to.
 * ```method``` is an attribute which is used to specify how the data will be sent.
* The ```<input type="">``` element allows you to have a textbox. The ```type``` attribute states the type like text or password.
 * There is the ```name``` attribute which just stands for the name of the data.
 * There is the ```id``` attribute which makes you typing inside the textbox once if it has the same ```form``` attribute as the label.
 * There is the ```placeholder``` tag which shows a grey text when textbox is empty.
 * There is the ```value``` tag which shows an actual value inside the textbox.
* The ```<button type="">``` element allows you to create a button. The ```type``` attribute is the type of button, like submit -> in order to send the data.
* The ```<textarea>``` just shows a lot of text in a certain location. 

## Radio Button (in forms etc.) ##

* You can have radio button with the ```input``` element.
 * ```<input type="radio" name="" id="" value="">TEXT```.
  * The ```name``` attribute specifies a family of buttons. Like a group.
  * The ```TEXT``` is the text which will appear on the button.
  * The ```value``` attribute is the value which will be sent once the form is sent to the server.
  * You can add the ```checked``` attribute in order to have a default option set.

## Checkbox ##

* ```<input type="checkbox" name="" id="" value="">TEXT```.
 * Same attributes as radio buttons.

## Select ##

* ```<select name="" id="">```
 * Has ```<option value="">TEXT</option>``` elements.
 * This is like unordered lists with list items.
 * You can test this in order to see exactly what this HTML tag does.

## Keyboard Shortcuts ##

* [Windows Keyboard Shortcuts Cheat Sheet](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-windows.pdf)

## Div and Span ##

* ```<div>``` and ```<span>``` are used for grouping.
 * ```<div>``` is used to group multiple elements.
 * ```<span>``` is used to group inline content (like text inside a heading/paragrpah etc.).

# CSS #

## Syntax ##

* ```selector {property: value;}```

## Grouping Selectors ##

* You can group selectors like that: ```selector, selector, selector {property:value;}```.

## Id's ##

* Id's go by ```#id {property: value;}```.
* Id's are unique to **one** HTML element. If you would like to assign an id to multiple elements use a class instead.

## Class ##

* Classes go by ```.class {property: value;}```.
* You can have multipe classes on the same HTML element: ```<element class="class1 class2"></element>```.

## Inheritance ##

* Children elements inherit styles from the parent, unless the children have their own styles.
* Also, they inherit only the properties which the are **not** common with the parent.

## Last Rule, Specificity and Universal Selector ##

* Last rule is when we have the same property on one element. It is the last rule (i.e color) which will apply.
* Specificity is like strength. I.e. if you set a color of a paragraph to red, and before that rule you have a class which sets the color to green and apply the class to the paragraph. It will be green. You can google specificity for more information.
* Universal selector is ```* {property: value;}``` and applies styles to all elements. It has the least amount of specificity.

## CSS color and background-color Properties ##

* ```color``` changes the color of the text.
* ```background-color``` changes the background color of an element.

## RGBA ##

* Take 4 numbers, the 4th one is opacity and take value in range(0, 1).

## External Resources For Color ##

* [coolors.co](coolors.co) helps you select amazing color shcemes to your website.

## Calc Functions ##

* You can use ```calc()``` in order to conduct math. I.e. ```calc(100 vh - 100px)```.

## height: auto; min-height; max-height; overflow ##

* ```heihgt: auto;``` is the default value and it sets the height to the minimum heihgt required to contain the child elements/content.
 * When setting the width, the height is automatically calculated to minimally fit all the child elements/content vertically.
* We have the ```overflow``` property which is in charge of the excess content once we set a width the the content does not fit the size we set.
 * The ```hidden``` value hides all content that doesn't fit the size we set it to.
 * The ```scroll``` value makes it so inside the size you set the element to you can scroll with a scroll bar to see additional content.
* The ```min-height``` sets the minimum height of an element. If the content needs more than the minimum height the element will adjust to a size which will fit the content.
* The ```max-height``` set the maximum height of an element. If the content doesnt fit it, use the ```overflow``` property.

## Typography ##

* The ```font-size: value;``` sets the font size to the ```value```.
* The ```font-familty: value;``` sets the actual font of the element.
* You can import custom fonts from [Google Fonts](https://fonts.google.com/).
* The ```font-weight: value;``` is how thick or thin the characters in the text should be.
* ```font-style``` sets font style for a text like ```italic```.

## text-align and text-indent ##

* The ```text-align: value;``` decides the text alignment of an element.
* The ```text-indent: value;``` decides the text indentations of an element. 

## More Text Properties ##

* The ```line-height: value;``` property sets the distance in between the lines.
 * If you use as a ```value``` just a regular number, it means that the value is the number * font size.
* The ```letter-spacing: value;``` property sets the distance between each letter.
* The ```text-decoration: value;``` property sets the text decordation of the element. I.e. on ```<a>``` a ```text-decoration: none;``` will get rid of the underline.
* The ```text-transfrom: value;``` property transforms the text. I.e. to ```uppercase```.

## CSS Box Model ##

![](images/css-box-model.gif)

* You can change padding with ```padding: value;``` or ```padding-top: value;```, ```padding-right: value;```, ```padding-bottom: value;```, ```padding-left: value;```
 * The general ```padding: value;``` can take 4 arguements in the order mentioned above or 1 arguement which will be applied to all 4 sides or 2 arguements which the first represents top and bottom and the second represents right and left.
* 
