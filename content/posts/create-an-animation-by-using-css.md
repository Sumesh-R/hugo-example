---
title: "create-an-animation-by-using-css"
date: 2022-01-30T20:12:24+05:30
draft: false
---
# Create an Animation by using CSS


Category: website
Created Time: January 27, 2022 7:27 PM
Current Score: Ok
Finished?: No
Up Online?: No
author: virkam
topics: Anime effects

# Table of Contents

# Name: Anime Effects by HTML and CSS


# Links:

# Notes:

## Create a basic HTML page:

At the first ,you want to create a “div” in a body section at the same time create the “class” as ‘header’.In that  you want to create similar “div” with different “class’s” for the HTML page.

At first ,we need to create a “div” in the body section with `class`  named `header`. And then we need to create mutltiple `classes` as shown below

**To achieve this, you can use the similar tags as “div” and “class”**

```html
<body>
    <div class="header">
      <div class="inner_box incircle"></div>
      <div class="inner_box outcircle"></div>
      <div class="inner_box one"></div>
      <div class="inner_box two"></div>
      <div class="inner_box three"></div>
      <div class="inner_box four"></div>
      <div class="inner_box five"></div>
      <div class="inner_box six"></div>
    </div>
  </body>
```

## **Create a “body”  and “header” section by using css:**

In the body section just use the “background-image” as “radial-gradient” and use the similar contents as follows:

```css
body {
  background-image: radial-gradient(
    circle farthest-corner at center,
    #c0faf5 20%,
    #7affc1 80%
  );
}
```

In the header section use the “position” as ‘absolute’ and mention the pixels of “width , height , border-radius and perspective” and also the important thing to mention is “ top and left “ measurement by calculating the values as follows:

```css
.header {
  position: absolute;
  top: calc(50% - 180px);
  left: calc(50% - 180px);
  width: 400px;
  height: 400px;
  border-radius: 50%;
  perspective: 800px;
}
```

## To create an inner-box by CSS:

For creating an inner-box the main thing to include is “ position as absolute , box- sizing as border-box and also include the width , height , border-radius “.

```css
.inner_box {
  position: absolute;
  box-sizing: border-box;
  width: 100%;
  height: 100%;
  border-radius: 50%;
}
```

## Create an inner box .incircle and .out circle:

For incircle we can use left and top as “0%” and and border-bottom as follows:

```css
.inner_box.incircle {
  left: 0%;
  top: 0%;
  border-bottom: 5px solid #000000;
}
```

For outcircle we can use right and bottom as “0%” and and border-bottom as follows:

```css
.inner_box.outcircle {
  right: 0%;
  bottom: 0%;
  border-top: 5px solid #000000;
}
```

## To create an inner_box.___ by using CSS:

To create an inner_box.one , inner_box.two etc.., for that we can include the specifications like “ left , right , top , bottom and also border-top , border-bottom , border-left , border-right and finally animation “ as follows: 

```css
.inner_box.one {
  left: 0%;
  top: 0%;
  animation: rotate-outcircle 1s linear infinite;
  border-bottom: 13px solid #000000;
}

.inner_box.two {
  right: 0%;
  top: 0%;
  animation: rotate-two 1s linear infinite;
  border-right: 13px solid #0011ff;
}

.inner_box.three {
  right: 0%;
  bottom: 0%;
  animation: rotate-three 1s linear infinite;
  border-top: 13px solid #ff0000;
}

.inner_box.four {
  left: 0%;
  bottom: 0%;
  animation: rotate-four 1s linear infinite;
  border-right: 13px solid #8f009c;
}

.inner_box.five {
  left: 0%;
  right: 0%;
  animation: rotate-five 1s linear infinite;
  border-top: 13px solid #37ac01;
}

.inner_box.six {
  bottom: 0%;
  right: 0%;
  animation: rotate-six 1s linear infinite;
  border-left: 13px solid #888016;
}
```

## Keyframe content creation:

At the final , we want to create the @keyframe  content for the “ rotate-one , rotate-two etc ..,”.In that we want to include 0% and 100% and include “transform” specification and that rotate X  , rotate Y , rotate Z and mention the degree for each of the rotation .

```css
@keyframes rotate-one {
  0% {
    transform: rotateX(350deg) rotateY(450deg) rotateZ(0deg);
  }
  100% {
    transform: rotateX(35deg) rotateY(45deg) rotateZ(360deg);
  }
}

@keyframes rotate-two {
  0% {
    transform: rotateX(500deg) rotateY(150deg) rotateZ(0deg);
  }
  100% {
    transform: rotateX(50deg) rotateY(15deg) rotateZ(360deg);
  }
}

@keyframes rotate-three {
  0% {
    transform: rotateX(350deg) rotateY(550deg) rotateZ(0deg);
  }
  100% {
    transform: rotateX(35deg) rotateY(55deg) rotateZ(360deg);
  }
}

@keyframes rotate-four {
  0% {
    transform: rotateX(500deg) rotateY(-550deg) rotateZ(0deg);
  }
  100% {
    transform: rotateX(50deg) rotateY(-55deg) rotateZ(360deg);
  }
}

@keyframes rotate-five {
  0% {
    transform: rotateX(400deg) rotateY(-150deg) rotateZ(0deg);
  }
  100% {
    transform: rotateX(40deg) rotateY(-15deg) rotateZ(360deg);
  }
}

@keyframes rotate-six {
  0% {
    transform: rotateX(350deg) rotateY(-450deg) rotateZ(0deg);
  }
  100% {
    transform: rotateX(35deg) rotateY(-45deg) rotateZ(360deg);
  }
}
```

# Summary:

In this topic we can learn the basic anime effect by using basic HTML and CSS .And we use the only simple tags in HTML and  simple specifications in CSS .