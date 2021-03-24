# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: Ashani Jewell

Time spent: **12** hours spent in total

Link to project: (https://glitch.com/edit/#!/ashani-jewell-project)

## Required Functionality

The following **required** functionality is complete:

* [x] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [x] "Start" button toggles between "Start" and "Stop" when clicked. 
* [x] Game buttons each light up and play a sound when clicked. 
* [x] Computer plays back sequence of clues including sound and visual cue for each button
* [x] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [x] User wins the game after guessing a complete pattern
* [x] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [x] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [x] Buttons use a pitch (frequency) other than the ones in the tutorial
* [x] More than 4 functional game buttons
* [x] Playback speeds up on each turn
* [ ] Computer picks a different pattern each time the game is played
* [x] Player only loses after 3 mistakes (instead of on the first mistake)
* [x] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn
 
The following **additional** features are implemented:

- [x] Named the individual buttons
- [x] Added a hover affect on buttons
- [x] Changed the button sizing of the game buttons and margins


## Video Walkthrough

Here's a walkthrough of implemented user stories:
Example of using all three chances and losing.
![](https://cdn.glitch.com/a18594b5-3020-4121-b204-3f8a6b924e0d%2Fezgif.com-video-to-gif.gif?v=1616118252420)
Example of playing the pattern and repeating it back. Example of winning the game.
![](https://cdn.glitch.com/a18594b5-3020-4121-b204-3f8a6b924e0d%2Fezgif.com-video-to-gif%206.gif?v=1616405439668)

## Reflection Questions
1. <b>If you used any outside resources to help complete your submission (websites, books, people, etc) list them here.</b>
- w3schools
- stackoverflow
- geeksforgeeks
- tutorialspoint


2. <b>What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) </b>
My first challenge started when I was working on sprucing up the buttons. I started by going to the website about <img> tag’s and tried to use the sample line they had as a template for my image, but I was still not seeing a picture. I did a little more digging to find that the “src” variable was actually a URL, so I would have to use the whole URL given in the assets section to find the picture. Once this was done, the picture was there, even when I wasn’t holding the button down. I knew this meant that I would have to do something to the #button:active section of the CSS tab, but I was still very unclear on what. I decided to hide the image in the HTML section and tried to show it only in the #button.active section, but it seemed like nothing was working. It did some further research of the website that was provided to help with the <img> tag and found something I thought would help, which was using background-image: url(“URL OF IMAGE”) inside the #button:active function. Once I did this, I had successfully put an image into the button when the button was being clicked. Next, when working on speeding up the game, I thought everything was going well since the game was giving the lose game and win game output when appropriate, and stopping when the stop button was pressed, but I the game was continuously speeding up even when the game was over. I realized this was happening because I was only removing seconds from the clueHoldTime variable without restarting in places like stopGame(), loseGame() and winGame(), which would be places where the game cycle would restart. Once the variable was implemented in these three places, the game only sped up during the players game cycle and restarted when a player played a new game!

3. <b>What questions about web development do you have after completing your submission? (recommended 100 - 300 words) </b>
Before completing my submission, I wanted to make sure that the app functioned the way I had intended for it to do. As a result, I ran a lot of trials of the game either by myself or asked those around me to play the game. When doing this, I was wondering if there was a quicker way of running tests like this when building an app and/or a website? Additionally, are the languages used in this assignment (JavaScript, CSS, and HTML) the main languages used in web development? Lastly, would it make you a more competitive candidate to know full-stack, instead of specializing in either back-end or front-end?

4. <b>If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) </b>
If I had a few more hours to work on this project, I would try to spend more time implementing the other optional features, like finishing the timer and making a random secret pattern. Additionally, I would have found a way to scale the pictures I used in the button, to the size of the button. This would have given me more versatility in what pictures I could use since some pictures were too zoomed in to look appealing, because the picture being used was of its original size. Lastly, I would try to find a way to make a player lose a turn or lose the game if they were to guess when the system was still playing the pattern.



## License

    Copyright [Ashani Jewell]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.