# GetHubby
Code Institute User Centric Frontend Develtopment: Milestone Project One

This is an imagined dating site for developers and specificially geared towards users of GitHub leveraging the existing social & community aspects of same. The goal is to have a site which appeals to developers by using industry lingo and to allow users to sign-up via existing, commonly used industry tools (i.e. GitHub).

[Go to GetHubby](https://nealbrophy.github.io/GetHubby/)

<img src="https://github.com/nealbrophy/GetHubby/blob/master/images/ipad.gif" alt="site demo on ipad" width="300px" align="left">

<img src="https://github.com/nealbrophy/GetHubby/blob/master/images/iphone.gif" alt="site demo on iphone" width="200px" align="center">


--- 
## UX
 
The site is intended to be simple and minimalistic while also colourful and fun. The information should be short and to the point but with a light-hearted tone where appropriate. Text should use industry terminology to present an industry-specific focus.

### User Stories:
- As a single person, I want a modern and appealing site which is simple to navigate.
- As a developer, I want a site that caters to my interests and is clearly aimed at people like me.
- As a modern user, I want a mobile-friendly site that looks as good on small screens as large.

### Wireframes

The initial wireframe was intended to outline the basic structure of the site and took inspiration from several popular current dating sites such as [EliteSingles](https://dating.elitesingles.com/), [Match.com](https://ie.match.com/), and [OKCupid](https://www.okcupid.com/). The second wireframe took the structure from the first, simplified it somewhat, and added some style/colour.

<img src="https://github.com/nealbrophy/GetHubby/blob/master/wireframes/wireframe-1-bw.png" alt="wireframe-1" width="318px" align="left">

<img src="https://github.com/nealbrophy/GetHubby/blob/master/wireframes/wireframe-2-colour.png" alt="wireframe-2" width="400px" align="center">


---

## Features

The navbar is responsive and will switch to a hamburger menu on small screens. 

The hero section contains an eye-catching jumbotron slideshow with images of a variety of possible users of site. A mock-typing animation was added to the text overlayed on the slideshow to suggest a relation to coding (and more specifically GitHub commands).

On med & large screens the about section contains simple, colourful flip-cards with a short title (and icons representing the theme of the title) on the front and a short summary of the feature in question on the back. One small screens the flip cards are replaced by a collapsing list.

The testimonials section shows a circular image of imagined couples beside a short quote from each couple. The button beneath each quote opens a mock Q&A with the couple (bootstrap-modal on larger screens, bootstrap-collapse on smaller screens).

The contribute section links to this GitHub repo. The sign-up section is made to look like a code-editor window with mock-HTML text.

---
 
### Existing Features

- Carousel with typing animation overlaid
- Links to relavant sections with smooth scroll
- Flip-cards
- Modal/Collapse for couple Q&As depending on screen size
- Buttons display a popout icon relating to the content/target of said button.
- On large screens there is an arrow icon with hover.css effect to highlight that additional content is below and links to the next section.

### Features Left to Implement

Once I've progressed in the JavaScript module I would like to add some more advanced features such as:
- A separate, customized modal for the Member Login.
- Randomised elements such as the color pallete for the flip-cards and the testimonials (couple images/names/quotes).
- GitHub OAuth integration, or at least the appearance of such. 
- A database of mock profiles and the ability to actually run through a sign-up process.

## Technologies Used

- [Bootstrap](https://getbootstrap.com/)
    - The project uses **Bootstrap** framework to simplify the initial layout and include advanced features such as the jumbotron and carousel.
- [Hover.css](http://ianlunn.github.io/Hover/)
    - The project uses the **Hover.css** collection to add appealing animations to icons & buttons.
- [Font Awesome](https://fontawesome.com)
    - The project uses **Font Awesome** for attractive and simple icons.
- [Google Fonts](https://fonts.google.com/)
    - The project uses **Google Fonts** for custom typefaces.

## Testing

The site has been developed using the mobile first approach with responsive elements where possible and media queries when necessary. All changes to the site were tested in Google Chrome, Firefox, Opera, and Vivaldi browsers (leveraging the developer tools in each) and across Windows (desktop), Linux (desktop & laptop), and Android operating systems (mobile).

During testing I found that some absolutely positioned elements had moved up/down further depending on which browser was used. The most consistant explanation I found for this was that absolutely positioned elements need to have a relatively positioned parent element. Making this change mitigated but did not eliminate the browser variance. Small variances in position at different screen sizes was addressed using media queries.

## Deployment

GetHubby is hosted on GitHub pages and is deployed from the master branch. Any changes committed to the master branch will automatically update on the GitHub deployment.

To run the site locally you can clone it using the following instructions:
- Create a folder in the desired location on your computer.
- Open a terminal ([Mac instructions](https://macpaw.com/how-to/use-terminal-on-mac)|[Windows instructions](https://www.quora.com/How-do-I-open-terminal-in-windows)|[Linux instructions](https://www.howtogeek.com/howto/22283/four-ways-to-get-instant-access-to-a-terminal-in-linux/))
- Navigate to the folder you created using `cd` command (e.g. `cd ~/Documents/GetHubby`)
- Type `git init`
- Next type `git clone https://github.com/nealbrophy/GetHubby`
- To break the link between your local copy and the repo at https://github.com/nealbrophy/GetHubby type `git remote rm origin`


## Credits

### Content
All text content was created by me. The modified Octocat images in the Testimonial and Contribute section were created by me for the purposes of this educational site only.

### Media
- [Pexels](https://www.pexels.com/)
    - adults-bald-bouquet Photo by Vasyl Potochnyi from Pexels
    - affection-beach-couple Photo by Gustavo Peres from Pexels
    - couple-facial-hair-garden-2440069 Photo by Gustavo Peres from Pexels
    - photo-of-women-facing-each-other-1167028 Photo by Brett Sayles from Pexels
    - couple-standing-on-top-of-hill-1995718 Photo by Luis Fernandes from Pexels
    - man-and-woman-forming-heart-hand-shape-1066801 Photo by juan mendez from Pexels
    - group-of-people-looking-at-laptop-screen-3183129 Photo by fauxels from Pexels
    - couple-about-to-kiss-2993031 Photo by Innoh Khumbuza from Pexels
- [Pixabay](https://pixabay.com/)
    - code-1839406_1920 Image by Pexels from Pixabay
- [Unsplash](https://unsplash.com/)
    - diego-rezende-CFIv79QxPjA-unsplash Photo by Diego Rezende on Unsplash


### Acknowledgements
- Typewriter effect inspired by [this CSS-Tricks article](https://css-tricks.com/snippets/css/typewriter-effect/) with simplified implementation taken from [this instructional video by Codingflag](https://www.youtube.com/watch?v=6vOJoAmbza0).
- Flip cards from [this W3C tutorial](https://www.w3schools.com/howto/howto_css_flip_card.asp)
- GITHUB®, the GITHUB® logo design, OCTOCAT® and the OCTOCAT® logo design are exclusive trademarks registered in the United States by GitHub, Inc.

## This student project and any original content therein is for educational use only ##
