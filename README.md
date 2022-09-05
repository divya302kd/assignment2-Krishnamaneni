# assignment2-Krishnamaneni
# Krishnamaneni Divya
## My favourite museum is Salar Jung museum
Museums are buildings in which we see many things of **artistic**, cultural, historical, traditional and objects of **scientific** interest. 
***
Rajiv Gandhi International Airport is near to Salar Jung museum
## Route map to Titanic museum
1. Maryville
2. Kansas city
    1. Airport
    2. terminal departures
    3. take a flyt to Newyork city
3. Newyork Airport
    1. Terminal departures
    2. Take a flyt to Hyderabad city
4. Rajiv Gandhi International Airport
    1. Terminal Departure
    2. Come out from airport
    3. Book a cab to go to Salar jung museum
* Jamal market shopping complex
    * Fruits
    * Electronics
* Nizam museum
* Chowmahalla Palace
* Laad bazar
    * shopping
    * clothes

**[link to aboutme](AboutMe.md)**

***
# About famous cities
The following table describes famous cities everyone must visit.
|Name of city|Important location|Time   |
|:---------: |:----------------:|:-----:|
| Newyork    | Statue of Liberty|3 hours|
| Tokyo      | tokyo skytree    |4 hours|
| London     | British museum   |5 hours|
| Paris      | Eiffel tower     |5 hours|

***
# Pithy Quotes
>"Life is a journey, not a destination."
>Author: *Ralph Waldo Emerson*<br>
>"Enthusiasm makes up for a host of deficiencies."
>Author: *Barack Obama*

***
# Code fencing
>Material Design has been all over the place lately. One part of it consists on stacking layers on top of each others like real paper sheets. To achieve such an effect in CSS, we need to use the box-shadow property. To avoid having to manually write the shadows every time, we can build a little Sass mixin for it. The only thing this mixin will do is outputting a box-shadow declaration based on the given $depth (from 0 to 5). Shadows will actually be computed by two functions: bottom-shadow and top-shadow. Quick link to the source<https://stackoverflow.com/questions/17098818/what-is-wrong-with-my-box-shadow-sass-mixin>

```
@mixin card($depth) {
  @if $depth < 1 {
    box-shadow: none;
  } @else if $depth > 5 {
    @warn "Invalid $depth `#{$depth}` for mixin `card`.";
  } @else {
    box-shadow: bottom-shadow($depth), top-shadow($depth);  
  }
}
@function top-shadow($depth) {
  $primary-offset: nth(1.5 3 10 14 19, $depth) * 1px;
  $blur: nth(1.5 3 10 14 19, $depth) * 4px;
  $color: rgba(black, nth(.12 .16 .19 .25 .30, $depth));

  @return 0 $primary-offset $blur $color;
}

/// Computes a bottom-shadow for a card effect.
/// @param {Number} $depth - depth level
/// @return {List}
@function bottom-shadow($depth) {
  $primary-offset: nth(1.5 3 6 10 15, $depth) * 1px;
  $blur: nth(1 3 3 5 6, $depth) * 4px;
  $color: rgba(black, nth(.24 .23 .23 .22 .22, $depth));

  @return 0 $primary-offset $blur $color;
}
```
Quick link to the code<https://css-tricks.com/snippets/sass/material-shadows-mixin/>


