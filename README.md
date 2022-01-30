# Ritual Effect

Ritual Effect are an alternative rock band based in Dublin, Ireland. This site aims to promote the band's music, live shows, etc. and is targeted towards both fans and music industry professionals alike, as well as the casual visitor. Users of this site will be able to access the band's music and videos through embedded audio and video files, links to media and streaming sites and links to their various social media pages. Users can also read a band biography, see news about upcoming releases and live performances, and find contact and booking information. (There is also a form to sign up to the band's mailing list (time permitting!?).)

    (screenshot)

The site can be viewed [here](url).

## Features
---
### Existing Features
- Navigation Bar

    (screenshot)

- Landing Page Image

    (screenshot)

- Call to Action

    (screenshot)

- Footer

    (screenshot)

- Band Bio Page

(screenshot)

- Music & Videos Page

    (screenshot)

    - Music Section

    (screenshot)

    - Video Section

    (screenshot)

- News & Events Page

    (screenshot)

    - Latest News Section

    (screenshot)

        Begins with a link to a separate page listing upcoming gigs.

    - Upcoming Gigs Page

    (screenshot)

        Begins with links: 'Back to News'; 'Back to Home'.

- Gallery Page

    (screenshot)

- Contacts Page

    (screenshot)

### Features for Future Implementation

- Form??

## Testing
---

- Verify that this website works in various browsers: Chrome; Firefox; Safari; Opera.

- Confirm that this website is responsive, looks good and functions on all standard screen sizes using the devtools device toolbar.

- Confirm that the header, navigation links and content are readable and understandable.

### Bugs

#### Fixed Bugs
- #### Header navigation menu: sizing issue

    I'm not sure if it qualifies as a bug, per se, but I noticed a sizing problem with the header on smaller screens, especially in landscape mode, when I first started to style it for responsive design. It encroached too far down onto the hero image, obscuring it, even after downsizing, but if I made the navigation menu any smaller it became difficult to see. I also wanted to avoid reducing the size of the band logo at all, if possible.

    I realised that I could solve the issue by switching the original, inline-styled navigation menu for a 'hamburger' style drop-down menu on medium to small screen sizes. I achieved this by first wrapping the original #main-menu list in a div with an id of "main-menu-inline". I then created the drop-down menu inside the same `<nav>` element in HTML by using the `<details>` element with a Font Awesome 'hamburger' icon in the `<summary>` tag, and copied the original navigation menu list into the disclosure widget. I gave it an id of "main-menu-dropdown", styled it to look like a standard drop-down menu and set the media queries to switch between the two menu styles at 800 pixels using the property `display: none;`. The media queries can be seen below.
```css
    @media screen and (min-width: 801px) {
        #main-menu-dropdown {
            display: none;
        }
    }
    @media screen and (max-width: 800px) {
        #main-menu-inline {
            display: none;
        }
    }
```
- #### Forced to reset after 6 commits as large video file prevented push


#### Unfixed Bugs

### Validator Testing

- HTML

    Check no errors are returned when passing through the official [W3C validator](url).

- CSS

    Check no errors are returned when passing through the official [(Jigsaw) validator](url).

- Accesiblity

    Confirm that the website is accsessible and easy to read by running it through Lighthouse in devtools.

    (screenshot)

## Deployment
---
The site is to be deployed to GitHub pages. The steps to deploy are as follows:

- In the GitHub repository, navigate to the Settings tab
- From the source section drop-down menu, select the Master Branch
- Once the master branch has been selected, the page will be automatically refreshed with a detailed ribbon display to indicate the successful deployment.

The live link can be found [here](url).

## Credits
---

### Content

- The code for the basic structure of the social media links in the footer came from the Code Institute [Love Running](https://markhewitt76.github.io/love-running/index.html) project.

- The icons in the footer, drop-down menu and other various locations are taken from [Font Awesome](https://fontawesome.com/).

- The main fonts used are from [Google Fonts](https://fonts.google.com/).

### Media

All images, audio files and video files are the property of Ritual Effect and were supplied by the band.
