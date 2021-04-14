## Images

* If you use images, they should:

    * Be relevant
    * Convey information
    * Convey the right mood
    * be instantly recognisable
    * Fit the color palette

* If you are building a site from scratch, it is good practice to create a folder for all of the images the site uses.

* add an image into the page you need to use an ```<img>``` element. This is an empty element.

* ```src``` Tells the browser where to find the image.

* ``alt`` Provides a text description of the image.

* ```title``` Provides additional informations about the image.

* ```height``` this specifies the height of the image in pexels.

* ```width``` this specifies the width if the images in pixels.

* images can be placed before the paragraoh, inside it the start of it, and in the middle of it.

* Three rules for creating images
    1. Save images in the right format
    
    2. Save images at the right size

    3. Use the correct resolution.

* Animated GIFs show several frames of an image in sequence and therefore can be used to create simple animations.

* Creating an image that is partially transparent 
(or "see-through") for the web involves 
selecting one of two formats:
    
    * Transparent GIF
    * PNG

* ```<figure>``` is element used to contain images and their caption so that the two are associated.

* ```<figcaption>``` element has been added to HTML5 in order to allow web page authors to add a caption to an image.

## Color

* he color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:

* RGB values These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,100,90).

* HEX codes These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign. For example: ```#ee3e80``` .

* Color names There are 147 predefined color names that are recognized by browsers. For example: DarkCyan.

* Every color on a computer screen is created by mixing amounts of red, 
green, and blue. To find the color you want, you can use a color picker.

* HUE is near to the colloquial idea of color. Technically speaking however, a color can also have saturation and brightness as well as hue.

* Saturation refers to the amount of gray in a color. At maximum saturation, there would be no gray in the color. At minimum saturation, the color would be mostly gray.

* Brightness (or "value") refers to how much black is in a color. At maximum brightness, there would be no black in the color. At minimum brightness, the color would be very dark.

* When picking foreground and background colors, it is important to ensure that there is enough contrast for the text to be legible.

* Opacity property which allows you to specify the opacity of an element and any of its child elements. The value is a number between 0.0 and 1.0

* rgba property allows you to specify a color, just like you would with an RGB value, but adds a fourth value to indicate opacity.

* hsl color property that is an alternative way to specify colors. contains HUE, Saturation, and Lightness.

* hsla color property is same as hsl but with fourth value Alpha. Alpha expressed as a number between 0 to 1.0 represents transperency.

## Text

* Serif fonts have extra details on the ends of the main strokes of the letters. These details are known as serifs.

* Sans-serif fonts have straight ends to letters, and therefore have a much cleaner design.

* Every letter in a monospace (or fixed-width) font is the same width.(Non-monospace fonts have different widths.)

* Cursive fonts either have joining strokes or other cursive characteristics, such as handwriting styles.

* Fantasy fonts are usually decorative fonts and are often used for titles. They're not designed for long bodies of text.

* When choosing a typeface, it is important to understand that a browser will usually only display it if it's installed on that user's computer.

* The ```font-family``` property allows you to specify the typeface that should be used for any text inside the element(s) to which a CSS rule applies.

* The ```font-size``` property enables you to specify a size for the font. There are several ways to specify the size of a font. The most common are: Pixels, Percentages, and EMs.

* ```@font-face``` allows you to use a font, even if it is not installed on the computer of the person browsing, by allowing you to specify a path to a copy of the font, which will be downloaded if it is not on the user's machine.

* The ```font-weight``` property allows you to create bold text. There are two values that this property commonly takes: normal and bold.

* The ```text-transform``` property is used to change the case of text giving it one of the following values: uppercase, lowercase, and capitalize.

* The ```text-decoration``` property 
allows you to specify the 
following values: none, underline, overline, line-through, and blink.

* The ```text-align``` property allows 
you to control the alignment of 
text. The property can take one 
of four values: left, right, center, and justify.

* The ```vertical-align``` property is a common source of confusion. It is not intended to allow you to vertically align text in the middle of block level elements such as ```<p>``` and ```<div>```, although it does have this effect when used with table cells (the ```<td>``` and ```<th>``` elements). It is more commonly used with inline elements such as ```<img>```, ```<em>```, or ```<strong>``` elements.

* The ```text-indent``` property allows you to indent the first line of text within an element. The amount you want the line indented by can be specified in a number of ways but is usually given in pixels or ems.

* The ```text-shadow``` property used to create a drop shadow, which is a dark version of the word just behind it and slightly offset. It can also be used to create an embossed effect by adding a shadow that is slightly lighter than the text.

* You can specify different values for the first letter or first line of text inside an element using ```:first-letter``` and ```:first-line.```

* ```:link``` This allows you to set styles for links that have not yet been visited.

* ```:visited``` This allows you to set styles for links that have been clicked on.

* ```:hover``` This is applied when a user hovers over an element with a pointing device such as a mouse.

* ```:active``` This is applied when an element is being activated by a user; for example, when a button is being pressed or a link being clicked.

## JPEG vs PNG vs GIF

* JPEG format used for all images that contain a natural scene or photograph where variation in colour and intensity is smooth.

* PNG format used for any image that needs transparency or for images with text & objects with sharp contrast edges like logos. Use GIF format for images that contain animations.

* Compression types:

    1. lossless compression, it is possible to reconstruct the original image from the compressed image because there is no information loss during compression.

    2. lossy compression dat loss is irreversible, and its algorithms always have a superior compression ratio.

    * JPEG is a lossy compression specification that takes advantage of human perception.

    * PNG is a lossless image format using DEFLATE compression. No data is lost during compression and no compression artefacts are introduced in the image.

    * GIF is also a lossless image format that uses LZW compression algorithm. It was favoured over PNG for simple graphics in websites in its early days because the support of PNG was still growing.

* Transparency indicates something that is completely invisible. Logos and icons often need to be placed on backgrounds with variable colours.

    * JPEG images don’t support transparency and are hence not usable for such cases.

    * PNG images support transparency in two ways — inserting an alpha channel that allows partial transparency or by declaring a single colour as transparent (index transparency).

    * GIF images support transparency by declaring a single colour in the colour palette as transparent (index transparency). 

* Colors

    * JPEG images can support around 16 million colours. This is what makes them suitable for storing images of natural scenes.

    * PNG images mainly have two modes — PNG8 and PNG24. PNG8 can support upto 256 colours whereas PNG24 can handle upto 16 million colours like a JPEG image.

    * GIF images are limited to 256 colours. If index transparency is used, then one of these 256 colours is assigned as transparent and the remaining 255 are used for other colours.

* Animation, in this case, refers to any change or movement in the image. It doesn’t necessarily have to have frame rates like an animated video, but essentially a part or the entire image changes with time.

    * Of these 3 formats, only GIF supports animation. This capability makes GIF format suitable for delivering engaging ads and banners.

    [Back to Home](README.md)
