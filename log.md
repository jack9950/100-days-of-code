Day 7 and 8:
**Today’s progress:**
Finished the weather app.

APIs:
  - http://ipinfo.io/developers for the user location lookup (using ip)
  - https://openweathermap.org/api for the weather data
  - http://cloudinary.com/ for free image hosting

To do:
  1. Allow the user to manually enter / change their location
  2. Apply css styles to the app to give it polish

**Thoughts:**
UI design is tough! I need to add some better fonts to the app to make it look better.


**Learned today:**
- backgrounds and backgound sizing
- Positioning the footer at the bottom of the page regardless of screen size and amount of content.


**Links to work:**
https://github.com/jack9950/100-days-of-code
https://github.com/jack9950/Local-Weather
http://codepen.io/jack9950/full/wgzayE/


Day 6: Jan 12th 2017
**Today’s progress:**
Figured out the Weather API icons and got the app pulling in the right icons from the api. Currently displaying weather in Fahrenheit.

APIs:
  - http://ipinfo.io/developers for the user location lookup (using ip)
  - https://openweathermap.org/api for the weather data

To do:
  1. Handle error conditions when the user's location cannot be found
  2. Allow the user to change between Fahrenheit and Celcius
  3. Add a nice background that changes with the user's weather.
  4. Polish up the UI and make it responsive - probably use Bootstrap here again
  5. Allow the user to manually enter / change their location
  6. Apply css styles to the app to give it polish

**Thoughts:**
UI design is tough!


**Learned today:**
-Pulling in external resources like icons
-How to display degrees celcius using decimal, hexadecimal or UTF reference - I used
 the decimal reference in the app.


**Links to work:**
https://github.com/jack9950/100-days-of-code
https://github.com/jack9950/Local-Weather


Day 5: Jan 11th 2017
**Coded for an hour but was too exhausted from work to do anything else, so will summarize last 2 days under Day 6**


Day 4: Jan 9th 2017

**Today’s progress:**
Weather app - got the user location and api calls working properly with ajax.

APIs:
  - http://ipinfo.io/developers for the user location lookup (using ip)
  - https://openweathermap.org/api for the weather data

To do:
  1. Handle error conditions when the user's location cannot be found
  2. Allow the user to change between Fahrenheit and Celcius
  3. Add weather icons
  4. Polish up the UI and make it responsive - probabaly use Bootstrap here again

**Thoughts:**

Learned the *HARD* way that asynchronous (ajax) requests do not stop the rest of script from continuing
The A in ajax stands for asynchronous! I lost a lot of time like so:
  - I initialized a variable outside the ajax function call. I then called the ajax function.
    Within the ajax function, I updated the variable. Once the ajax was done,
    I tried to use the variable (outside the ajax function). I kept getting undefined
    as the value of the variable! After beating my head on Google search for a while,
    I got a brutal reminder... because the request is asynchronous, the script went happily along.
    When I tried to use the variable, the ajax call had not completed,
    so the variable was still undefined! The variable was updated after the ajax call,
    but too late for me to use it! At the time I called the variable, it was still undefined!

**Learned today:**
ajax calls really are asynchronous, as in really really, for real!
The script keeps chugging along without waiting for the ajax call to return.
This is a very good thing, but I have to keep this in mind before trying to use
variables that need to be updated by the ajax code.

**Links to work:**
https://github.com/jack9950/100-days-of-code
https://github.com/jack9950/Local-Weather


Day 3: Jan 8th 2017

**Today’s progress:**
Random Quote Machine: App is now responsive across all screen sizes, small, medium, large and extra large. Used API http://api.forismatic.com/api/1.0/ for the random quotes. Next up, weather app.

**Thoughts:**

Picking great backgrounds is hard. I need a course of designing pages, colors, backgrounds etc.

**Learned today:**
Using backgrounds.

**Links to work:**
https://github.com/jack9950/FCC-Random-Quote-Machine
http://codepen.io/jack9950/full/begvmQ/
https://github.com/jack9950/FCC-Random-Quote-Machine
https://github.com/jack9950/100-days-of-code



Day 2: Jan 6th 2017

**Today’s progress:**
Random Quote Machine: I finally got app resposive to mobile / phone screen. Next step: make it responsive across all screen sizes, small, medium, large and extra large.

**Thoughts:**
Bootstrap makes responsive design a lot easier. I see why it is so popular. Without it I would have to write miles of css and javascript. Based on my limited experience, this is what I guess I would have to do: First create a css grid system for each screen size. Then write the javascript to make the BOM and DOM class changes depending on the screen size. Thank you Bootstrap!

I will continue to refactor the Random Quote Machine code to be responsive to all screen sizes. Over the last week I read through the basic Bootstrap tutorials at http://www.tutorialrepublic.com/twitter-bootstrap-tutorial/ and I will refactor code to use the Bootstrap mobile first responsive 12 column grid.

**Learned today:**
Positioning content, floats, clearfix for floats to return the document flow back to normal, typography shorthand, setting relative line height for text.

**Links to work:**
https://github.com/jack9950/FCC-Random-Quote-Machine
http://codepen.io/jack9950/full/begvmQ/


Day 1: Jan 5th 2017

**Today’s progress:**
Forked the 100-days-of-code repo at https://github.com/jack9950/100-days-of-code. Learned the basics of git and GitHub. Committed my code from the Random Quote Machine to GitHub at https://github.com/jack9950/FCC-Random-Quote-Machine.

**Thoughts:**
I am really starting to love the command line (BASH on Linux Mint). Once I got the hang of it, using command line git to push my code to GitHub was a breeze. If I am serious about becoming a developer, I have to learn how to use Version Control and so far so good with git. Long way to go learning all the nitty gritty details of git, but off to a good start.

I still need to refactor the Random Quote Machine code to be mobile responsive. I will start on this tomorrow. Over the last week I read through the basic Bootstrap tutorials at http://www.tutorialrepublic.com/twitter-bootstrap-tutorial/ and I will refactor code to use the Bootstrap mobile first responsive 12 column grid.

**Learned today:**
Command line git: clone a repository, make changes, stage the changes, commit the changes locally and finally push the commit to remmote repository on GitHub.

**Links to work:**
https://github.com/jack9950/FCC-Random-Quote-Machine
http://codepen.io/jack9950/full/begvmQ/


<!--
## Day 1: 1 Jan 2017
**Today’s progress:**
**Thoughts:**
**Learned today:**
**Links to work:**
-->

<!--

## Day 3: 3 Jan 2017

**Today’s progress:** Finished the responsive large image code (both CSS and JavaScript) for the top section of the portfolio. I might tweak the text behavior a bit more later on, but for now it's working well.

**Thoughts:** It's so time-consuming to adjust a big background image to be responsive. There's probably a library or plugin for this that I don't know about.

**Learned today:** How to combine `background-size: cover;` and `background-position: center;` and write JavaScript to change the way the background behaves on a phone screen. `$(window).height()` is handy.

**Links to work:** “Build a Personal Portfolio Webpage” at Codepen.io: [A Free Code Camp project](http://codepen.io/macloo/full/rjBKLo/) with Bootstrap.


## Day 2: 2 Jan 2017

**Today’s progress:** Built and implemented a working PHP sendmail page for the contact form in my “Build a Personal Portfolio Webpage” project (see [Resources](resources.md) for link). Tested. Works. Note that my contact form is pretty much copied from [here](https://bootswatch.com/sandstone/#forms). Also added large responsive background image to About section. Added a panel to the footer.

**Thoughts:** Lots of time spent on getting that background image to behave nicely. Reworked some JavaScript I figured out previously for another project. Not done with the About section yet. Portfolio section still empty.

**Learned today:** `background-size: contain;` and `background-size: cover;` (CSS) for a responsive background image. I thought `contain` would work, but it turned out that `cover` was what I needed.

**Links to work:** “Build a Personal Portfolio Webpage” at Codepen.io: [A Free Code Camp project](http://codepen.io/macloo/full/rjBKLo/) with Bootstrap.


## Day 1: 1 Jan 2017

**Today’s progress:** Forked the [100 Days Of Code repo](https://github.com/Kallaway/100-days-of-code); updated [Log](log.md) and [Rules](rules.md). Also changed the README to link to the [original repo](https://github.com/Kallaway/100-days-of-code). Started the “Build a Personal Portfolio Webpage” project. Made/edited the navbar and DIVs for each section. Coded social icons, using Font Awesome. Added contact form.

**Thoughts:** Beginning “100 Days Of Code” would be quite a challenge if you'd never used GitHub before. (Of course, it's a great chance to learn to use GitHub!) At [Free Code Camp](https://www.freecodecamp.com/macloo), I’ve completed the Front End Development Certification lessons through “JSON APIs and Ajax” with one exception: “Build a Personal Portfolio Webpage.” Next up: “Intermediate Front End Development Projects."

**Learned today:** How to add jQuery and other files to a Codepen.io project. How to use alert colors as background colors in Bootstrap. How to install Font Awesome via CDN ([see how](http://fontawesome.io/get-started/)), and how to code the icons (yay!).

**Links to work:** “Build a Tribute Page”: [Georgia O’Keeffe, Artist](http://codepen.io/macloo/full/mORjyd/), in which I practiced using Bootstrap. This is a Free Code Camp project I finished earlier. Today I started “Build a Personal Portfolio Webpage”: [Another Free Code Camp project](http://codepen.io/macloo/full/rjBKLo/) with more Bootstrap. I exported today’s code [as a gist](https://gist.github.com/macloo/4448f77d928a7e3283910de0aab9f845).

-->
