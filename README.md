npm-round-slider
================

[![NPM version][npm-image]][npm-url]
[![Downloads][downloads-image]][downloads-url]

# roundSlider - A free jQuery plugin

========================================================================================================================================
## This project is still under development. I put it aside for the moment to try it in an another way (SVG way and if I succeed, I will add a link to the github). I tried with this fork of roundSlider to organise the code, rewrite it to understand it better and add support of multiple handles accordingly to a configuration object.

## I partialy succeeded in doing it AND what is simply missing is to colorize correctly the good path between handles. If anyone is interested in continuing this project or have an idea, he is the most welcome to contribute.

## Thanks
========================================================================================================================================

### Installation

```
$ npm install npm-round-slider --save
```

### The Sass way

If you like to customize you can either remove the CSS fully and write your own selectors using the Sass mixins or you just use the Sass settings file to customize the look and feel.

To customize the style using the Sass settings file you should copy the settings file to your own Sass folder.

```
cp node_modules/npm-round-slider/dist/scss/settings/_roundslider-settings.scss styles
```

Then just import your copy of the settings file before you import the roundslider.scss file and change the settings in your copy as desired.

```
@import "_my-roundslider-settings";
@import "npm-round-slider/dist/scss/roundslider";
```

Default settings

The settings file contains all relevant variables used in the mixins and while generating the default classes. You can simply change the settings for styling. If you want to override certain settings based on state or pseeudo selectors, you can use the individual mixins to only override specific styles.

Take a look at the settings to see how to customize the style of the default class selectors.

### What's this ?

Round slider (also can call as Circular slider, Radial slider) is a jQuery plugin that allows the user to select a value or range of values.

Not only a round slider, it supports the quarter, half and pie circle shapes also.

![roundSlider - full slider, pie slider, half slider and quarter slider types](/images/sliders.png)

You can check the demos of various circle shapes [here](http://roundsliderui.com/demos.html#various-circle-shapes "various circle shapes - demo").

### Different Theming and Appearances ?

By customizing the CSS styles we can make different appearances.

![roundSlider - different theming and appearances](/images/appearances.png)

You can check the detailed demos [here](http://roundsliderui.com/demos.html#different-theming-and-appearances "different theming and appearances").

### Browser Support

IE 9+, Chrome, Firefox, Safari, Opera (including Mobile devices).

### Options

The roundSlider has several properties and events to interact with the control programmatically. 

To know more about the **Options**, please check the [documentation](http://roundsliderui.com/document.html#options "Documentation about roundSlider Options").

```javascript
	$("#slider").roundSlider({
		min: 0,
		max: 100,
		step: 1,
		value: null,
		radius: 85,
		width: 16,
		handleSize: "+0",
		startAngle: 0,
		endAngle: "+360",
		animation: true,
		showTooltip: true,
		editableTooltip: true,
		readOnly: false,
		disabled: false,
		keyboardAction: true,
		mouseScrollAction: false,
		sliderType: "default",
		circleShape: "full",
		handleShape: "round",
		lineCap: "square",

		// events
		beforeCreate: null,
		create: null,
		start: null,
		drag: null,
		change: null,
		stop: null,
		tooltipFormat: null
	});
```

### Some quick links

- [How to use ?](http://roundsliderui.com/document.html#how-to-install "roundSlider - How to use ?")
- [Customizations](http://roundsliderui.com/demos.html#customizations "roundSlider - Customizations")
- [Different Theming](http://roundsliderui.com/demos.html#different-theming-and-appearances "roundSlider - Different theming and appearances")

### Licence

roundSlider is licensed under the terms of the [MIT license](http://roundsliderui.com/licence.html "roundSlider - MIT licence").

[npm-image]: https://img.shields.io/npm/v/npm-round-slider.svg?style=flat-square
[npm-url]: https://npmjs.org/package/npm-round-slider
[downloads-image]: http://img.shields.io/npm/dm/npm-round-slider.svg?style=flat-square
[downloads-url]: https://npmjs.org/package/npm-round-slider
