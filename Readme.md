<button
  style="
    --width-size: 11px;
  "
>
  Button
</button>

<style>
  calc( var(--width-size) + 2px)
</style>

## I need a way to calculate the values that result.

## resources
https://medium.com/@chuksFestus/understanding-how-css-calc-works-fc994ffa49a6

https://www.google.com/search?q=get+the+computed+value+of+a+div&oq=get+the+computed+value+of+a+div&aqs=chrome..69i57.4928j0j1&sourceid=chrome&ie=UTF-8

https://www.uxpin.com/studio/blog/media-queries-responsive-web-design/

https://www.sitepoint.com/beyond-media-queries-time-get-elemental/

element queries:
https://github.com/tysonmatanich/elementQuery
<br/>https://github.com/filamentgroup/elementary
<br/>https://github.com/Snugug/eq.js
<br/>https://github.com/marcj/css-element-queries

https://hugogiraudel.com/2014/02/06/calc-css-riddle/

## Still to be done:
#### 1) get value of width of div via javascript.
shrink that down to a truncated value.

2020px / 500 = 4px
1501px / 500 = 3px
725px  / 500 = 1px
273px  / 500 = 0px

#### 2) put the truncated chunk variable computed in step 1 into media query
@media only screen and (max-width: calc( var(--x) * 1220px ) {
    .custom { width: calc( var(--x) * 359px ); }
}

#### 3) make sure it works.

