# Less Mixins
A collection of helpful LESS mixins.

## Similar projects

https://github.com/dmitryf/elements<br/>
https://github.com/madebysource/lesshat<br/>
https://github.com/clearleft/clearless<br/>
https://github.com/mdo/preboot

## Usage

**.font-size(@sizeValue);**<br/>
*Sets font-size as rem with px fallback. Assumes base font size is 16px. You can change base font size by chancing @base-font-size*
```
@base-font-size: 18;
h1 {
	.font-size(24);
}
```
**.inline-block();**<br/>
*Sets display: inline-block and adds IE7 fixes:* \**display: inline;* \**zoom: 1;*

**.text-shadow(@string: 0 1px 3px rgba(0, 0, 0, 0.25));**<br/>

**.box-shadow(@string);**<br/>

**.drop-shadow(@x: 0, @y: 1px, @blur: 2px, @spread: 0, @alpha: 0.25);**<br/>

**.inner-shadow(@x: 0, @y: 1px, @blur: 2px, @spread: 0, @alpha: 0.25);**<br/>

**.box-sizing(@type: border-box);**<br/>

**.border-radius(@radius: 5px);**<br/>

**.border-radiuses(@topright: 0, @bottomright: 0, @bottomleft: 0, @topleft: 0);**<br/>

**.opacity(@opacity: 0.5);**<br/>

**.gradient(@startColor: #eee, @endColor: white);**<br/>

**.horizontal-gradient(@startColor: #eee, @endColor: white);**<br/>

**.animation(@name, @duration: 300ms, @delay: 0, @ease: ease);**<br/>

**.animation-forwards(@name, @duration: 300ms, @delay: 0, @ease: ease);**<br/>

**.transition(@transition);**<br/>

**.transform(@string);**<br/>

**.scale(@factor);**<br/>

**.size(@size);** of **.size(@width, @height);**<br/>
```
.selector:after {
	content: '';
	display: block;
	.size(100px);
}
.selector:before {
	content: '';
	display: block;
	.size(100px, 200px);
}
```
**.rotate(@deg);**<br/>

**.skew(@deg, @deg2);**<br/>

**.translate(@x, @y:0);**<br/>

**.translate3d(@x, @y: 0, @z: 0);**<br/>

**.perspective(@value: 1000);**<br/>

**.transform-origin(@x:center, @y:center);**<br/>