# Sass Machine: Part 2

#### A second, independent Sass project using an alternate wireframe as a starting point, December 8, 2017

#### By **Luke Bertram**

## Description

This is a second (and solo) attempt at creating a landing page for a website about the inevitable doom of our land at the hands of an ancient malevolent force that humanity cannot hope to comprehend or appease. This version will be built from an alternate wireframe that was established on the first day of a two-day in-class project in Epicodus' CSS course.

## Setup/Installation Requirements

For greatest ease of use, simply visit [this website](http://lukebertram.github.io/sass-machine2) in your web browser of choice. However, if you're feeling frisky, you can also use the following steps to clone the project from [GitHub](http://github.com) and run it locally on your own computer:

 * Visit the github page for [this project](http://github.com/lukebertram/sass-machine2)
 * Click the "Clone or Download" button and copy the address found there. Alternatively, just copy this address to your clipboard: https://github.com/lukebertram/sass-machine2.git
 * Access your system's command line interface (_ie Terminal, for MacOS Users_) and navigate to your home directory by entering the following magical spell into your command line (note: do not enter the '$' character):
 >$cd ~

 * Next, cast the following, more advanced spell:  
 >$git clone https://github.com/lukebertram/sass-machine2.git

 * Finally, open the project in your system's default web browser with the following final incantation:
 >$open sass-machine2/index.html


## Known Bugs


## Support and Contact Details

Flag me down in class, or send me a tweetbook on facestagram if you have any troubles.

## Two-Day Project Thoughts and Feedback

The 2-day version of this project was confusing and difficult primarily due to our conflation of the terms "wire-framing" and "templating." Whereas wire-framing first can be a relatively quick and intuitive process, templating first would seem to encourage us to jump into coding the layout of the page before having established a layout to follow - which I now know was the opposite of what was intended by the lesson.

It also seemed difficult to me to draw a clear line between the non-coding and coding phases of laying out the page at the time of the project. It's easy enough to draw out a wireframe of what we'd like the page to look like once completed. However, it felt difficult to propose methods of attaining those visual goals without trying them out in code. I realize now, after our standup discussions, that this was exactly the point of the exercise - to teach us to consider the problems and potential solutions before jumping into coding something that was way off-base.

Throughout the process, I found myself wishing I had more concrete examples of everything we were trying to do: how someone had written a mixin that was actually useful, what a good wireframe would look like, or just a fully realized sass project with good organization of custom and/or vendor components that I could use as a reference or model to layout my own project. I ended up debating with my pair on several occasions the merits of various ways of splitting our Sass into different files.

Once we got to day 2 of the project, I felt that things started to go much more smoothly. Perhaps I was just less uneasy once we were able to start implementing our proposed solutions to our various layout problems. That said, I wish we'd had more time to do the actual work of building the Sass. While my pair and I were making good progress, by the end of the day we were still a ways off from achieving even the basic layout laid forth in our wireframe.

If we could do this project again I feel it would go more smoothly now that I have some idea of what to expect from the whole process. I feel confident that I could more effectively break down design goals and competently research possible methods of achieving them before even beginning to code. But I'm not sure if there's room in the course's schedule for us to do this all again.
#### Changes in Approach for Independent Project
_how you will change your approach today. Of course you won't be pairing, so working alone is a given. Beyond that, did you learn something about a specific tool that will change your approach today? Did you learn something from your pair's process and workflow that will inform your work? How about the way you segment your work, apply styles, and commit?_

Yesterday, my pair and I decided to work in parallel to help brush up on our group git workflow. While we did encounter some unexpected problems (using Sass requires additional files/directories to be ignored to prevent painful merge processes) the idea of branching to implement each new component/layout element seems like a good model to follow for future group projects. I would like to try to do this even when working on my own just to get more accustomed to it.

Additionally, when writing our index.html file, my pair utilized semantic divisions in laying out the webpage and informed me that they are a useful convention in making a webpage more accessible to screen-readers and the like. I would like to adopt this practice myself, as even setting aside accessibility issues, it feels like a simple way to write slightly more descriptive and readable code.

## Technologies Used

Most notably, these projects focused on utilizing the unique functionalities of SASS to more efficiently generate the final CSS stylesheet for the webpage. Below is a list of Sass features and how they were implemented in the original 2-day project:

| Sass Element | Implementation |
|:------------:|:---------------|
| Nesting | This feature was used all over the place to style both parent elements and their children in an easy to read way. Nesting seems to be one of the most intuitive and useful parts of Sass. |
| Mixins  | Among others, we created a mixin for absolutely positioning child elements within a parent, as well as mixins for tablet and desktop media queries. |
| Variables | We used variables all over the place. Any time the value of some styling property might appear arbitrary to someone new to the code or seemed likely to change over the lifetime of the page, we replaced it with a descriptive variable name and defined that variable in a dedicated sass file within the abstracts directory. Some specific uses of variables included defining repeated colors, background images, and height/width of various layout elements. |
| Extends | These were used to keep padding and margin values consistent across various layout elements.|
| Imports/7-1 File Structure | This folder structure was used to separate Sass elements into distinct files/functionalities and organize them to make them easier to locate. When compiled, all necessary files were imported into main.scss before being processed into a single CSS file. |

### License

MIT License

Copyright (c) 2017 **Luke Bertram**
