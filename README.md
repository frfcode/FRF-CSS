## CSS

### hierarchy of selectors of css

Example:
```
<p id="demo" class="test" style="color: pink;">Hello World!</p>
```
Therefore the hierarchy is divided into

1. style="color: pink;"
2. id="demo"
3. class="test"
4. p

More info: https://www.w3schools.com/css/css_specificity.asp

### MY MEDIA QUERIES MY STANDAR

```
@media only screen and (max-width: 480px) and (min-width: 300px){}
@media only screen and (max-width: 660px) and (min-width: 481px){}
@media only screen and (max-width: 840px) and (min-width: 661px) {}
@media only screen and (max-width: 992px) and (min-width: 841px){}
@media only screen and (max-width: 1024px) and (min-width: 992px){}
@media only screen and (max-width: 1200px) and (min-width: 1025px){}
@media only screen and (max-width: 1279px) and (min-width: 1201px){}
@media only screen and (max-width: 1919px) and (min-width: 1280px){}
@media only screen and (min-width: 1920px){}

```

### MENU MOBILE WITH CSS

use input checkbox as a parent element to perform some action in the menu at the mobile level, it must be used with absolute position

```
<input type="checkbox" class="demo-menu-checkbox">
<div class="menu-mobile">
    <i class="fa fa-bars" aria-hidden="true"></i>
</div>
<ul class="new-menu">
  <li>
    <a href="#" class="d-text-rubik">FAQ</a>
  </li>
  <li>
    <a href="#" class="d-text-rubik">LOGIN</a>
  </li>
  <li>
    <a href="#" class="d-text-rubik">REGISTER</a>
  </li>
</ul>
/* ACTIVE */
.demo-menu-checkbox:checked ~ .new-menu{
  }
/* INACTIVE */
.dr-menu-checkbox:not(:checked) ~ .new-menu{
  }
```


### FIX PAGES WITH FLEXBOX AND APLICATE RESPONSIVE DESSING

for fix pages with flexbox aplicate flex in your document css, example

```
.container-box {
   flex-direction: row;
   flex-wrap: wrap;
   display: flex;
   margin-right: auto;
   margin-left: auto
}
.container-box_element{
    flex-basis: 25%;
    max-width: 100%;
}

/* FIX FLEXBOX WITH MEDIA QUERIES*/

@media only screen and (max-width: 480px) and (min-width: 300px){
  .container-box_element{
    flex: 1
  }
}

@media only screen and (max-width: 660px) and (min-width: 481px){
   .container-box_element{
    flex: 0.5
  }
}
```
