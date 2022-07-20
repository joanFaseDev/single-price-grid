# Frontend Mentor - Single price grid component solution

This is a solution to the [Single price grid component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/single-price-grid-component-5ce41129d0ff452fec5abbbc). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Intro & Context](#intro--context)
  - [Analysing the project](#analysing-the-project)
  - [Planning](#planning)
  - [Review](#review)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
-

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the component depending on their device's screen size
- See a hover state on desktop for the Sign Up call-to-action

### Screenshot

![](C:\Users\joanf\Desktop\CSS\FrontEndMentor\SinglePriceGridComponent\singlePrice_mobile.png)

![](C:\Users\joanf\Desktop\CSS\FrontEndMentor\SinglePriceGridComponent\singlePrice_desktop.png)

### Links

- Solution URL: [Project on GitHub](https://github.com/joanFaseDev/single-price-grid)
- Live Site URL: [Projet hosted through Vercel](https://single-price-grid-two-alpha.vercel.app/)

## My process

### Intro & Context

First and foremost, you know that english isn't my first language and that, even if i do try to make myself clear, there's time when i do grammatical errors and mispellings. My apologies if that happen.

This is my third Frontend Mentor's project and i wanted to try something a little different this time which is writing this README file while working on the project. The reason is i usually write this down once the project is finished and, by then, i always have difficulties to remember what i done, how and why. Plus i'm pretty slow and when i'm finished i usually am tired which makes the writing not very enjoyable to me. So this time, i'm planning, writing what i plan, execute then do it over. It feels way more natural to me because 1) it makes the writing an actual part of the project instead of something that come after it's done and 2) writing about the project while working on it helps clarify your thought and your vision for the project which makes the building way easier to manage. Well, that the theory, time to test it!

### Analysing the project

The project is about building a responsive card which can be displayed through two different designs, a mobile and a desktop one. What's important here in my opinion is that the mobile design and the desktop design have similarities in their layout. Both have three main parts which can be named 'community', 'subscription' and 'about'. The interesting thing that makes that project way more easier to tackle is that the layout inside this three main parts is practically identical for the two designs. Sure the way the three parts are positionned relative to one another change between the mobile and the desktop design but the inside of these parts is nearly identical in both designs. It's important to me because it means that once i have one of the design figured out, i can use most of my code for the other without altering much of it.

### Planning

I will to do this project using CSS Grid because i feel it's a really powerful and flexible tool to build all kinds of layout. Also, a couple of hours sooner, i watched part of a Grid Crash Course made by youtube's channel [Traversy Media](https://www.youtube.com/watch?v=0xMQfnTU6oo) and felt like doing a project to test what i just learned.

I'm gonna start with the mobile design because as an aspiring front-end developper it seems more manageable to me (there's usually less space to handle in a mobile design which means less chance to screw up). Plus that's what i'm used to. I'll need a container to transform into a grid and here i'm gonna use a main html element to do the job. On my last projects, i was made aware by helpful people of accessibility, landmarks and semantic tags so from now on i'm gonna try to work on it.

The container is going to be divided in three rows (one for each part) and one column. That way, when switching to the desktop design, i'll change the container layout through media queries into something like two rows and two columns. I'll probably use the _grid-template-areas_ property which i find really cool even if managing rows and columns through _grid-row_ and _grid-column_ is probably more efficient.

The padding between the different elements inside the three parts of the card doesn't seem to change much so i'm gonna spend extra time on the mobile design to be sure that everything looks nice. That way i won't have to change much when doing the desktop design.

I estimated the container for the mobile design to be something like 300-350 pixels (double that for desktop design) but i'm gonna try using percentages here because i want to get a feel for relative units (as they are more used that absolute ones, at least that's my understanding). 90% for the mobile design to 50% for the desktop one. That's the idea. I'll also used the max-width property in a media query targeting the desktop design to make sure that the container stop growing past a certain point (in case the user have a very large screen).

### Review

For the most part, i followed and executed what was planned. I couldn't totally replicate some paddings/margins and i think the reason is i exclusively used rem units. Em units would probably have been better because the font's dimensions and margins could have scaled on desktop design but i find these units incredibly hard to use and i don't have enough pratice to use them on a gut feeling. That's the reason i like rem better, it's a relative unit but also very constant.

Overall, i think i did ok. The result could have been better but i'm happy about the process. The whole planning/writing/executing plan feels way more natural than the way i did projects before so i think i'll stick with it and try to improve what i can.

### Built with

- Semantic HTML5 markup
- CSS
- CSS Grid

### What I learned

- I used this project to get confortable with semantic tags. Accessibility seems to be mandatory nowadays so i think aspiring developper should get to work with it from the get-go. I wanted to use _article_ elements inside the _main_ tag but it's used for autonomous content and i didn't feel like it was the case here so i ended up making three _section_ elements which seemed better than general container like _div_. I also provided _aria-labelledby_ attribute to all section's header and _aria-label_ to the button's one but i'm not quite sure i did it the right way so i'll try to ask when putting the project live.
- I also tried to apply some naming convention to my css classes. I read some articles about BEM and other methods to better organize our code as developpers and i thought it seems really useful. Sure BEM is for way larger projects than that but i suck at naming and i always have troubles navigating my files so i want at least some methodology to save some time or, at least, to not lose too much.
- I discovered that the inspector from Firefox/Chrome browser had a color picker! And it was really useful on that project because it helped me better understand what property i needed to change to obtain a render pretty close from the template.

### Continued development

I wish to keep using the css grid model for the next projects. I feel like the tool is really powerful and learning how to use it properly could potentially helps a lot in the future.

I also want to dig deeper in accessibility stuff (aria attributes, semantic tags, etc, ...) because that matters a lot in modern front-end development and i think that using these tools should become natural for us.

Finally i think i'm going to learn how to use css variables. Preprocessor's stuff way too early for me (plus i don't feel like i need them for small project like this) but reusing simple bits of code seems like something that would help me a lot. Plus variables bring clarity, it's always simpler to use a color with a name instead of an hsl code i'm unable to remember for more than 1 minute...

### Useful resources

- [MDN Article on Aria roles](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles)

## Author

- Website - [GitPage hosting all my projects from Frontend Mentor](https://joanfasedev.github.io/FrontEnd-mentor-projects/)
- Frontend Mentor - [@joanFaseDev](https://www.frontendmentor.io/profile/joanFaseDev)
