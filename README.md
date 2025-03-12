# Simple JavaScript Slider

A lightweight and customizable image slider built with vanilla JavaScript, HTML, and CSS.

## Demo

![Slider Preview](assets/images/1.jpg)  
*(Replace with an actual GIF or screenshot of your slider in action.)*

## Features

✅ Image sliding with navigation buttons  
✅ Keyboard arrow navigation  
✅ Swipe support for mobile devices  
✅ Auto-play functionality  
✅ Customizable styles and settings  

## Installation

1. Clone this repository:
   ```sh
   git clone https://github.com/yourusername/your-slider-repo.git

    Navigate to the project folder:

    cd your-slider-repo

    Open index.html in a browser.

Usage

The slider is instantiated in main.js. By default, it creates two sliders with different settings:

import {Slider} from "./Slider.js";

const slider = new Slider({
    barsColor: "dimgrey" // Default slider with minimal customization
});

const sliderDuplicate = new Slider({
    sliderID:   "dupl_slider",
    slideTime: 4,  // Each slide lasts 4 seconds
    imageLinks: [
        "assets/images_add/1.jpg",
        "assets/images_add/2.jpg",
        "assets/images_add/3.jpg",
        "assets/images_add/4.jpg",
        "assets/images_add/5.jpg",
        "assets/images_add/6.jpg"
    ],
    barsColor: "red",
    barsHoverColor: "orange"
});

Customization

You can customize the slider by passing an object with the following properties:
Property	Type	Default Value	Description
sliderID	String	"orig_slider"	The ID of the container element
slideTime	Number	1 (second)	Time per slide in autoplay mode
imageLinks	Array	["assets/images/1.jpg", "assets/images/2.jpg", ...]	List of image URLs
barsColor	String	"dimgrey"	Background color of navigation bars
barsHoverColor	String	"lightgrey"	Hover color of navigation bars
Controls
Action	Control Method
Next slide	Click → button, right arrow key, or swipe left
Previous slide	Click ← button, left arrow key, or swipe right
Auto-play Start/Stop	Click the play/pause button
Direct image selection	Click on the navigation bullets
File Structure

📂 your-slider-repo
 ├── 📂 assets
 │   ├── 📂 images
 │   ├── 📂 images_add
 │   ├── 📂 styles
 │   │   ├── normalize.css
 │   │   ├── style.css
 ├── index.html
 ├── Slider.js
 ├── main.js
 ├── README.md
