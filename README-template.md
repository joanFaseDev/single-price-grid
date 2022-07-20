# Frontend Mentor - Single price grid component solution

This is a solution to the [Single price grid component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/single-price-grid-component-5ce41129d0ff452fec5abbbc). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the component depending on their device's screen size
- See a hover state on desktop for the Sign Up call-to-action

### Screenshot

![](./screenshot.jpg)

Add a screenshot of your solution. The easiest way to do this is to use Firefox to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

Alternatively, you can use a tool like [FireShot](https://getfireshot.com/) to take the screenshot. FireShot has a free option, so you don't need to purchase it. 

Then crop/optimize/edit your image however you like, add it to your project, and update the file path in the image above.

**Note: Delete this note and the paragraphs above when you add your screenshot. If you prefer not to add a screenshot, feel free to remove this entire section.**

### Links

- Solution URL: [Project on GitHub](https://github.com/joanFaseDev/single-price-grid)
- Live Site URL: [Projet hosted through Vercel](https://single-price-grid-two-alpha.vercel.app/)

## My process

### Intro & Context

First and foremost, know that english isn't my first language and that, even if i do try to make myself clear, there's time when i do grammatical errors and mispellings. My apologies if that happen.

This is my third Frontend Mentor's project and i wanted to try something a little different this time which is writing this README file while working on the project. The reason is i usually write this down once the project is finished and, by then, i always have difficulties to remember what i done, how and why. Plus i'm pretty slow and when i'm finished i usually am tired which makes the writing not very enjoyable to me. So this time, i'm planning, writing what i plan, execute then do it over. It's feels way more natural to me because 1) it makes the writing an actual part of the project instead of something that come after it's done and 2) writing about the project while working on it helps clarify your thought and your vision for the project which makes the building way easier to manage. Well, that the theory, time to test it!

### Analysing the project

Building a responsive card which can be displayed through two different designs, a mobile and a desktop one. What's important here in my opinion is that the mobile design and the desktop design have similarities  in their layout. Both have three main parts which can be named 'community', 'subscription' and 'about'. The interesting thing that makes that project way more easier to tackle is that the layout inside this three main parts is practically identical for the two design. Sure the way the three parts are positionned relative to one another change between the mobile and the desktop design but the inside of these parts is commun to both designs. It's important to me because it means that once i have one of the design figured out, i can use most of my code for the other without altering much at all.

### Planning 

I will to do this project using CSS Grid because i feel it's a really powerful and flexible tool to build all kinds of layout. Also, a couple of hours sooner, i watched part of  a Grid Crash Course made by youtube's channel [Traversy Media](https://www.youtube.com/watch?v=0xMQfnTU6oo) and felt like doing a project to test what i just learned.

 I'm gonna start with the mobile design because as an aspiring front-end developper it seems more manageable to me (there's usually less space to handle for a mobile design which means less chance to screw up). Plus that's what i'm used to. I'll need a container to transform into a grid and here i'm gonna use a main html element to do the job. On my last projects, i was made aware by helpful people of accessibility, landmarks and semantic tags so from now on i'm gonna try to work on it.  

The container is going to be divided in three rows (one for each part) and one column. That way, when switching to the desktop design, i'll change the container layout through media queries into something like two rows and two columns. I'll probably use the *grid-template-areas* property which i find really cool even if managing rows and columns through *grid-row* and *grid-column* is probably more efficient.

The padding between the different elements inside the three parts of the card doesn't seem to change much so i'm gonna spend extra time on the mobile design to be sure that everything looks nice. That way i won't have to change much when doing the desktop design.

I estimated the container for the mobile design to be something like 300-350 pixels but i'm gonna try using percentages here because i want to get a feel for relative units (as they are more used that absolute ones, at least that's my understanding). 90% for the mobile design to 50% for the desktop one. That's the idea.



### Built with

- Semantic HTML5 markup
- CSS 
- CSS Grid

### What I learned

* I used this project to get confortable with semantic tags. Accessibility seems to be mandatory nowadays so i think aspiring developper should get to work with it from the get-go. I wanted to use *article* elements inside the *main* tag but it's used for autonomous content and i didn't feel like it was the case here so i ended up making three *section* elements which seemed better than general container like *div*. I also provided *aria-labelledby* attribute to all section's header  and *aria-label* to the button's one but i'm not quite sure i did it the right way so i'll try to ask when putting the project live.

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

To see how you can add code snippets, see below:

```html
<h1>Some HTML code I'm proud of</h1>
```
```css
.proud-of-this-css {
  color: papayawhip;
}
```
```js
const proudOfThisFunc = () => {
  console.log('🎉')
}
```

If you want more help with writing markdown, we'd recommend checking out [The Markdown Guide](https://www.markdownguide.org/) to learn more.

**Note: Delete this note and the content within this section and replace with your own learnings.**

### Continued development

Use this section to outline areas that you want to continue focusing on in future projects. These could be concepts you're still not completely comfortable with or techniques you found useful that you want to refine and perfect.

**Note: Delete this note and the content within this section and replace with your own plans for continued development.**

### Useful resources

* [MDN Article on Aria roles](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles)



## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**

## Acknowledgments

This is where you can give a hat tip to anyone who helped you out on this project. Perhaps you worked in a team or got some inspiration from someone else's solution. This is the perfect place to give them some credit.

**Note: Delete this note and edit this section's content as necessary. If you completed this challenge by yourself, feel free to delete this section entirely.**
