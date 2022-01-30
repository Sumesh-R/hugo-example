---
title: "next-level-animation-by-using-html-and-css"
date: 2022-01-30T20:12:24+05:30
draft: false
---
# Next Level Animation by using HTML and CSS

Category: website
Created Time: January 29, 2022 9:00 PM
Current Score: Ok
Finished?: No
Up Online?: No
author: virkam
topics: Anime effects

# Table of Contents

# Name: Next Level animation by using HTML and CSS.

![post_3.png](Next%20Level%20Animation%20by%20using%20HTML%20and%20CSS%20514833c9042c41639a9ee8034a513226/post_3.png)

# Links:

# Notes:

## Create an HTML page:

In this HTML page at body section “div” section can be created and inside that “class” also we should create as “header” and also “style” . And also inside that another “div” section and also ”class” should be created as “main” .

Again inside that another “div” section and for that “div” another “class” . And finally another “div” section this is the important section because the main content should be added here . 

For this section “class” should be created . Inside that a new tag we want to create i.e.., “span” inside that “class” also want to create for the index count 0 to 6 mentioned as follows., 

**To achieve this, you can use the similar tags as “div” , “class” and “span”.**

```html
<body>
    <div class="header" style="--hue: 260; --saturation: 82; --lightness: 73">
      <div class="main">
        <div class="header_words" style="--index: 0">
          <div class="words" enterd_word="L">
            <span class="entered_letters" aria-hidden="true">l</span>
            <span class="entered_letters" aria-hidden="true">l</span>
            <span class="entered_letters" aria-hidden="true">l</span>
            <span class="entered_letters" aria-hidden="true">l</span>
            <span class="entered_letters"></span>
          </div>
        </div>
        <div class="header_words" style="--index: 1">
          <div class="words" enterd_word="o">
            <span class="entered_letters" aria-hidden="true">o</span>
            <span class="entered_letters" aria-hidden="true">o</span>
            <span class="entered_letters" aria-hidden="true">o</span>
            <span class="entered_letters" aria-hidden="true">o</span>
            <span class="entered_letters"></span>
          </div>
        </div>
        <div class="header_words" style="--index: 2">
          <div class="words" enterd_word="a">
            <span class="entered_letters" aria-hidden="true">a</span>
            <span class="entered_letters" aria-hidden="true">a</span>
            <span class="entered_letters" aria-hidden="true">a</span>
            <span class="entered_letters" aria-hidden="true">a</span>
            <span class="entered_letters"></span>
          </div>
        </div>
        <div class="header_words" style="--index: 3">
          <div class="words" enterd_word="d">
            <span class="entered_letters" aria-hidden="true">d</span>
            <span class="entered_letters" aria-hidden="true">d</span>
            <span class="entered_letters" aria-hidden="true">d</span>
            <span class="entered_letters" aria-hidden="true">d</span>
            <span class="entered_letters"></span>
          </div>
        </div>
        <div class="header_words" style="--index: 4">
          <div class="words" enterd_word="i">
            <span class="entered_letters" aria-hidden="true">i</span>
            <span class="entered_letters" aria-hidden="true">i</span>
            <span class="entered_letters" aria-hidden="true">i</span>
            <span class="entered_letters" aria-hidden="true">i</span>
            <span class="entered_letters"></span>
          </div>
        </div>
        <div class="header_words" style="--index: 5">
          <div class="words" enterd_word="n">
            <span class="entered_letters" aria-hidden="true">n</span>
            <span class="entered_letters" aria-hidden="true">n</span>
            <span class="entered_letters" aria-hidden="true">n</span>
            <span class="entered_letters" aria-hidden="true">n</span>
            <span class="entered_letters"></span>
          </div>
        </div>
        <div class="header_words" style="--index: 6">
          <div class="words" enterd_word="g">
            <span class="entered_letters" aria-hidden="true">g</span>
            <span class="entered_letters" aria-hidden="true">g</span>
            <span class="entered_letters" aria-hidden="true">g</span>
            <span class="entered_letters" aria-hidden="true">g</span>
            <span class="entered_letters"></span>
          </div>
        </div>
      </div>
    </div>
  </body>
```

## Create an normal CSS page :

For that as usual  “*” box-sizing and transition should be added and root section and media section should be added as follows:  

```css
* {
  box-sizing: border-box;
  transition: all 0.15s ease 0s;
}
:root {
  --movement: 0.85;
  --stop: 0.5;
  --duration: calc((var(--movement) * (1 / var(--stop))));
  --stagger: 0.1125;
  --perspective: 500;
  --size: 50;
  --ease: cubic-bezier(1, -0.52, 0.53, 0.2);
  --bg: #00ffeaad;
  --panel: rgb(99, 6, 6);
  --color: #d0ff00;
  --hue: 23;
  --saturation: 100;
  --lightness: 55;
}
@media (prefers-color-scheme: dark) {
  :root {
    --bg: #34cec1ad;
    --panel: rgb(99, 6, 6);
    --color: #d0ff00;
  }
}
```

## To create an body section :

In that body section the important thing we should be added i.e.., “ align-items , background , display , justify-content , min-height and overflow as follows:

```css
body {
  align-items: center;
  background: var(--bg);
  display: flex;
  justify-content: center;
  min-height: 100vh;
  overflow: hidden;
}
```

## Crete an header section and main section :

For “header” we should only calculate the “perspective” section . In the main section as usual we should create “ display , transform and transform-style “ condition as follows:

```css
.header {
  perspective: calc(var(--perspective) * 1px);
}
.main {
  display: flex;
  transform: translate(calc(var(--size) * 0.7px), 0) rotate(0deg);
  transform-style: preserve-3d;
```

For the 3D effects with different angles we can change the rotating degree for the angle X , Y and Z as follows:

```css
.main {
  display: flex;
  transform: translate(calc(var(--size) * 0.7px), 0) rotateX(-50deg)
    rotateY(50deg) rotateZ(30deg);
  transform-style: preserve-3d;
```

## To create a header-words and words section :

In header words the special conditions can be applied i.e.., “ webkit-animation , animation , transform-origin and transform-style “ created as follows: 

```css
.header_words {
  -webkit-animation: jump calc(var(--duration) * 1s)
    calc((var(--stagger, 0) * var(--index, 0)) * 1s) var(--ease) infinite;
  animation: jump calc(var(--duration) * 1s)
    calc((var(--stagger, 0) * var(--index, 0)) * 1s) var(--ease) infinite;
  transform-origin: bottom center;
  transform-style: preserve-3d;
}
.header_words .words {
  -webkit-animation: rotate calc(var(--duration) * 4s)
    calc((var(--stagger, 0) * var(--index, 0)) * 1s) ease infinite;
  animation: rotate calc(var(--duration) * 4s)
    calc((var(--stagger, 0) * var(--index, 0)) * 1s) ease infinite;
```

In words section as usual condition should be followed , and the main thing is we want to calculate the height , width and margin-right and for our convenience we can also add the new font family created as follows:  

```css
.words {
  color: var(--color);
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
    Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
  font-size: 2rem;
  font-weight: bold;
  height: calc(var(--size) * 1px);
  margin-right: calc(var(--size) * 0.2px);
  position: relative;
  text-transform: uppercase;
  transform-style: preserve-3d;
  width: calc(var(--size) * 1px);
```

## Create an main part of the animation i.e.., entered-letters :

In the section entered-letters as usual normal thing should be created as followed as before we should calculate the height , width and border for the various sizes for our convenience and the as usual thing should be added as follows :

 

```css
.entered_letters {
  align-items: center;
  background: var(--panel);
  border: 5px
    hsl(var(--hue), calc(var(--saturation) * 1%), calc(var(--lightness) * 1%))
    solid;
  display: flex;
  height: calc(var(--size) * 1px);
  justify-content: center;
  left: 50%;
  position: absolute;
  top: 50%;
  width: calc(var(--size) * 1px);
}
```

In the entered-letters the fore most important thing we should add for the 3D effects , so we can separate that into 5-type and each of that we want to create “transform” condition , in that we want to add translate 3D and also mention the rotating direction and calculate the translate-3D condition as follows :

```css
.entered_letters:nth-of-type(1) {
  transform: translate3d(-50%, -50%, 0)
    translate3d(0, 0, calc(var(--size) * 0.5px));
}
.entered_letters:nth-of-type(2) {
  transform: translate3d(-50%, -50%, 0) rotateX(90deg)
    translate3d(0, 0, calc(var(--size) * 0.5px));
}
.entered_letters:nth-of-type(3) {
  transform: translate3d(-50%, -50%, 0) rotateX(180deg)
    translate3d(0, 0, calc(var(--size) * 0.5px));
}
.entered_letters:nth-of-type(4) {
  transform: translate3d(-50%, -50%, 0) rotateX(-90deg)
    translate3d(0, 0, calc(var(--size) * 0.5px));
}
.entered_letters:nth-of-type(5) {
  transform: translate3d(-50%, -50%, 0) rotateY(-90deg)
    translate3d(0, 0, calc(var(--size) * 0.5px));
```

## Create an webkit-keyframes for the rotate and jump condition :

In that @-wekit-keyframes for rotate and jump the common thing is transform condition and the main difference is  “rotation degree “ for the “rotate” and “ scale condition and translate” condition for “jump” as follows:

  

```css
@-webkit-keyframes rotate {
  0%,
  30.625% {
    transform: rotateX(0deg);
  }
  33.125%,
  81.625% {
    transform: rotateX(90deg);
  }
  83.125%,
  100% {
    transform: rotateX(180deg);
  }
}

@-webkit-keyframes rotate {
  0%,
  30.625% {
    transform: rotateX(0deg);
  }
  33.125%,
  81.625% {
    transform: rotateX(90deg);
  }
  83.125%,
  100% {
    transform: rotateX(180deg);
  }
}
```

## Final part of the code , create keyframes for rotate and jump :

In that @keyframes as usual followed in the before condition for rotate and jump the common thing is transform condition and the main difference is  “rotation degree “ for the “rotate” and “ scale condition and translate” condition for “jump” as follows:

```css
@keyframes rotate {
  0%,
  30.625% {
    transform: rotateX(0deg);
  }
  33.125%,
  81.625% {
    transform: rotateX(90deg);
  }
  83.125%,
  100% {
    transform: rotateX(180deg);
  }
}

@keyframes jump {
  0%,
  50%,
  100% {
    transform: scaleX(1) scaleY(1) translate(0, 0);
  }
  15% {
    transform: scaleX(1.2) scaleY(0.8) translate(0, 0);
  }
  25% {
    transform: scaleX(0.9) scaleY(1.1) translate(0, -100%);
  }
}
```

# Summary:

In this we have learnt about the the next level animation by using HTML an CSS . So it may be easy for creating the animation for the 3D effects and also by using different angles .