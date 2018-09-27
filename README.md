# GrowWithGoogleScholarship
Learning notes

## Flex
- display: flex;
- flex-wrap: wrap;
- order: 1;

## Patterns
- column drop
- mostly fluid: similar to column drop but add margins when expend over certain width
- layout shifter: box orders can be changed when width changes, extra container may be used
- off canvas: contents are hidden when viewport is small, e.g., the hamburger button; translate & transition

## Responsive table columns for small and large viewports
- hiding table columns using display: none
- no more table for small viewports using display: block
- contained scrolling by put the table in a div and set the width: 100% and overflow-x: auto

## Fonts
- ideal measure (character per line) for web: 65 cpl
- good fonts are at least 16px and 1.2em

## Units, Formats, Environments
- width: 100%vw (set width to 100% of the viewport width)
- height: 100%vh (set height to 100% of the viewport height)
- width: 100%vmin
- height: 100%vmin (set width or height to the miminum of the viewport width and height)
- width: 100%vmax
- height: 100%vmax (set width or height to the maximum)

## Responsive images
- using Grunt
- npm install -g grunt-cli
- brew install imagemagick
- brew install GraphicsMagick
- edit Gruntfile.js
- grunt responsive_images

## Performance
- use icon fonts
- use utf-8 icons instead of png icons

## Full responsiveness
- `srcset` with `x`, reacting to Device Pixel Ratio (DPR)
```HTML
<img src="image_2x.jpg" srcset="image_2x.jpg 2x, image_1x.jpg 1x" alt="a cool image">
```
- `srcset` with `w`, reacting to Image Width
```HTML
<img src="image_200.jpg" srcset="image_200.jpg 200w, image_100.jpg 100w" alt="a cool image">
```

## Accessibility
Web Content Accessibility Guidelines (WCAG)
- Perceivable
- Operable
- Understandable
- Robust

Setup a simple local web server using a [Chrome extension](https://chrome.google.com/webstore/detail/web-server-for-chrome/ofhbbkphhbklhfoeikjpcbhemlocgigb/related?hl=en)
