# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: Andrew Valerio

Time spent: 5 hours spent in total

Link to project: (https://glitch.com/edit/#!/eminent-extreme-heart) (https://github.com/AndrewValerio/ColorConcentration)

## Required Functionality

The following **required** functionality is complete:

* [Yes] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [Yes] "Start" button toggles between "Start" and "Stop" when clicked. 
* [Yes] Game buttons each light up and play a sound when clicked. 
* [Yes] Computer plays back sequence of clues including sound and visual cue for each button
* [Yes] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [Yes] User wins the game after guessing a complete pattern
* [Yes] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [Yes] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [Yes] Buttons use a pitch (frequency) other than the ones in the tutorial
* [Yes] More than 4 functional game buttons
* [Yes] Playback speeds up on each turn
* [Yes] Computer picks a different pattern each time the game is played
* [Yes] Player only loses after 3 mistakes (instead of on the first mistake)
* [No] Game button appearance change goes beyond color (e.g. add an image)
* [No] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [Yes] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!
- [ ] Timer has a display and is paused when user presses stop, then resets back to 10 when they click start again.
- [ ] Timer shows that the user loses once time hits zero, an resets as new game is started.

## Video Walkthrough (GIF)

If you recorded multiple GIFs for all the implemented features, you can add them here:

<img src = "http://g.recordit.co/VukN9ooMRK.gif" width = 250><br>
<img src = "http://g.recordit.co/GPLQvTyoUt.gif" width = 250><br>
<img src = "http://g.recordit.co/CBXNcHR39d.gif" width = 250><br>
<img src = "http://g.recordit.co/lWY3qt4liq.gif" width = 250><br>


## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
https://stackoverflow.com/questions/48557368/how-to-stop-countdown-after-zero
https://stackoverflow.com/questions/52909830/typeerror-cannot-read-property-classlist-of-null
https://stackoverflow.com/questions/2450954/how-to-randomize-shuffle-a-javascript-array
https://developer.mozilla.org/en-US/docs/Web/CSS/font-family
https://www.w3.org/wiki/CSS/Properties/color/keywords
https://developer.mozilla.org/en-US/docs/web/javascript/reference/global_objects/math/random

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 
I encountered an error in my code as I was given a "TypeError: Cannot read property 'classList' of null" error which lead to me reviewing the code until I noticed that my id for button was "id = Button1" for all the corrosponding buttons instead of having the 'B' lowercase to "id = button1" for all the buttons. Additionally I encountered another obstacle when developing the guess(btn) function to where after I played a game I wouldn't be able to go through a new game unless i refreshed the page. I even resorted to trying the given algorithm/logic for it with the same issue which I eventually was able to fix by resetting guessCounter to 0 after every successful sequence reproduced by the user that didn't result in the game ending. I drew out how the program was working which helped me vizualize the processes it needed to go through every time it looped through the logic. The problem was that the game would play back the sequence but would think you are at the last button for the sequence before, instead of starting the guesses at the beginning so resetting guessCounter to zero within the loop solved the issue. 

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 
A question I have about web development after this submission is that specifically on this project, what is the most practical and efficient way to have the text in HTML be dynamically modified. In my case I attempted to have a text where it displays the number of strikes you have left as you play, similar to how a countdown timer will function. I used this resource https://www.informit.com/articles/article.aspx?p=2832403&seqNum=12 but I still didn't really understand how to do it in a way that I can develop the function in the script.js file and just have the identifier in the index.html file.

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 
I think I would spend more time on figuring out and understanding the dynamically modified text within the game and use it to add a countdown timer and a number of strikes left indicator as it would add a more intense experience. I would also change my method of making the game speed up as in the beginning it works a little too slow and then in the last sequence before winning it goes a little too fast in my opinion. After that I think I would just add a better color choice to make the game more proffessional looking and mess with the fonts to see what works best.

## Interview Recording URL Link

https://ucr.zoom.us/rec/share/nhjqzJaxcdXRMW2t8xrFHHwLm0sPSn80Wl3zF4acvmXiFZ7lqUtW08Embwj7-m5a.UqTpekT2kGulJTD7?startTime=1648622473000 (Passcode: OKDw8dC&)


## License

    Copyright Andrew Valerio

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
