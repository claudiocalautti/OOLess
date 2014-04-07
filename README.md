# OOLess - Object Oriented Less

_For faster and more efficient stylesheets that are easier to write and maintain._

## What is it?

OOLess is a template for your css/styles folder, it uses some simple conventions that helps you to write your styles in an organized and clean way, following the object oriented css rules (separate structure and skin, separate container and content).

## How to use

Compile with [Prepros](http://alphapixels.com/prepros/) and use the following options:
- Auto compile
- Compress CSS
- Auto Prefix CSS (required)

## Table of Contents

There is a nice Table of Contents in the style.less so you can look this up quickly while working in your project.

> * RESETS: reduce browser inconsistencies.
* COLORS: variables of all colors in the design.
* FONTS: font-face and main fonts settings.
* SKIN: only backgrounds and shapes mixins or classes.
* GRIDS, SIZES & POSITIONING: general structure.
* ELEMENTS: most used elements like buttons, boxes etc.
* COMMONS & PAGES: pages/sections style built using the previous assets (for example: skin-button-mixin() -> in .button-class{}).
* MEDIAQUERIES: responsive


## Selector Pattern

The following class is an example of the most used css properties in a logical order that make easy to figure out what the selector doing.

>	.example{
		// sizing
		width: 10px;
		height: 10px;
		margin: 10px;
		padding: 10px;
		// positioning
		float: left;
		float: right;
		clear: both;
		position: absolute;
		top: 0;
		left: 0;
		bottom: 0;
		right: 0;
		// skin background
		background: url(../img/some.jpg) no-repeat center;
		background-size: cover;
		// skin border	
		border: 1px solid red;
		border-radius: 10px;
		box-shadow: 1px 1px 3px black;
		// copy
		font: 10px/12px 'Arial';
		text-align: left;
		font-weight: bold;
		font-style: italic;
		color: green;
		// other properties
		z-index: 9;
		overflow: auto;
		display: none;
		// animations
		transition: all 300ms ease-in-out;
		// hover and pseudo selector
		&:hover{
			// children of class on hover
			.child-example{
			}
		}
		&:last-child{
		}
		&:first-child{
		}
		&:before,
		&:after{
		}
		// children of class
		.child-example{
		}
	}








## License

[MIT License](http://opensource.org/licenses/MIT)