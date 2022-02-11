# Project one - *Yoga 4 Life*

Site url: <https://dmcginley.github.io/project1_yoga_site/>

Repository for the project: <https://github.com/dmcginley/project1_yoga_site>

## Table of contents

  - [Wireframe](#wireframe)
  - [Style Guide](#style-guide)
  - [References Section](#references-section)
  - [Testing](#testing)
	- [Validator Testing](#Validator-Testing)
	- [Manual Testing](#Manual-Testing)
	- [Responsive Testing](#Responsive-Testing)
- [Deployment](#deployment)
- [Credits](#credits)




![Mockup image for the website ](assets/markdown_images/mockup.png "Mockup")

### Designed with a 'Mobile First' responsive design.


## Wireframe
I created the Desktop, Tablet and Mobile wireframe of the Home Page in greyscale so I could see the hierarchy of the elements on the page. 

*Using basic shapes, created using Figma prototyping tool.*

![Wireframe created in Figma](assets/markdown_images/wireframe.png "Wireframe")


## Who is this website for
The site is designed for absolute beginners looking to learn yoga starting with a good and simple foundation. People wishing to learn from home using easy techniques that can be done at any part of the day in short bursts.
The website is video heavy for the more visual student, so it can give more of a feel of following along with a teacher.

People with less free time on their hands wishing to get into a healthy lifestyle.

### Design Decisions
- Simple design choice.

	I created three CSS style sheets for easy navigation and changing of elements on in the website. Each style sheets has a table of contents at the top of each page to help navigate through it.

	The CSS style sheets are named clearly as:

	- style.css
	- utilities.css
	- hamburger_menu.css


- Clean design, color, and ease of navigation.

	The text, icons, video all have white space around them so as not to detract from each other. The less important content is designed to sit further back by use of tone and color (eg. the card icons are dark grey). While the button or 'Begin Your Yoga Journey' section are bright and with greater contrast.

	The 'call to action' button in the Hero section brings you to the video content page, as this is the main goal of the website.

	The hamburger_menu is implemented using the help of this [CSS hamburger menu tutorial](#Credits) linked below.

	For the navigation the icon & text on the left brings you to the home page. The other two are clearly different in yellow to the right of the nav bar. The page you're on is indacated in white underlined, (when in mobile view this link is hidden as it cant be clicked).

	![Navigation bar - nav](assets/markdown_images/nav.png "navbar")

	The footer is a simple flexbox container with centred content and a restriction in the icons of *max-width: 700px;* so the icons dont spread too far apart on larger screens.

	![Footer and icons inside](assets/markdown_images/footer.png "footer")

	#### Card section

	The card section is also often the main part of a website as it is the bullet-points for what the visitor will get. In this case learn points to keep in mind while watching and following along with the videos.

	<details><summary>Image of card section</summary>

	![Card & icon section](assets/markdown_images/card.png "icon cards")

	</details>

### Typography
- [Cabin](https://fonts.google.com/?query=Cabin) - for the h1, h2 and h3 as a strong, clean, easy to read font.

- [Rubik](https://fonts.google.com/specimen/Rubik?query=Rubik) - for the body, simmiler to Cabin font, midderen and clean in style

- [Libre+Baskerville](https://fonts.google.com/specimen/Libre+Baskerville?query=Libre+Baskerville) - fo tthe quotation on the home page, a more flowery font looks like a book type of font.

### Color Choices
I went for a muted color palette which is in keeping with a lot of yoga websites.
The buttons stand out in the hierarchy with stronger colors as do the videos against the off white.

## Style Guide


### Responsiveness
Mobile first and then 3 main breakpoints for desktop (768px, 980px 1440px).
The 1440px large display is so the website doesn't break on large QHD monitors.





### Accessibility
- 'alt' text on images 
- 'title' on the social icons in the footer
- contrasting colors
- easy to see buttons and navigation area
- background images to to be distracting or masking the text
e.g on mobile version of the site I darkened the background Hero image so as not to detract from the text as it is displayed on the small screen.


### Consistency
- colors, I reduced the colors used by about half.
- footer same feel placeing at the bottom of the page.
- icons match both from Google and Boxicons.  
- fonts match header fonts and content (paragraph) fonts.
- padding is same for each element across the web site.

## Testing

- Lighthouse in Chrome DevTools.


Best Practices on the video page was the only one that was low at (85), "SameSite cookie" this is server-side issue I think.
I also reserched this here on [stackoverflow](https://stackoverflow.com/questions/60822936/where-to-add-samesite-none). 

	*Tested in Incognito mode.*

![website in Lighthouse in Chrome ](assets/markdown_images/both_lighthouse.png "Lighthouse score")

After a few errors like images being too big or missing title on social links (facebook, twitter)
I ran Lighthouse a few times to check my code and text.
Tested both mobile and desktop.

### Validator Testing
- HTML
<https://validator.w3.org/>

After a few errors I went back to the code and researched the fixes using Google or Stack overflow to find the solution.
For example I had a problem with the "quote section"  *< picture > < source srcset...* were the error was showing I had to have a "sizes" along with the "source".


- CSS
<https://jigsaw.w3.org/css-validator/>

Passed with no errors in the code.


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


#### Responsive Testing
I used Chrome and Firefox "developer tools, device toggle" to check the responsiveness for each device. From iPhone, roughly 320px, to laptop 1920px, and to the desktop at 2560px (QHD).


I also used "developer tools" to check the margin and padding on each element to check the style didn't break, especially on smaller devices usually caused by margin or overflow fixed widths to elements on the page. Fixing any sizing errors or overflow of content as I went along.

## Deployment
Deployed using GitHub Pages. <https://github.com/dmcginley/project1_yoga_site/settings/pages>

Once uploaded I checked everything was working ok. I checked response times and refresh time.
Also checking every link and button was working.

## Image optimization for the web

### “srcset”, and “sizes” for [Responsive Images](#How-to-Use-HTML5-“picture”,-“srcset”,-and-“sizes”-for-Responsive-Images)

I wanted to make the images responsive through pulling in different resolution images depending on screen size.
Using both Webp and Jpg (as a fall-back).


How to Use HTML5 “picture”, “srcset”, and “sizes” for Responsive Images



After I edited the images in [Gimp](https://www.gimp.org/), I'd pass the images through Optimizilla or Tinypng and then put them in the image folder. *(Personally I found Optimizilla to be the better of the two websites for keeping a clean image).*

- [Optimizilla](https://imagecompressor.com/)

- [Tinypng](https://tinypng.com/)

Later I also used Imgbot, automated optimizing of my images as they're uploaded to GitHub, *(Free for open source projects).*

- [Imgbot](https://github.com/marketplace/imgbot)

 [squoosh](https://squoosh.app/) - Used to convert jpg files to WebP. 

favicon.io used for generating the set of images for the tab in the browser.

- favicon.io
<https://favicon.io/favicon-converter/>

## Resources
*General reading and resources.*

- The Code Institute course material.

- [w3schools](https://www.w3schools.com/) to help with links and lists.

- [MDN Web Docs](https://developer.mozilla.org/en-US/) for looking up flex and grid, scaling images, iframe for video content.

- [*CSS-TRICKS](https://css-tricks.com/)

- [Scrimba](https://scrimba.com/) video tutorials about Flex & Grid.

- [web.dev](https://web.dev/learn/) the Learn section, Responsive Design, Media queries.

- [Can I use](https://caniuse.com/) to check browser support for different elements on the site such as SVG icons, WebP images.



- [How to Use HTML5 “picture”, “srcset”, and “sizes” for Responsive Images](https://webdesign.tutsplus.com/tutorials/quick-tip-how-to-use-html5-picture-for-responsive-images--cms-21015?utm_source=pocket_mylist)


Book I used for further reading on HTML5 semantic markup.
- [HTML & CSS: Design and Build Websites](https://www.goodreads.com/book/show/10361330-html-and-css) *by Jon Duckett.*

## Credits
*Sites content, media, and help with implementing code for tutorials/on-line help.*

<fieldset>

In this section you need to reference where you got your content, media and extra help from. It is common practice to use code from other repositories and tutorials, however, it is important to be very specific about these sources to **avoid plagiarism**.

</fieldset>

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

- Pure CSS hamburger menu learnt from 'FollowAndrew' on YouTube <https://www.youtube.com/watch?v=sjrp1FEHnyA&t=1707s>


#### Using Flex & Grid.

- Using Flex and Grid elements from Kevin Powell on YouTube <https://www.youtube.com/kepowob>

- Layout of the body divided into a 3 section grid
from Layout Land <https://www.youtube.com/channel/UC7TizprGknbDalbHplROtag>


- Aligning Flex items for the Footer **Traversy Media**
<https://www.youtube.com/watch?v=3YW65K6LcIA>

#### Form
- Code Institute course material. The section for Semantic Form Elements, eg. fieldset, legend.

- < fieldset > - The Field Set element form Mozilla <https://developer.mozilla.org/en-US/docs/Web/HTML/Element/fieldset>

- Form from w3schools and the book HTML&CSS *by Jon Duckett* <https://www.w3schools.com/howto/howto_css_contact_form.asp>


## Content

The text for the Home page I came up with myself as I used to work in a smiler field of health teaching and training.

The text for the Video page was taken from Wikipedia articles on the [list of asanas](https://en.wikipedia.org/wiki/List_of_asanas).

Yoga on Wikipedia
<https://en.wikipedia.org/wiki/Yoga>

#### Icons
- [Material Icons](https://developers.google.com/fonts/docs/material_icons) - The icons in the card section were taken from Google's Material Icons. Idownloaded the svg and used inside img tags.


- [Boxicons](https://boxicons.com/) - The icons in the footer were taken from Boxicons. I downloaded the svg code and paisted it in to try get everything smaller on the site to try and help with loading speeds.

- [Bootstrap Icons](https://icons.getbootstrap.com/) - The star icons on the video page are from Bootstrap, also using the svg code, rather than the images.

#### Images and Videos
The images and photos used on the site are from [Pexels.com](https://www.pexels.com/)

 The watermark I created using [Inkscape](https://inkscape.org/) *(vector graphics software).*

<details><summary>Logo in Inkscape</summary>

![Icon/Watermark created in Inkscape ](assets/markdown_images/inkscape.png "Inkscape")

</details>





