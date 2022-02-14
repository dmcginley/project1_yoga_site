# Project one - *Yoga 4 Life*

Site url: <https://dmcginley.github.io/project1_yoga_site>

Repository for the project: <https://github.com/dmcginley/project1_yoga_site>

# Table of contents

  - [Wireframe](#wireframe)
  - [Who is this website for](#who-is-this-website-for)
  - [Design Decisions](#design-decisions)
  - [Typography](#typography)
  - [Color Choices](#color-choices)
  - [Responsiveness](#responsiveness)
  - [Accessibility](#accessibility)
  - [Consistency](#consistency)
  - [Testing](#testing)
    - [Lighthouse in Chrome DevTools.](#lighthouse-in-chrome-devtools)
    - [Validator Testing](#validator-testing)
    - [Manual Testing](#manual-testing)
    - [Responsive Testing](#responsive-testing)
  - [Deployment](#deployment)
  - [Image optimization for the web](#image-optimization-for-the-web)
  - [Resources](#resources)
  - [Credits](#credits)
  - [Content](#content)
    - [Icons](#icons)
    - [Images and Videos](#images-and-videos)

<p>&nbsp;</p>

![Mockup image for the website ](assets/markdown_images/mockup.png "Mockup")

#### *Designed with a 'Mobile First' responsive design.*


## Wireframe
I created the Desktop, Tablet and Mobile wireframe of the Home Page in greyscale, using basic shapes so I could see the hierarchy of the elements on the page. 

*created using Figma prototyping tool.*

![Wireframe created in Figma](assets/markdown_images/wireframe.png "Wireframe")


## Who is this website for
The site is designed for absolute beginners looking to learn yoga starting with a good and simple foundation. People wishing to learn from home using easy techniques that can be done at any part of the day in short bursts.
The website is video heavy for the more visual student, so it can give more of a feel of following along with a teacher.

People with less free time on their hands wishing to get into a healthy lifestyle.

## Design Decisions


As a method of working to keep uniformity across the website, I created three CSS style sheets for easy navigation and changing of elements on in the website. Each style sheets has a table of contents at the top of each page to help navigate through it.

The CSS style sheets are named clearly as:

- style.css
- utilities.css
- hamburger_menu.css


#### Simple, clean design, color, and ease of navigation.

The text, icons, video all have white space around them so as not to detract from each other. The less important content is designed to sit further back by use of tone and color (eg. the card icons are dark grey). While the button or 'Begin Your Yoga Journey' section are bright and with greater contrast.

The 'call to action' button in the Hero section brings you to the video content page, as this is the main goal of the website.

The hamburger_menu is implemented using the help of this [CSS hamburger menu tutorial](#Credits) linked below.

For the navigation the icon & text on the left brings you to the home page. The other two are clearly different in yellow to the right of the nav bar. The page you're on is indacated in white. (when in mobile view this link is hidden as it can not be clicked).

![Navigation bar - nav](assets/markdown_images/nav.png "navbar")

The footer is a simple flexbox container with centred content and a restriction in the icons of *max-width: 700px;* so the icons don't spread too far apart on larger screens.

![Footer and icons inside](assets/markdown_images/footer.png "footer")

#### Card section

The card section is also often the main part of a website as it is the 'bullet-points' for what the visitor will get/learn. In this case learning points to keep in mind while watching and following along with the videos.

<details><summary>Image of card section</summary>

![Card & icon section](assets/markdown_images/card.png "icon cards")

</details>

## Typography
![Typography](assets/markdown_images/type.png "Typography")


- [Cabin](https://fonts.google.com/?query=Cabin) - for the h1, h2 and h3 as a strong, clean, easy to read font.

- [Rubik](https://fonts.google.com/specimen/Rubik?query=Rubik) - for the body, simmiler to Cabin font, modern and clean in style.

- [Libre+Baskerville](https://fonts.google.com/specimen/Libre+Baskerville?query=Libre+Baskerville) - for the quotation on the home page, I chose a more flowery font to look similar to a book type of font, or something in print.

All three fonts together helps continue the clean aesthetic across the site.

## Color Choices

In the end I went for a simple color palette (cutting my colors down by about half), which I found is in keeping with a lot of yoga websites.
The buttons stand out in the hierarchy with stronger colors as do the videos against the off white.

I chose the common red and blue style of button, red usually as a call to immediate action and blue in the form.


![Color sheet](assets/markdown_images/colors.png "Main colors")


#### CSS :root Selector -  *pseudo-class selector*
I used the :root Selector for creating a personalised color set.

eg. The black to be a dark grey, and the white to be a off-white.


![Color code in the utilities.css](assets/markdown_images/color.png ":root Selector color code")



## Responsiveness
I created the website using mobile first and then I have 3 main breakpoints for desktop/tablet (768px, 980px 1440px).
The 1440px large display is so the website doesn't break on large QHD monitors.

The website has a basic Grid across all four pages, with a minmax for the page content. Three elements: the header, main and footer.

![Grid code](assets/markdown_images/base_grid.png "The code for main Grid layout")

The 1fr allows for the white margins on either side to collapse to 0 before the main content starts to shrink, Same for when it grows the main content won't go past 240ch in width.



## Accessibility
- 'alt' text is applied to every image. 
- 'title' on the social icons in the footer, explaining where each link takes you.
- Contrasting colors.
 	* Easy to see buttons and navigation area.
	
		The main (red) button I had to adjust to a darker red because devtools through up an error saying it was too low contrast.
- Background images not to be distracting or masking the text
e.g on mobile version of the site I darkened the background Hero image so as not to detract from the text as it is displayed on the small screen, and could appear more cramped.


## Consistency
- Colors, I reduced the colors used by about half once I settled on a color palette.
- The footer is placed at the bottom of every page.
	* For the shorter pages I used a flex container to push the footer to the bottom.
- The icons all match the same style, from Google and Boxicons, and Bootstrap.
- The fonts match, the header fonts and content (paragraph) fonts.
- The padding is same or smiler for each element across the website, for padding on boxes 2em or 4em.
on text in the smaller numberes eg. 0.4 or 0.6 or 0.8rem.
- Text size in in rem and box/container padding is in em. (there are a few occasions where I went with rem where it better suited the style).

## Testing

### Lighthouse in Chrome DevTools.


Best Practices on the video page was the only one that was low at (92), the issue was "SameSite cookie", this is server-side issue so there was little I could to to fix the issue.
I also reserched this here on [stackoverflow](https://stackoverflow.com/questions/60822936/where-to-add-samesite-none). I also reached out to my tuttores and pears on Slack to conferm the issue.

*Tested in Incognito mode.*

![website in Lighthouse in Chrome ](assets/markdown_images/both_lighthouse.png "Lighthouse score for home page")

After a few errors like images being too big or missing title on social links (facebook, twitter)
I ran Lighthouse a few times to check my code and text.
Tested both mobile and desktop.

When testing in Lighthouse, this is when I desided to have Webp image format as well as Jpg.

### Validator Testing
- HTML
<https://validator.w3.org/>

After a few errors I went back to the code and researched the fixes through a web serch or on Stack overflow to find the solution.

For example I had a problem with the "quote section"  *< picture > < source srcset...* were the error was showing I had to have a "sizes" along with the "source".

For the iframes it suggested that all styling should go in the CSS file, so I fixed that.

On final run the "Document checking completed. No errors or warnings to show" in all the four pages.


- CSS
<https://jigsaw.w3.org/css-validator/>

No Error Found in the three CSS pages.


### Manual Testing
- How I went about it.
I checked each link went to the desired page and that all < a > tags opened in a new tab.
Checked the videos and their refresh times.

The web browsers I used in manual testing are Chrome, Firefox, Microsoft Edge, and Opera.

DOM X-Ray

I used this Chrome extension to check the flow of white space and that the items were centred.

<details><summary>DOM X-Ray in use</summary>

![DOM X-Ray being used on the website ](assets/markdown_images/dom_x_ray.png "DOM X-Ray")

</details>


### Responsive Testing
I used Chrome and Firefox "developer tools, device toggle" to check the responsiveness for each device. From iPhone, roughly 320px, to laptop 1920px, and to the desktop at 2560px (QHD).

Usual errors here were that the image wasn't fully responsive, was a problem with scaling (the image would overflow its container usual arounf 300 or 400px). 

I also used "developer tools" to check the margin and padding on each element to check the style didn't break, especially on smaller devices usually caused by margin or overflow fixed widths to elements on the page. Fixing any sizing errors or overflow of content as I went along.

## Deployment
Deployed using GitHub Pages. <https://github.com/dmcginley/project1_yoga_site/settings/pages>

Once uploaded I checked everything was working ok. I checked response times and refresh time.
Also checking every link and button was working.

## Image optimization for the web

I wanted to make the images responsive while pulling in different resolution images depending on screen size.
Using both Webp and Jpg (as a fall-back).

I used “srcset”, and “sizes” for [Responsive Images](#how-to-use-html5-picture-srcset-and-sizes-for-responsive-images)

The 'quote' picture on the homepage probably took the longest to set up as as it's a constantly responsive image so I had to carefly work out which resolution image to pull in.

![testing for pulling different images](assets/markdown_images/responsive.png "Testing of image resolutions")

I put the width in pixels over each image, so I could clearly see which image was being pulled in during testing.

(For this I used Firefox, as Chrome once a larger images is pulled in it cashes it, and won't revert to the smaller image again).


I learnt How to Use HTML5 “picture”, “srcset”, and “sizes” for Responsive Images


After I edited the images in [Gimp](https://www.gimp.org/), I'd pass the images through Optimizilla or Tinypng and then put them in the image folder. *(Personally I found Optimizilla to be the better of the two websites for keeping a clean image).*

- [Optimizilla](https://imagecompressor.com/)

- [Tinypng](https://tinypng.com/)

Later I also used Imgbot, automated optimizing of my images as they're uploaded to GitHub, *(Free for open source projects).*

- [Imgbot](https://github.com/marketplace/imgbot)

 - [squoosh](https://squoosh.app/) - Used to convert Jpg files to WebP. 

- [favicon.io](https://favicon.io/favicon-converter/) - used for generating the set of images for the tab in the browser.


## Resources
*General reading and resources.*

- The Code Institute course material.

- [w3schools](https://www.w3schools.com/) - to help with links and lists.

- [MDN Web Docs](https://developer.mozilla.org/en-US/) - for looking up flex and grid, scaling images, iframe for video content.

- [*CSS-TRICKS](https://css-tricks.com/) - help with flex, images, background image.

- [Scrimba](https://scrimba.com/) - video tutorials about Flex & Grid.

- [web.dev](https://web.dev/learn/) - the Learn section, for Responsive Design, Media queries.

- [Can I use](https://caniuse.com/) - to check browser support for different elements on the site such as SVG icons, WebP images, srcset.



- [How to Use HTML5 picture srcset and sizes for Responsive Images](https://webdesign.tutsplus.com/tutorials/quick-tip-how-to-use-html5-picture-for-responsive-images--cms-21015?utm_source=pocket_mylist) - srcset and sizes in the picture element.


Book I used for further reading on HTML5 semantic markup.
- [HTML & CSS: Design and Build Websites](https://www.goodreads.com/book/show/10361330-html-and-css) *by Jon Duckett.*

## Credits
*Sites content, media, and help with implementing code for tutorials/on-line help.*

- Help with linear-gradient for the Hero image.

 	
	<https://www.w3schools.com/howto/howto_css_hero_image.asp>


- Use of the < picture >  element and implementing webp.

	<https://web.dev/serve-images-webp/>

	*  further help with < picture >  element and srcset to get two image types at different media query breakpoints.

		<https://www.youtube.com/watch?v=Rik3gHT24AM&t=6s>

- Pushing footer to bottom on thank you page
	
	<https://stackoverflow.com/>

	*The link to the method used.*

	<https://stackoverflow.com/questions/4575826/how-to-push-a-footer-to-the-bottom-of-page-when-content-is-short-or-missing>

- Pure CSS hamburger menu learnt from 'FollowAndrew' on YouTube

 	<https://www.youtube.com/watch?v=sjrp1FEHnyA&t=1707s>


#### Using Flex & Grid.

- Using Flex and Grid elements from Kevin Powell on YouTube

 	<https://www.youtube.com/kepowob>

- Layout of the body divided into a 3 section grid
from Layout Land

	<https://www.youtube.com/channel/UC7TizprGknbDalbHplROtag>


- Aligning Flex items for the Footer **Traversy Media**

	<https://www.youtube.com/watch?v=3YW65K6LcIA>

#### Form
- Code Institute course material. The section for Semantic Form Elements, eg. fieldset, legend.

- < fieldset > - The Field Set element form Mozilla

	<https://developer.mozilla.org/en-US/docs/Web/HTML/Element/fieldset>

	* < fieldset > and < legend >

		Code Institute - Semantic Form Elements.

- Form from w3schools and the book HTML&CSS *by Jon Duckett*

 	<https://www.w3schools.com/howto/howto_css_contact_form.asp>


## Content

The text for the Home page I came up with myself as I used to work in a smiler field of health teaching and training.

The text for the Video page was taken from Wikipedia articles on the [list of asanas](https://en.wikipedia.org/wiki/List_of_asanas).

Yoga on Wikipedia
<https://en.wikipedia.org/wiki/Yoga>

### Icons
- [Material Icons](https://developers.google.com/fonts/docs/material_icons) - The icons in the card section were taken from Google's Material Icons. I downloaded the svg and used inside img tags.


- [Boxicons](https://boxicons.com/) - The icons in the footer were taken from Boxicons. I downloaded the svg code and pasted it in, to try get everything smaller on the site to try and help with loading speeds.

- [Bootstrap Icons](https://icons.getbootstrap.com/) - The star icons on the video page are from Bootstrap, also using the svg code, rather than the images.

### Images and Videos
The images and photos used on the site are from [Pexels.com](https://www.pexels.com/)

 The watermark I created using [Inkscape](https://inkscape.org/) *(vector graphics software).*

<details><summary>Logo created in Inkscape</summary>

![Icon/Watermark created in Inkscape ](assets/markdown_images/inkscape.png "Inkscape")

</details>





