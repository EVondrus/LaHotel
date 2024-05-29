# La Hotel

![GitHub contributors](https://img.shields.io/github/contributors/EVondrus/Lahotel)
![GitHub last commit](https://img.shields.io/github/last-commit/EVondrus/LaHotel)
![GitHub language count](https://img.shields.io/github/languages/count/EVondrus/LaHotel)
![Font Awesome version](https://img.shields.io/badge/Font%20Awesome-v6.5.2-purple)
![Travis CI Build]()


[Here is a link to the final project]()

This site is a comprehensive hotel management system, designed to streamline the operations of both hotel owners and guests alike. This platform is tailored to enhance the user experience for those seeking accommodations, offering a seamless journey from browsing to booking, alongside robust administrative tools for managing hotel operations efficiently.

This site is fully responsive on all modern screen sizes, and it allows the different users to easily add, edit or delete their profiles, reservations, hotel and room details.

This site was built using HTML, CSS, Bootstrap, JavaScript, jQuery, Python, Django, and it uses a SQL database through Code Institute.

![Final project mockup screenshot from Am I Responsive]()

## Contents

* [Icon Key](#icon-key)

* [User Experience](#user-experience)
  * [Initial Discussion](#initial-discussion)
  * [User Stories](#user-stories)
  * [Project goals](#project-goals)

* [Design](#design)
  * [Color Scheme](#color-scheme)
  * [Typography](#typography)
  * [Imagery](#imagery)
  * [Wireframes](#wireframes)
  * [Features](#features)
  * [Future Features](#future-features)
  * [Navigation bar](#navigation-bar)

* [Database Design](#database-design)

* [Technologies Used](#technologies-used)
  * [Languages](#languages)
  * [Workspace](#workspace)
  * [Version Control](#version-control)
  * [Wireframing](#wireframing)
  * [Responsive Design](#responsive-design)
  * [Documentation](#documentation)
  * [Site Design](#site-design)
  * [Database Design](#database-design)
  * [Frameworks, Libraries and Others](#frameworks-libraries-and-others)

* [Deployment](#deployment)

* [Testing](#testing)
  * [Solved Bugs](#solved-bugs)
  * [Known Bugs](#known-bugs)

* [Credits](#credits)
  * [Code](#code)
  * [Content](#content)
  * [Media](#media)
  * [Acknowledgements](#acknowledgements)

---

## Icon key

&#128272; <-- Superuser only access

&#128100; <-- Logged In Only

&#128683; <-- Logged Out only

&#9989; <-- Yes / Visible

&#10060; <-- No / Not visible

[Back to the top](#lead-shot-hazard)

---

## User Experience

### Initial Discussion

* This project is something I wanted to create as I'm a passionate traveler and previously been working in the hotel buisness.
* I wanted to create a website linked to a database, which allows users to log in, view hotel information, room details, and make room reservations.
* I wanted the administration to be able to add, edit and delete hotel information, room details and reservations.

### User Stories

**User Story Id** | **As a / an...** | **I should be able to...** | **So that I can...** |
| --- | --- | --- | --- |
||| **Overall** ||
| A1 | Site User | View hotel details, rooms, room details and contact information | Make informed decisions about the choice of my stay and reservation |
| A2 | Site Owner | Match the design and personality of the hotel with the site | Easily show guests that this site is linked to the hotel |
| A3 | Site Owner | Offer a website that is easy to navigate and free of confusion | Avoid the stress of guests needing more assistance than necessary |
| A4 | Staff User | Access necessary tools and information | Perform job duties effectively |
| A5 | Admin User | Manage the overall operation of the hotel | Ensure smooth daily operations |
||| **Viewing & Navigation** ||
| B1 | Site User | Easily navigate the site | Enjoy a seamless browsing experience |
| B2 | Site User | View detailed information and amenities offered by the hotel | Understand what the hotel provides |
| B3 | Site User | Browse through all available rooms | Select accommodations that meet my preferences |
| B4 | Site User | View full room information including price, amenities, images, capacity and availability | Evaluate options before making a reservation |
| B5 | Site User | Easily see the total estimated cost of my stay | Budget accordingly for my visit |
| B6 | Site User | Receive visual feedback upon completing actions | Instantly confirm that my interactions with the site are acknowledged |
| B7 | Site User | Contact the hotel via the site | Ask questions or request services |
||| **Registration & User Accounts** ||
| C1 | Site User | Register for an account | Store my personal details for faster bookings in the future |
| C2 | Site User | Log In | Access my account |
| C3 | Site User | Log Out | 	Protect my personal information on public or shared devices |
| C4 | Site User | Receive an email confirmation after creating an account | Verify my registration was successful |
| C5 | Site User | Create, update or delete my personal information | Ensure my profile remains accurate and up-to-date |
| C6 | Site User | Reset Password | Easily recover my account access if I forget my password | Regain access to my account without needing to create a new one
| C7 | Site User | Request Account Deletion | Have the option to permanently delete my account | Exercise control over my personal data post-stay
||| **Sorting & Searching** ||
| D1 | Site User | Sort rooms by category | Easily compare different room types |
| D2 | Site User | View details of a specific room category | Get a clear idea of what each room category offers |
| D3 | Site User | Input my desired check-in and check-out dates | Sort room availability according to my travel schedule |
| D4 | Site User | View availability calendar for each room category | At a glance, see which days rooms are available |
||| **Reservation** ||
| E1 | Site User | Make a reservation online without having to pay upfront | Secure my room for my stay without immediate financial commitment |
| E2 | Site User | View details of my reservation | Confirm the specifics of my booking |
| E3 | Site User | Easily modify my reservation details from my profile page | Adjust my stay based on changing plans |
| E4 | Site User | Revisit my reservation after logging out and back in | Retrieve my booking details |
| E5 | Site User | Receive a confirmation email with details of my reservation | Have a record of my confirmed booking |
| E6 | Site User | Cancel my reservation through the site | Change my plans if needed |
| E7 | Site User | Make a room reservation without having to log in | Quickly and easily secure a room for my stay without the need for an account |
||| **Hotel Admin Management** ||
| F1 | Admin User | Edit any hotel or room details | Update details of the hotel and rooms |
| F2 | Admin User | Delete any details about the hotel or room listings | Remove old information from the site and maintain accuracy and relevance of our inventory |
| F3 | Admin User | Add a new hotel details and/or room types | Add new hotel features and/or Expand our accommodation options |
| F4 | Admin User | Create, read, update, and delete reservations | Efficiently manage room bookings |
| F5 | Admin User | Create, read, update, and delete staff profiles | Manage hotel staff and their responsibilities |
||| **Hotel Staff Management** ||
| G1 | Staff User | Create and update their account staff profiles | Personalize their profile for hotel operations |
| G2 | Staff User | Create, update and delete reservations | Assist guests with room reservation |
| G3 | Staff User | Create, update and delete guest details | Assist guests with personal details |
| G4 | Staff User | Create, update, and delete room statuses | Update room availability and manage reservations |
||| **Authentication & Security** ||
| H1 | Site User | Verify my email address | Ensure my account is set up securely |
| H2 | Site User | Be confident that my password is stored securely | Feel safe from malicious activity |
| H3 | Site Owner | Be confident of the security of the restricted pages | Feel safe from malicious activity |


### Project Goals

* The main goal is to create an easily editable site to elevate the guest experience and simplify hotel operations.
* Designed with a user-centric approach, the platform should cater the needs of site users, site owners, staff users, and admin users.
* This project also demonstrates my understanding of maintaining a database attached to a website, with full CRUD (Create, Read, Update and Delete) functionality, using CI SQL database, and Cloudinairy Services.

[Back to the top](#)

---

## Design

### Color Scheme

* The main colors used in this site are Dark Slater Blue, Gold and Cloudy White.
* These main colors are the colors in the hotels's logo, and they permeate through the site.
* These colors were each selected to embody the serene elegance and natural beauty of a Scandinavia, reflecting the tranquil ambiance and sophisticated charm of the setting.
* A dark green has been used for the sucess messages, to signify that this is a successive action.
* A dark red has been used for all Delete buttons, to signify that this is a destructive action.
* The mustard yellow has been used for the hover state of the call-to-action buttons.
* Different color shades have also been used on the hover state of the social media icons on the Contact page to match the icons.

![Color scheme](static/docs/img/colors.png)

### Typography

* For the fonts, I selected Roboto Slab for headings and Open Sans for body text, both available through Google Fonts.
* These choices were made with a keen focus on readability and accessibility, ensuring a welcoming experience for users with dyslexia and partial visual impairments.
* The elegance and readability of these fonts contribute to the app's overall sophistication and ease of use.
* By utilizing the standard HTML font size of 16px, ensuring to not have any fonts smaller than that, to aid visually impaired users.
* Also, the recommended smallest font size for accessible websites is 12px, so by keeping all font sizes at the HTML standard of 16px or above, I ensured to be fully compliant with the [Penn State University Accessibility and Usability Guidelines](https://accessibility.psu.edu/fontsizehtml/).
* Font sizes are also able to be zoomed to 200% without losing contrast or functionality, to comply with the [WCAG Guidelines on fonts](https://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-scale.html).
* Lastly, to prevent the app from appearing overly assertive, I incorporated a mix of uppercase and lowercase text strategically.

![An example of the font used]()

### Imagery

* The imagery and logo featured within this hotel app are meticulously crafted using advanced [AI technologies]()
* Integrated to forge a powerful connection between the hotel's brand and the app's interface.
* Subtle box shadows and gradients have been artfully applied. These design elements echo the hotel's graphic styling, characterized by neutral, soft colors and refined lines, enhancing the app's aesthetic appeal.
* All links have their underlines removed for stylistic purposes. The links in the footer re-gain their underlines when they're hovered over or focused on.
* All interactable objects have hover and focus styles applied to make it clear to the user that those objects are interactable.
* Icons from [Font Awesome](https://fontawesome.com/) have been used throughout the site to add meaning where relevant. These icons are accompanied by either visible text or descriptive aria-labels, ensuring inclusivity and accessibility.
* Button and link colors have been used to convey meaning, mainly in the use of the color red to convey 'Delete' or 'Cancel' as dangerous actions.

### Wireframes

* [Wireframes for desktop, mobile, and tablet for this project]().
* [Database schema for this project]().

### Features

### Home page

* This feature allows the user to:
 * Get a view of the hotel's ambiance with high-quality images and engaging text, providing visitors with a glimpse of the hotel's offerings.
 * Fill out a check in - check out form to check for room avaliability of the desired dates. 
 * Viewing the room types in a carousell - each option linking to a detailed room description page with the choice to make a room reservation.

#### Create a user profile

* This feature allows the user to:
  * Register for an account with an email address, first name, last name and password.
  * Ensure no typos by entering the password twice, with the site checking to confirm that the passwords match.
  * Ensure the correct email address by sending a verification email to the email address the user has supplied. ( CHECK )
  * &#128100; Store their details for faster checkout.
  * &#128100; Keep a record of their reservation history.

![User's profile, including details update form]()

### Log in

* This feature allows the user to:
 * Log in to the site with email address and password.
  * Check the box to "remeber me" for upcoming logins.
 * Browse their profile page.
  * View, update and delete their profile details.
 * Browse their room reservations.
  * View, update and cancel room reservations.
 * Change password.

#### Rooms

* This feature allows the user to:
  * View all rooms of the hotel on the website.
  * Browse rooms by category through the main navigation bar or carousell from the homepage.
  * Click on a room card to view the full room details, including:
    * Category
    * Price per night
    * Capacity
    * Image
    * Description
    * User Input check in - check out dates
    * Avaliability for desired dates
  * Click the 'Book' button to be redirected to the page for making a reservation of the selected room.

![Rooms page with back to top button]()

#### &#128272; Create, Edit and Delete Room details

* This feature allows the superuser to:
  * Add a new category and/or room details to the hotel.
  * Edit an existing categoy or room details.
  * Delete an existing category or room.
  * Include images, by uploading directly from the superuser's computer.

![Admin functionality to create, update or room details]()

#### &#128272; Create, Edit and Delete Hotel details

* This feature allows the superuser to:
  * Add a new details to the About and Contact page.
  * Edit an existing information.
  * Delete an existing information.
  * Include images, by uploading directly from the superuser's computer.

![Admin functionality to create, update or delete hotel details]()

#### &#128272; Create, Edit and Delete Room reservations

* This feature allows the superuser to:
  * Add a new room reservation.
  * Edit an existing reservation.
  * Delete an existing reservation.

![Admin functionality to create, update or delete room reservation]()

#### Confirm to delete modal

* This feature allows the user to:
  * &#128272; Confirm deletion of a reservation or their profile.
  * &#128272; Avoid accidentally deleting a product.

![Confirm to delete modal]()

#### Reservation

* This feature allows the user to:
  * Add check in and check out dates.
  * Fill up details for the reservation
   * name, lastname
   * no. of guests
   * phonenumber
   * address
   * emailadress
  * Adjust the quantity of rooms.
  * Edit or delete room category for the the reservation.
  * View the grand total and details in the reservation.

![A shopping bag with an item in it](static/docs/img/bag-feature.png)

#### Navigation bar

The navigation bar changes depending on user status and screen size:

| Nav Link | &#128683; | &#128100; | &#128272; |
|-------|-----|-----|-----|
| Logo (Homepage) | &#9989; | &#9989; | &#9989; |
| Home | &#9989; | &#9989; | &#9989; |
| Rooms | &#9989; | &#9989; | &#9989; |
| Room Details | &#9989; | &#9989; | &#9989; |
| Contact Us | &#9989; | &#9989; | &#9989; |
| About | &#9989; | &#9989; | &#9989; |
| Hotel Management | &#10060; | &#10060; | &#9989; |
| Profile | &#10060; | &#9989; | &#9989; |
| Log Out | &#10060; | &#9989; | &#9989; |
| Log In | &#9989; | &#10060; | &#10060; |
| Register | &#9989; | &#10060; | &#10060; |

* Navigation bar

![Overall navigation bar]()

* Logged in

![Logged in navigation dropdown]()

* Logged out

![Logged out navigation dropdown]()

* An admin

![Admin navigation dropdown]()

* On small screen sizes

![Mobile navigation burger icon]()
![Mobile navigation bar expanded]()

#### Auto-updating copyright year

* The copyright year auto-updates to the current year.

![The auto-updating copyright feature]()

#### About Section

* This feature allows the user to:
  * Read about the hotel, it's history and owners.
  * Navigate to the room details.
  * Navigate to any of the hotel's social media pages.

 ![The About page]()

#### Contact section

* This feature allows the user to:
  * Contact the hotel via email for queries about their stay or reservation.
  * View adress and location including google maps.
  * View phone number to contact the hotel in a quicker manner.
  * Navigate to any of the hotel's social media pages.
  * It also has a customised hover feature, where when the user hovers over each icon, the icon becomes the main color of the site that it is linking to.

![The Contact Us page, with an example of the hover effect applied]()

### Future Features (TBC)

* Stock count for each product size, including out-of-stock sizes.
* Book button is disabled if the chosen room category is not avaliable for the desired dates.
* Social media login via Facebook and Google.
* Special offers.
* Regex or number validation on phone number fields.

### Defensive Design

* Form validation
  * This has been used on every form input on the site to ensure the correct data is added.
  * If incorrect data is added, red warning text appears, to instruct the user on how to fix the error.
  * Image file uploads are validated by [Django's ImageField](https://docs.djangoproject.com/en/3.2/ref/models/fields/#imagefield), to ensure that the images that are uploaded are genuine images, and aren't malicious.
  * Messages when an action is completed
  * A message will appear in the top right of the screen when the following actions are completed:
    * The user deletes their profile.
    * The user edits the date of their resrvation.
    * The user cancel their resrvation.
    * A reservation succeeds.
    * A reservation fails due to unavaliability.
    * An error occurs.
    * &#128100; A user updates their profile information.
    * &#128100; A user deletes their profile.
    * &#128272; A superuser adds a new room category.
    * &#128272; A superuser edits room details.
    * &#128272; A superuser delete a room or room category.
* Default image
  * A default image will display if there is no image added.
  * A default image will display if the image link has broken.
* Custom error pages
  * A custom 404 error page will show if the user attempts to visit a page that doesn't exist.
  * A custom 500 error page will show if an internal server error occurs.
* Login validation
  * The `@login_required` decorator has been used to ensure that the restricted pages are secure.
  * If a logged-out user tries to access a restricted page, they will be redirected to the login page.
  * If a logged-in user without access rights tries to access a restricted page, it redirects them to the homepage, and presents them with a message saying 'You do not have access to this page'.

[Back to the top](#)

---

## Database Design (TBC)

This database uses a SQL database through Code Institure. [ER Diagram]().

[Back to the top](#)

---

## Technologies Used

### Languages Used

#### HTML

* [HTML5](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5)

#### CSS

* [CSS3](https://developer.mozilla.org/en-US/docs/Archive/CSS3#:~:text=CSS3%20is%20the%20latest%20evolution,flexible%20box%20or%20grid%20layouts.)

#### JavaScript

* [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
* This project uses JavaScript ES6 and jQuery.

#### Python

* [Python](https://www.python.org/)
* This project uses Python 3.12.3.

### Workspace

#### GitPod & Visual Studio Code

[GitPod](https://gitpod.io/) was used as a virtual IDE workspace to build this site.
[Visual Studio Code](https://code.visualstudio.com/) was used as a local IDE workspace to build the site.

### Version Control

#### Git

[Git](https://git-scm.com/) was used for version control by utilizing the Gitpod and VS Code terminal to add and commit to Git and push to GitHub.

#### GitHub

[GitHub](https://github.com/) is used to store the code for this project after being pushed from Git.

### Wireframing

#### Balsamiq

[Balsamiq](https://balsamiq.com/) was used to create the wireframes during the design process.

### Responsive Design

#### Am I Responsive Design

[Am I Responsive Design](http://ami.responsivedesign.is/#) was used to check the responsive design of the site, and to create the final site image.

#### Responsinator

[Responsinator](http://www.responsinator.com/) was used to help improve the responsive design on a variety of devices.

### Documentation

#### Shields.io

[Shields.io](https://shields.io/) was used to create the GitHub badges for the top of this README.md file.

#### Carbon

[Carbon](https://carbon.now.sh/) was used to take elegant screenshots of code for this documentation.

#### JSHint extension

[JSHint Extension](https://open-vsx.org/vscode/item?itemName=dbaeumer.jshint) was used on GitPod to maintain code quality at all times.

#### markdownlint extension

[markdownlint Extension](https://open-vsx.org/vscode/item?itemName=DavidAnson.vscode-markdownlint) was used on GitPod to ensure all markdown was correctly formatted.

### Site Design

#### Font Awesome

[Font Awesome](https://fontawesome.com/) was used on all pages to add the icons.

#### Google Fonts

[Google Fonts](https://fonts.google.com/) was used to select all the fonts on the site.

#### Favicon.io

[favicon.io](https://favicon.io/) used to create a site favicon.

#### Calendar

[Python calendar module](https://docs.python.org/3/library/calendar.html) was used to display the date of upcoming gigs in a user-friendly format.

### Packages (TBC)

| Name | Purpose |
|------|---------|
| Django | Framework |
| Flake-8 | Syntax |
| Pylint | Syntax |
| Pillow | Images |
| django-allauth | Authentication |
| django-storages | Custom Storage Backends |
| django-countries | Country Form Field |
| gunicorn | WSGI HTTP Server |
| django-crispy-forms | Front End Form Rendering |
| dj-database-url | Database Configuration |
| psycopg2-binary | PostgreSQL DB Adaptor |
| coverage | Test Coverage |
| travis.ci | Testing |
| | |

### Hosting

#### Heroku

[Heroku](https://www.heroku.com) was used to deploy the live site initially.

#### Cloudinairy

[Amazon AWS S3](https://s3.console.aws.amazon.com/s3) was used to host this project's images and static files.

### Frameworks, Libraries, and Others

#### Google DevTools

[Google DevTools](https://developer.chrome.com/docs/devtools/) was used to help find what code correlated to which feature.

#### Lighthouse

[Lighthouse](https://developers.google.com/web/tools/lighthouse) was used to ensure that the code was as performant as possible, conforming to best practices, and SEO and Accessibility guidelines.

#### WebPageTest

[WebPageTest](https://www.webpagetest.org/) was used to ensure that the code was as performant as possible, conforming to best practices, and SEO and Accessibility guidelines. As it is often more reliable than Lighthouse, this was used near the end of the project to fix any remaining issues.

#### Jinja

[Jinja](https://jinja.palletsprojects.com/en/3.0.x/) was used to help create the templating for this site.

#### Bootstrap

[Bootstrap](https://getbootstrap.com/) was used to create a beautiful, responsive website.

#### jQuery

[jQuery](https://jquery.com/), a JavaScript library was used for DOM traversal, HTML manipulation, and event handling.

#### Djecrety

[Djecrety](https://djecrety.ir/) was used to generate a strong `SECRET_KEY`.

#### pip

[pip](https://pip.pypa.io/en/stable/) was used to install the required dependencies for this site.

#### Slack

[Slack](https://slack.com/intl/en-gb/) was used to communicate with the [Code Institute](https://codeinstitute.net/) community for help and support with bug fixes, and a peer code review.


[Back to the top](#)

---

## Deployment (TBC)

[Please click here for all Deployment steps and requirements]().

[Back to the top](#)

---

## Testing (TBC)

[Click here to view the full testing steps](), which were completed on every device and Google Chrome, Safari and Microsoft Edge browswers, and screenshots of testing.

### Solved Bugs (TBC)



### Known Bugs

* None found, if any errors are found, please contact me via my GitHub ([EVondrus](https://github.com/EVondrus/)) to get them fixed.

[Back to the top](#)

---

## Credits

### Code

* [Font Awesome](https://fontawesome.com/): Library of icons used for social media and download links.
* This website was made with the help of the tutorials from Code institute for the Code Star project by Chris Zielinski. The code has been customised and improved to fit this project.
* [Django Documentation](https://docs.djangoproject.com/en/3.2/) has been used to ensure correct syntax usage throughout the code.
* [Stack Overflow](https://stackoverflow.com/) has been used to help with deciphering the django error codes, and searching for bug fixes.
* [Chris Anstey](https://github.com/ansteychris), a Digital Experience Lead at Google, for the discussion we had about Lighthouse vs WebPageTest.
* I followed [this video from JustDjango](https://www.youtube.com/watch?v=NG48CLLsb1A) to add the Google social login functionality.
* Diasy Mc Dee
* [Dave Horrocks](https://github.com/DaveyJH) helped me with working out the logic and syntax for the Songkick API data and the Django testing.

### Content

* All content was created by [Ellenor Vondrus](https://github.com/EVondrus).
* [Click here to view links to all sites I used for research or testing]().

### Media

* All media on this site is created by me and my partner Mladen Djurdjevic, using AI technologies.

### Acknowledgements

* My mentor, Antonio Rodriguez, at [Code Institute](https://codeinstitute.net/), for continuous helpful feedback and support.
* The team at [Code Institute](https://codeinstitute.net/), for teaching me the necessary skills to create this site.
* The awesome people at the #community-Sweden slack channel.
* My partner Mladen Djurdjevic for his continuous support throughout my coding journey.

[Back to the top](#)


