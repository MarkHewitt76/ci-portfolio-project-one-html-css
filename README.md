# Ritual Effect

Ritual Effect are an alternative rock band based in Dublin, Ireland. This site aims to promote the band's music, live shows, etc. and is targeted towards both fans and music industry professionals alike, as well as the casual visitor. Users of this site will be able to access the band's music and videos through embedded audio and video files, links to media and streaming sites and links to their various social media pages. Users can also read a band biography, see news about upcoming releases and live performances, and find contact and booking information. There is also a form to sign up to the band's mailing list.

![Homepage screenshot](/assets/images/screenshots/ritualeffect_homepage_responsive.png "Homepage")

The site can be viewed [here](https://markhewitt76.github.io/ritual-effect/news.html).

## Features
---
### Existing Features
- Navigation Bar

    - Featured on all pages across the site, the navigation bar includes the Logo and links to the Home page, Band page, Music page, Videos page, News/Events page, Gallery and Contact page. It is fixed to the top and is identical in each page to allow for easy navigation. The logo also serves as a link to the Home page.

    - As a responsive design feature, the bar changes from an inline menu on larger screens to a drop-down, 'hamburger' style menu on small and medium sized screens, containing all the same links and features.

    - This section will allow the user to easily navigate from page to page across all devices without having to revert back to the previous page via the ‘back’ button. 

    - The link to the page currently being displayed appears in uppercase with a double underline, allowing the user to tell at a galnce where they are on the site.

    ![Inline navigation bar screenshot](/assets/images/screenshots/ritualeffect_navbar_inline_7.png "Inline navigation bar")
    ![Drop-down navigation menu screenshot](/assets/images/screenshots/ritualeffect_navbar_dropdown.png "Drop-down navigation menu")
    ![Drop-down navigation menu open screenshot](/assets/images/screenshots/ritualeffect_navbar_dropdown_1.png "Drop-down navigation menu open")

- Landing Page Image

    - The landing, as seen in the introductory section, includes a full-page, eye-catching photograph of the band posing flamboyantly outside Sin-É, a well-known Dublin music venue.
    
    - This immediately introduces the user to the band's flamboyant nature.

- Call to Action

    - The landing image is overlaid with a call to action linking to the music page and containing album art and icons providing visual information on where the link leads.

    - This lets the user know that the band's album, Fossils, is available on various streaming sites and directs them straight away to where they can listen to it.

    ![Call to action screenshot](/assets/images/screenshots/ritualeffect_calltoaction.png "Call to action")

- Footer

    - The footer section, also featured on all pages across the site, includes links to the relevant streaming and social media sites for Ritual Effect. The links will open to a new tab to allow easy navigation for the user. It also includes a copyright statement.

    - The footer is valuable to the user as it encourages them to stream the band's music, watch their videos and keep connected via social media.

    ![Footer screenshot](/assets/images/screenshots/ritualeffect_footer.png "Footer")


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

30th Jan


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

The live link can be found [here](https://markhewitt76.github.io/ritual-effect/news.html).

## Credits
---

### Content

- The code for the basic structure of the social media links in the footer, and of the signup form on the contact page, came from the Code Institute [Love Running](https://markhewitt76.github.io/love-running/index.html) project.

- *responsive youtube video *

- *fieldset style structure of dates on news items & gig listings *

- The basic CSS code for the hover effect of the submit button on the contacts page signup form came from Colt Steele's Udemy course, 'The Web Developer Bootcamp'. 

- The icons in the footer, drop-down menu and other various locations are taken from [Font Awesome](https://fontawesome.com/).

- The main fonts used are from [Google Fonts](https://fonts.google.com/).

### Media

All images, audio files and video files are the property of Ritual Effect and were supplied by the band.
