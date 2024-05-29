# La Hotel

![GitHub contributors]()
![GitHub last commit])
![GitHub language count]()
![Font Awesome version]()
![Travis CI Build]()
![Testing coverage]()
![GitHub forks]()

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
  * [Audio](#audio)
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

#### Create a user profile

* This feature allows the user to:
  * Register for an account with an email address, username, and password.
  * Ensure no typos by entering the password twice, with the site checking to confirm that the passwords match.
  * Ensure the correct email address by sending a verification email to the email address the user has supplied.
  * &#128100; Store their details for faster checkout.
  * &#128100; Keep a record of their reservation history.

![User's profile, including details update form and order history]()

#### Rooms

* This feature allows the user to:
  * View all rooms of the hotel on the website.
  * Browse rooms by category through the main navigation bar.
  * Click on a room card to view the full room details, including:
    * Name
    * Category
    * Price per night
    * Image
    * Description
  * Click the 'Book' button to be redirected to the page for making a reservation of the selected room.

![Rooms page with back to top button]()

#### &#128272; Create, Edit and Delete Room details

* This feature allows the superuser to:
  * Add a new room to the hotel.
  * Edit an existing room.
  * Delete an existing room.
  * Include images, by uploading directly from the superuser's computer.

![Admin functionality to create and update products]()
