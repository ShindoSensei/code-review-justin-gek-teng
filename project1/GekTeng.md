# Code Review for GekTeng

## Project Repo

https://github.com/tgt87/wdi-project-1-tgt87

## Review

#### Project Purpose

The purpose of this project is to create a treasure hunt game. The puzzle-styled game involves collecting items in order to defeat a monster and obtain a treasure.

#### Project Organization

#### Features

  * A user is able to click on a button "Place tiles", which allows placement of maximum of 2 tiles on the grid. The logic was implemented by adding a click event listener to each tile and adding the a colored class with each successful click.
  * A user is able to move around coloured tiles using the arrow keys. This is implemented via a keydown event listener that prevents default arrow key behaviour and instead, translates it into 'movement' on the grid using moveOnPath function.

#### Areas of Success (Code, Organization)

* Javascript
  * Variables are named well, example "boy", "monster","shield",etc. It is easy to comprehend what each variable is doing.

  * Cool use of while loop and .includes method in creation of randomGenerate function!


* UI
  * Nice images used, has flavor of actual web games out in the market


* General
  * The game idea is very interesting and most importantly, it's an original concept. I believe this game has longevity and if developed further, will be a game that the market keeps coming back to play!


#### Areas for Improvement (Code, Organization)

* Javascript
  * Add commented headers to divide the logic into different sections for readability.

  * Global variable declarations to be grouped together at the top before functions.

  * Namespacing can be introduced via module pattern. Organise the variables and functions in a larger function. Dom manipulation and click event handlers can be outside this namespaced function.


* CSS
  * For the small images such as the boy, chest,monster,shield and keys, use CSS sprites technique. Combine these images into a single image file and use CSS to "carve out" the appropriate image. This helps with optimisation, as the server need only fetch a single image(composing of all the small images) as opposed to having to fetch a small image(boy/chest/monster/etc..) each time it is needed.
  For more info, visit https://css-tricks.com/css-sprites/


* UX
  * "Place tiles" button could be placed nearer to the grid, for users to easily move between grid and this button. Alternatively, do away with button and have turns reduce automatically every 2 clicks(Apart from first 2 clicks) so player can immediately click on grid without going back and forth.
