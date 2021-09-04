## CSS Units Explained

### Introduction

If choices to make in CSS units are overwhelming you don't worry this article can help you out. Understanding the basic fundamentals of CSS units is extremely important for any budding Web-based developer. They are the key to styling the way that is easy and friendly across multiple viewports*. 

> *Tip : viewport = Browser-Window Size.


### What is a CSS unit?

A CSS unit determines the size of a property you're setting for an element or its contents. There are various units in CSS to express the measurement and length of a said element. For example, if you want to set the property `padding` for a paragraph, you would give it a specific value.

Let's look at an example : 

```css
p {
   margin: 10px;
}
```
in this case, `padding` is the property, `10px` is the value, and `px` (or "pixel") is the CSS unit.          

### How to know you are using the right CSS units?

Well, there are no such things as you need to use these CSS units for these declarations of for example `padding`, `margin` etc. But if you understand the working behind each CSS unit and the principle behind it then this will help you make your decision much easier. 

### Basic principle of CSS units

#### Absolute Units vs. Relative 

![Absolute vs. Relative Units](https://i.postimg.cc/T1fRLmmK/unidade-relativa-vs-unidade-estatica.gif)

There are mainly two different categories of units: `absolute` and `relative`.

#### Absolute Units

These units are "absolute" that remain the same size regardless of the parent element or viewport*. The size of the element with an absolute unit does not change with the change in the size of the parent element or screen size. 

Absolute units can be useful when working on a project where responsiveness is not being considered. for example, desktop app.

Ex: Typically absolute unit example is `px` as it is widely used. 

`(1px = 1/96th of 1in)`

### Some basic Absolute units examples 

* `px` is used to define the measurement in pixels.
1px = 1/96th of inch.

* `pt` is used to define the measurement in points.
1pt = 1/72 of 1 inch. 

> Tip: these are the two widely used units among the other Absolute units.

#### Relative Units 

These units are "Relative" and can be useful for styling responsive sites because they scale relative to their parent element or viewport. The size of the element with the relative unit does change with the size of the parent element or screen size. 

We can use the relative units as the default for the `responsive elements`. it helps us to avoid update styles for different screen sizes.

Ex: rem is an example for Relative Units 

`(2rem = 2 * root-font size)`

```css
html {
/* root element font size */
font-size: 16px;
}

div{
/* 2 times the font size of root element*/
font-size:2rem;
   }

<html>
<div> Heading </div>
</html>
```
### Some basic Relative units examples

* `%` Percentage is a relative unit used such that it is relative to the parent element.  

If the size of the parent element increased then the size of the child element also increases as it is relative to the parent element.    

![relative unit %](https://i.postimg.cc/fTtjL9zz/ezgif-com-gif-maker.gif)

* `rem` is a relative unit that is Relative to the font size of the root.

if there is a change in root element font size that hence results in the change in the size of the rem value set for a particular element. 

```css
.header {
  font-size: 2rem;
}
```
> tip: 2rem = 2 * 16 (default root font size) = 32px 

* `em` is a relative unit that is relative to the font size of the parent element. 

if there is a change in parent element font size thus results in the change in the size of a particular element with `em` unit set.

 ```css
.child {
  font-size: 0.5em;
}
```

> tip: 0.5em = 0.6 * 16 (parent font size) = 9.6px

* `vw` is a relative unit that is Relative to 1% of the width of the viewport*.

if there is a change in width of the viewport thus results in the change in the size of a particular element with the `vw` unit set. 

![view height](https://i.postimg.cc/FsG5rzZH/vw.gif)

* `vh` is a relative unit that is 	Relative to 1% of the width of the viewport*.

If there is a change in height of the viewport thus results in the change in the size of a particular element with the `vh` unit set.

```css
.wrapper {
  height: 100vh;
}
```
### Bonus 

Yes, there are a lot of other units that I did not include in this article. The core reason being they are not used as widely as the ones I have explained and not to overwhelm you with a lot of together.

But ill leave down a few links that can help you out If you want to learn more.

#### Future Reading

| Links | URL |
| ------ | ------ |
| w3schools | https://www.w3schools.com/cssref/css_units.asp |
| MDN Web docs | https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Values_and_units |
| digitalocean | https://www.digitalocean.com/community/tutorials/css-css-units-explained |

------

Well, that's it for this article. Follow so you don't miss out on the other upcoming articles. 










 











