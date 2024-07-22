-- Pictures --

![Screenshot 2024-07-22 101447](https://github.com/user-attachments/assets/38298d3b-664e-412d-8ced-0b4fa1dc3af3)
![Screenshot 2024-07-22 101508](https://github.com/user-attachments/assets/62c436a4-91b3-4d84-b62b-493ed0b8fc3a)
![Screenshot 2024-07-22 101529](https://github.com/user-attachments/assets/aa5cfd5a-a08b-43a2-80a1-bca7e55b8990)
![Screenshot 2024-07-22 101557](https://github.com/user-attachments/assets/6c8be406-1fcf-404c-b0cf-b6198aa92009)
![Screenshot 2024-07-22 101619](https://github.com/user-attachments/assets/2b2935c8-8d74-4e88-ab59-d54ad03fc0ef)
![Screenshot 2024-07-22 101629](https://github.com/user-attachments/assets/b9f351ae-46fe-4386-b134-3007a44f4bb6)
![Screenshot 2024-07-22 101654](https://github.com/user-attachments/assets/393b788c-3bfa-47aa-b51c-18069d8baef6)
![Screenshot 2024-07-22 101708](https://github.com/user-attachments/assets/b3d13a0d-5cec-401a-95f6-dc417a980962)
![Screenshot 2024-07-22 101727](https://github.com/user-attachments/assets/bfda424f-c393-4f9a-af94-d4b7164c98e4)
![Screenshot 2024-07-22 101742](https://github.com/user-attachments/assets/97ca2267-9ac2-42ac-958b-bfa7b3d23786)
![Screenshot 2024-07-22 101800](https://github.com/user-attachments/assets/e80ed06d-b7ab-492a-9f4a-c38b3c6ecc15)
![Screenshot 2024-07-22 101812](https://github.com/user-attachments/assets/88107943-4c3c-450a-a7e1-6a10eb1d9400)
![Screenshot 2024-07-22 101824](https://github.com/user-attachments/assets/eaeb2926-3ae8-48be-87b9-f077b604b551)
![Screenshot 2024-07-22 101853](https://github.com/user-attachments/assets/9c4c5e8c-ecc6-4f64-894d-b0514c6b5759)
![Screenshot 2024-07-22 101907](https://github.com/user-attachments/assets/61efb1c4-04ba-48de-a63a-68a91919c6db)


-- Bio --
# Home Page Documentation

## Overview

This document provides an overview of the `home.html` page for the Task'd application. The page includes a navigation bar, a welcome section, an about section, and an accordion with additional information.

## Structure

### HTML Structure

The page is structured using HTML5 and Bootstrap 5.3.2 for styling and responsiveness.

### Head Section

- **Title**: Task'd
- **Meta Tags**: Charset, viewport settings
- **Bootstrap CSS**: Included via CDN

### Body Section

#### Navbar

- **Brand Logo**: Links to a YouTube video
- **Brand Name**: Links to `home.html`
- **Navigation Links**:
  - Home
  - About
  - Connect
- **Dropdown Menu**:
  - Task'd Menu
  - Task Details
  - Create Tasks
- **Login/Register Button**: Triggers an offcanvas component

#### Offcanvas Component

- **Login Form**: Includes fields for Username, Email, and Password
- **Buttons**: Login and Register

#### Welcome Section

- **Card**: Displays a welcome message and a motivational quote

#### About Section

- **Jumbotron**: Contains a carousel with images and a description of Task'd

#### Accordion

- **How It Works**: Describes the gamified task management experience
- **Helps Gamers**: Explains how Task'd helps users stay organized and motivated
- **Speed**: Placeholder for additional information

## Detailed Breakdown

### Navbar

```
<nav  class="navbar navbar-expand-md bg-dark navbar-dark">
	<!-- Navbar content -->
</nav>
```

- **Brand Logo**: `<a class="navbar-brand"`- `href="https://www.youtube.com/watch?v=dQw4w9WgXcQ">`
- **Brand Name**: `<a href="home.html" class="navbar-brand">`
- **Navigation Links**: `<ul class="navbar-nav ms-auto">`
- **Dropdown Menu**: `<li class="nav-item dropdown">`
- **Login/Register Button**: `<button class="btn btn-success btn-sm" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasTop" aria-controls="offcanvasTop">`

### Offcanvas Component

```
<div  class="offcanvas offcanvas-top"  tabindex="-1"  id="offcanvasTop"  aria-labelledby="offcanvasTopLabel">
	<!-- Offcanvas content -->
</div>
```

- **Login Form**: `<form class="row">`
  - Username: `<input type="email" class="form-control" id="emailInput" placeholder="Max 10">`
  - Email: `<input type="password" class="form-control" id="password" placeholder="Enter Email">`
  - Password: `<input type="email" class="form-control" id="emailInput" placeholder="Enter Password">`
- **Buttons**: `<a class="btn btn-warning mt-2 text-white" href="/Pages/task_dashboard.html" role="button">Login</a>`

### Welcome Section

```
<section>
	<div  class="card text-center bg-dark border-dark py-5 my-5">
	<!-- Welcome content -->
	</div>
```

</section>

- **Card Header**: `<div class="card-header shadow mb-2 py-5 bg-dark text-white border-dark display-5">`
- **Welcome Message**: `<h1 class="display-1"><span class="">Welcome</span>,</h1>`

### About Section

```
<section>
	<div  class="jumbotron bg-dark text-white shadow p-4 mb-4 py-5">
	<!-- About content -->
	</div>
```

</section>

- **Carousel**: `<div id="demo" class="carousel slide" data-bs-ride="carousel">`
  - Indicators: `<div class="carousel-indicators">`
  - Slides: `<div class="carousel-inner shadow-lg p-3 mb-5 bg-body rounded">`
  - Controls: `<button class="carousel-control-prev" type="button" data-bs-target="#demo" data-bs-slide="prev">`

### Accordion

```
<div  class="accordion"  id="accordionExample">
	<!-- Accordion content -->
</div>
```

- **How It Works**: `<div class="accordion-item">`
  - Description: `<div class="accordion-body">`
- **Helps Gamers**: `<div class="accordion-item">`
  - Description: `<div class="accordion-body">`
- **Speed**: `<div class="accordion-item">`
  - Placeholder: `<div class="accordion-body">`

## Conclusion

This document provides a detailed overview of the `home.html` page, including its structure and key components. The page is designed to be responsive and user-friendly, leveraging Bootstrap for styling and layout.

# Register Page Documentation

## Overview

The `register.html` page is a registration form for the Task'd application. It allows users to input their personal information and register for the service. The page is styled using Bootstrap 5.3.2 and includes various form validation feedback.

## Structure

### HTML Document

- **DOCTYPE Declaration**: Specifies the HTML5 document type.
- **HTML Tag**: The root element of the HTML document with `lang="en"` and `data-bs-theme="dark"` attributes.

### Head Section

- **Title**: Sets the title of the page to "Task'd".
- **Meta Tags**: Includes character set and viewport settings for responsive design.
- **Bootstrap CSS**: Links to the Bootstrap 5.3.2 CSS library.

### Body Section

#### Header

- **Navbar**: A dark-themed navigation bar with the Task'd logo and links to the home page and dashboard.
- **Bio Section**: A welcoming message for new users considering joining Task'd.

#### Main

- **Form Container**: Contains the registration form with fields for full name, address, email, and phone number.
  - **Full Name**: Text input for the user's full name with validation feedback.
  - **Address**: Text input for the user's address with validation feedback.
  - **Email**: Email input for the user's email address with validation feedback.
  - **Phone**: Tel input for the user's phone number with a pattern for 10-digit numbers and validation feedback.
- **Buttons**:
  - **Confirm**: A button to confirm registration, linking to the home page.
  - **Continue as Guest**: A button to continue as a guest, linking to the task dashboard.

#### Footer

- **Footer Section**: A dark-themed footer with a copyright notice.

### Scripts

- **Bootstrap JavaScript Libraries**: Links to Popper.js and Bootstrap JavaScript libraries for interactive components.

## Code Snippets

### Navbar

```
<nav  class="navbar navbar-expand-sm bg-dark navbar-dark">
	<div  class="container-fluid">
		<a  class="navbar-brand"  href="#">
			<img  src="/pics/logo.jpg"  alt="img"  style="width:70px;"  class="rounded-pill">
		</a>
		<a  href="home.html"  class="navbar-brand"><span  class="span text-warning">Tas</span>k'd</a>
		<div  class="collapse navbar-collapse"  id="navbarNav">
			<ul  class="navbar-nav ms-auto">
				<li  class="nav-item">
					<a  href="/Pages/home.html"  class="nav-link active"  aria-current="page"></a>
				</li>
				<li  class="nav-item dropdown">
					<a  class="nav-link dropdown-toggle text-white"  href="#"  role="button"  data-bs-toggle="dropdown">
						<span  class="span text-warning">Dash</span>board
					</a>
					<ul  class="dropdown-menu bg-dark">
						<li><a  class="dropdown-item text-white"  href="/Pages/task_dashboard.html">Task'd<span  class="span text-success"> Menu</span></a></li>
						<li><a  class="dropdown-item text-white"  href="/Pages/task_creation.html">Create <span  class="span text-success">Tasks</span></a></li>
					</ul>
				</li>
			</ul>
		</div>
	</div>
</nav>
```

### Registration Form

```
<div  class="container">
	<div  class="mb-3">
		<label  for="Full-name"  class="form-label">Full <span  class="text-success">Name</span></label>
		<input  type="text"  class="form-control"  id="fullname"  name="Full-name"  placeholder="Enter your full name"  />
		<div  class="valid-feedback">Looks good!</div>
		<div  class="invalid-feedback">Please enter a valid name.</div>
	</div>
	<br>
	<div  class="mb-3">
		<label  for="address"  class="form-label"><span  class="text-success">Add</span>ress</label>
		<input  type="text"  class="form-control"  id="address"  name="address"  aria-describedby="addressHelpId"  placeholder="Enter your address"  />
		<div  class="valid-feedback">Looks good!</div>
		<div  class="invalid-feedback">Please enter a valid address.</div>
	</div>
	<br>
	<div  class="mb-3">
		<label  for=""  class="form-label"><span  class="text-success">Em</span>ail</label>
		<input  type="email"  class="form-control"  name="email"  id="email"  aria-describedby="emailHelpId"  placeholder="abc@mail.com"  />
		<div  class="valid-feedback">Looks good!</div>
		<div  class="invalid-feedback">Please enter a valid email address.</div>
	</div>
	<div  class="mb-3">
		<label  for="phone"  class="form-label"><span  class="text-success">Ph</span>one</label>
		<input  type="tel"  class="form-control"  id="phone"  name="phone"  placeholder="Enter your phone number"  pattern="[0-9]{10}">
		<div  class="valid-feedback">Looks good!</div>
		<div  class="invalid-feedback">Please enter a valid 10-digit phone number.</div>
	</div>
	<br>
</div>
<div  class="container text-center">
	<a  name=""  id=""  class="btn btn-success"  href="/Pages/home.html"  role="button">Confirm</a>
	<a  name=""  id=""  class="btn btn-warning"  href="/Pages/task_dashboard.html"  role="button">Continue as guest</a>
</div>
```

### Footer

```
<footer  class="bg-dark text-white text-center py-3">
	<p>© 2024. All rights reserved.</p>
</footer>
```

### Scripts

```
<script  src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.11.8/dist/umd/popper.min.js"  integrity="sha384-I7E8VVD/ismYTF4hNIPjVp/Zjvgyol6VFvRkX/vR+Vc4jQkC+hVqc2pM8ODewa9r"  crossorigin="anonymous"></script>

<script  src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.min.js"  integrity="sha384-BBtl+eGJRgqQAUMxJ7pMwbEyER4l1g+O15P+16Ep7Q9Q+zqX6gSbd85u4mG4QzX+"  crossorigin="anonymous"></script>
```

## Notes

- Ensure that the Bootstrap CSS and JavaScript libraries are correctly linked for proper styling and functionality.
- The form includes basic validation feedback for user inputs.
- The page is designed to be responsive and user-friendly.

# Task'd - Dashboard Documentation

## Overview

This HTML page represents the dashboard for the Task'd application. It provides a user interface for navigating through different game-related tasks and guides.

## Structure

### HTML Document Structure

- **DOCTYPE**: HTML5
- **Language**: English (`lang="en"`)

### Head Section

- **Title**: Task'd - Dashboard
- **Meta Tags**:
  - `charset="utf-8"`
  - `viewport` for responsive design
- **Stylesheets**:
  - Bootstrap CSS v5.3.2
  - Custom stylesheet: `styles/task_dashboard.css`

### Body Section

- **Classes**: `bg-dark` for dark background

#### Header

- **Navigation Bar**:
  - **Brand**: Task'd logo and name
  - **Links**:
    - Home
    - Dashboard (Dropdown)
      - Task'd Menu
      - Create Tasks

#### Main Content

- **Card**: Title card with "Games Dashboard"
- **Container**: Holds the game cards
  - **Row**: Aligns game cards
    - **Columns**: Each column contains a card for a game
      - **Card**: Game card with image and buttons
        - **Buttons**:
          - Achievements and tasks
          - Guide

#### Footer

- **Footer Content**: Copyright information

### Scripts

- **Bootstrap JavaScript Libraries**:
  - Popper.js
  - Bootstrap.js

## Detailed Elements

### Navigation Bar

- **Logo**: Image with rounded-pill class
- **Brand Name**: Task'd with partial text highlighted
- **Dropdown**: Dashboard with links to Task'd Menu and Create Tasks

### Game Cards

- **Card 1**:
  - **Image**: A Short Hike
  - **Buttons**:
    - Achievements and tasks
    - Guide
- **Card 2**:
  - **Image**: Apex Legends
  - **Buttons**:
    - Achievements and tasks
    - Guide
- **Card 3**:
  - **Image**: Placeholder
  - **Button**: Achievements and tasks

### Footer

- **Text**: © 2024. All rights reserved.

## External Resources

- **Bootstrap CSS**: Bootstrap v5.3.2
- **Popper.js**: Popper.js v2.11.8
- **Bootstrap.js**: Bootstrap v5.3.2

## Custom Stylesheet

- **Path**: `styles/task_dashboard.css`

# Task Creation Page Documentation

## Overview

The Task Creation Page allows users to create and manage tasks. It includes a form for entering task details, selecting task categories, and uploading related files.

## HTML Structure

### Head Section

- **DOCTYPE Declaration**: Specifies the HTML version.
- **HTML Tag**: Sets the language attribute to English and the Bootstrap theme to dark.
- **Meta Tags**: Defines character set and viewport settings.
- **Title**: Sets the page title to "Task Creation Page".
- **Stylesheets**: Links to Bootstrap CSS for styling.

### Body Section

#### Header

- **Navigation Bar**:
  - Contains a brand logo and name.
  - Includes links to the home page and a dropdown menu for dashboard options.

#### Main Content

- **Container**:
  - A Bootstrap container with shadow and padding for the form.
  - **Heading**: "Create Tasks" with a text-decoration underline.

#### Form

- **Form Elements**:
  - **Pick Up**: A dropdown to select task types.
  - **Achievement Description**: A textarea for entering achievement descriptions.
  - **Task Name**: An input field for the task name.
  - **Task Description**: A textarea for the task description.
  - **Skill Level**: Checkbox options for selecting skill levels (Beginner, Intermediate, Advanced).
  - **Task Category**: Checkbox options for selecting task categories (Daily Quest, Weekly Quest, VIP's Quest).
  - **Achievement Tokens**: A dropdown to select the number of tokens.
  - **Date Task Was Created**: An input field for the creation date.
  - **Date Task Expires**: An input field for the expiration date.
  - **Task Status**: A dropdown to select the task status (Not Started, In Progress, Completed).
  - **Upload Picture**: A file input for uploading pictures.

#### Modal

- **Create Button**: Triggers a modal for confirmation before saving the task.
- **Modal Content**:
  - **Header**: Displays a warning message.
  - **Body**: Asks for confirmation to save the task.
  - **Footer**: Contains buttons to confirm or cancel the action.

### Scripts

- **Boxicons**: For icon usage.
- **Popper.js**: For Bootstrap tooltips and popovers.
- **Bootstrap JS**: For Bootstrap functionalities.

## External Resources

- **Bootstrap CSS**:
  - Bootstrap 4.5.2
  - Bootstrap 5.3.2
- **Boxicons**: Boxicons
- **Popper.js**: Popper.js
- **Bootstrap JS**: Bootstrap 5.3.2

## Usage

1.  **Navigate** to the Task Creation Page.
2.  **Fill out** the form with the necessary task details.
3.  **Click** the "Create" button to open the confirmation modal.
4.  **Confirm** or **cancel** the task creation in the modal.

## Notes

- Ensure all required fields are filled out before submitting the form.
- The modal provides a final confirmation step to prevent accidental task creation.

## License

# A Short Hike HTML Documentation

## Overview

This HTML document represents a webpage for "Task'd - A Short Hike". It includes a navigation bar, a dropdown menu, and several cards displaying tasks related to the game "A Short Hike".

## Structure

### HTML Document Structure

- `<!DOCTYPE html>`: Defines the document type and version of HTML.
- `<html lang="en">`: Root element of the HTML document with language set to English.
- `<head>`: Contains meta-information about the document.
- `<body>`: Contains the content of the document.

### Head Section

- `<title>`: Sets the title of the webpage.
- Meta tags:
  - `<meta charset="utf-8">`: Sets the character encoding.
  - `<meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">`: Ensures proper rendering and touch zooming on mobile devices.
- CSS Links:
  - Bootstrap CSS from CDN.
  - Custom stylesheet `styles/a_short_hike.css`.

### Body Section

- `<header>`: Contains the navigation bar.
  - `<nav class="navbar navbar-expand-sm bg-dark navbar-dark">`: Bootstrap navbar with dark theme.
  - `<div class="container-fluid">`: Container for the navbar content.
  - `<a class="navbar-brand" href="#">`: Brand logo and link.
  - `<a href="home.html" class="navbar-brand">`: Brand name link.
  - `<div class="collapse navbar-collapse" id="navbarNav">`: Collapsible part of the navbar.
  - `<ul class="navbar-nav ms-auto">`: Navbar items aligned to the right.
    - `<li class="nav-item">`: Individual navbar item.
    - `<li class="nav-item dropdown">`: Dropdown menu item.
      - `<a class="nav-link dropdown-toggle text-white" href="#" role="button" data-bs-toggle="dropdown">`: Dropdown toggle link.
      - `<ul class="dropdown-menu bg-dark">`: Dropdown menu.
        - `<li><a class="dropdown-item text-white" href="/Pages/task_dashboard.html">`: Dropdown item link.
        - `<li><a class="dropdown-item text-white" href="/Pages/task_creation.html">`: Dropdown item link.

### Main Section

- `<main>`: Main content of the page.
  - `<div class="container">`: Container for the dropdown.
    - `<div class="dropdown">`: Dropdown button.
      - `<button class="btn btn-dark dropdown-toggle mt-3 mb-3 form-control fs-3" type="button" id="triggerId" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">`: Dropdown button with image and text.
      - `<div class="dropdown-menu bg-dark form-control text-center" aria-labelledby="triggerId">`: Dropdown menu.
        - `<a class="dropdown-item bg-dark text-light" href="apex_legends.html">`: Dropdown item link.

### Task Cards

- Each task is represented by a Bootstrap card.
  - `<div class="card bg-warning border-dark mb-3">`: Card with yellow background and dark border.
  - `<div class="row g-0">`: Row for card content.
    - `<div class="col-1">`: Column for image.
      - `<img src="..." alt="Image" class="img-fluid border border-dark m-3">`: Task image.
    - `<div class="col-3">`: Column for card body.
      - `<div class="card-body">`: Card body.
        - `<h5 class="card-title">`: Task title.
        - `<p class="card-text">`: Task description.
        - `<p class="card-text">`: Task time and difficulty badge.
    - `<div class="col-2 d-flex align-items-center">`: Column for "Learn More" button.
      - `<div class="card-body">`: Card body.
        - `<a href="..." class="btn btn-primary border border-dark">Learn More</a>`: "Learn More" button.
    - `<div class="col-2 d-flex align-items-center">`: Column for "Mark as Complete" button.
      - `<div class="card-body">`: Card body.
        - `<a href="" class="btn btn-primary border border-dark">Mark as Complete</a>`: "Mark as Complete" button.

## External Resources

- Bootstrap CSS: `https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css`
- Custom CSS: `styles/a_short_hike.css`

## Images

- Various images are used for the tasks, sourced from external URLs.

## Navigation Links

- Home: `home.html`
- Task Dashboard: `/Pages/task_dashboard.html`
- Task Creation: `/Pages/task_creation.html`
- Apex Legends: `apex_legends.html`
- Task Details: `a_short_hike_details.html#<task_id>`

# Documentation for `apex_legends.html`

## Overview

This HTML document is a webpage for "Task'd - Apex Legends". It uses Bootstrap for styling and includes various sections such as a navigation bar, a dropdown menu, and multiple cards displaying different tasks related to the game Apex Legends.

## Structure

### HTML Document Structure

- **DOCTYPE Declaration**: Specifies the HTML5 document type.
- **HTML Tag**: Root element of the document.
- **Head Section**: Contains meta tags, title, and links to stylesheets.
- **Body Section**: Contains the main content of the webpage.

### Head Section

- **Title**: `Task'd - Apex Legends`
- **Meta Tags**:
  - `charset="utf-8"`
  - `name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no"`
- **Stylesheets**:
  - Bootstrap CSS from CDN
  - Custom stylesheet `styles/apex_legends.css`

### Body Section

- **Header**: Contains a navigation bar with branding and links.

  - **Navbar**:
    - Brand logo and name
    - Links to home and dashboard pages
    - Dropdown menu for dashboard options

- **Main Content**:

  - **Dropdown Menu**: Button with an image and text, leading to another game page.
  - **Task Cards**: Multiple cards displaying different tasks related to Apex Legends.

### Task Cards

Each card contains:

- **Image**: Represents the task.
- **Title**: Name of the task.
- **Description**: Brief description of the task.
- **Difficulty**: Badge indicating the difficulty level.
- **Buttons**: Links to learn more about the task or mark it as complete.

## Detailed Breakdown

### Header

```
<header>
	<nav  class="navbar navbar-expand-sm bg-dark navbar-dark">
		<div  class="container-fluid">
			<a  class="navbar-brand"  href="#">
				<img  src="/pics/logo.jpg"  alt="img"  style="width:70px;"  class="rounded-pill">
			</a>
			<a  href="home.html"  class="navbar-brand"><span  class="span text-warning">Tas</span>k'd</a>
			<div  class="collapse navbar-collapse"  id="navbarNav">
				<ul  class="navbar-nav ms-auto">
					<li  class="nav-item">
						<a  href="/Pages/home.html"  class="nav-link active"  aria-current="page"></a>
					</li>
					<li  class="nav-item dropdown">
						<a  class="nav-link dropdown-toggle text-white"  href="#"  role="button"  data-bs-toggle="dropdown">
						<span  class="span text-warning">Dash</span>board
						</a>
						<ul  class="dropdown-menu bg-dark">
							<li><a  class="dropdown-item text-white"  href="/Pages/task_dashboard.html">Task'd<span  class="span text-success"> Menu</span></a></li>
							<li><a  class="dropdown-item text-white"  href="/Pages/task_creation.html">Create <span  class="span text-success">Tasks</span></a></li>
						</ul>
					</li>
				</ul>
			</div>
		</div>
	</nav>
</header>
```

### Main Content

#### Dropdown Menu

```
<div  class="container">
	<div  class="dropdown">
		<button  class="btn btn-dark dropdown-toggle mt-3 mb-3 form-control fs-3"  type="button"  id="triggerId"  data-bs-toggle="dropdown"  aria-haspopup="true"  aria-expanded="false">
			<div  class="row g-0 align-items-center justify-content-center">
				<img  src="https://assets1.ignimgs.com/2019/02/04/apex-legends---button-fin-1549319070496.jpg?fit=bounds&width=188&height=188"  class="img-fluid rounded-2 col-1"  id="dropdownImage"  alt=""  />
				<div  class="h3 col-2 text-decoration-underline"><span  class="text-warning">Apex</span> Legends</div>
			</div>
		</button>
		<div  class="dropdown-menu bg-dark form-control text-center"  aria-labelledby="triggerId">
			<a  class="dropdown-item bg-dark text-light"  href="a_short_hike.html">A Short Hike</a>
		</div>
	</div>
</div>
```

#### Task Cards

```
Each task card follows a similar structure. Below is an example of one card:
<div  class="card bg-warning border-dark mb-3">
	<div  class="row g-0">
		<div  class="col-1">
			<img  src="https://steamuserimages-a.akamaihd.net/ugc/1672486157606558519/64E5EE904A4BF87C39B58F483248C73D735A2123/"  alt="Image"  class="img-fluid border border-dark m-3"  />
		</div>
		<div  class="col-3">
			<div  class="card-body">
				<h5  class="card-title">Apex Assault</h5>
					<p  class="card-text">Win a game as an assault character.</p>
					<p  class="card-text">
					Τ - 5
						<span  class="badge bg-primary ms-2">Intermediate</span>
					</p>
			</div>
		</div>
		<div  class="col-2 d-flex align-items-center">
			<div  class="card-body">
			<a  href="apex_legends_details.html#apexAssault"  class="btn btn-primary border border-dark">Learn More</a>
			</div>
		</div>
		<div  class="col-2 d-flex align-items-center">
			<div  class="card-body">
				<a  href=""  class="btn btn-primary border border-dark">Mark as Complete</a>
			</div>
		</div>
	</div>
</div>
```

## External Resources

- **Bootstrap CSS**: `https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css`
- **Custom Stylesheet**: `styles/apex_legends.css`

# A Short Hike Details Page Documentation

## Overview

This HTML document provides detailed information about various tasks and achievements in the game "A Short Hike". The page is styled using Bootstrap and custom CSS.

## Structure

### Head Section

- **Title**: Task'd - A Short Hike
- **Meta Tags**:
  - Charset: UTF-8
  - Viewport: width=device-width, initial-scale=1, shrink-to-fit=no
- **Stylesheets**:
  - Bootstrap CSS v5.3.2
  - Custom CSS: `styles/a_short_hike_details.css`

### Body Section

- **Header**: Contains a navigation bar with links to the home page and a dropdown menu for the dashboard.
- **Main Content**: Contains multiple cards, each representing a different task or achievement in the game.

## Detailed Breakdown

### Header

- **Navbar**:
  - Brand logo linking to the home page.
  - Navigation links:
    - Home
    - Dashboard (Dropdown)
      - Task'd Menu
      - Create Tasks

### Main Content

#### Hawk Peak Card

- **Image**: A picture representing Hawk Peak.
- **Title**: Hawk Peak
- **Description**: Make it to the top of the mountain.
- **Instructions**: Reach the Peak of the mountain.
- **Tips**:
  - Have at least 7 Golden Feathers to increase stamina.

#### The End Card

- **Image**: A picture representing the end of the game.
- **Title**: The End
- **Description**: Take a nice long nap.
- **Instructions**:
  - Reach Hawk Peak, return to the Rangers Cabin, and interact with it to trigger the end of the game.
- **Tips**:
  - You can continue playing after the end credits.

#### Remember This Day Forever Card

- **Image**: A picture representing the Beachstickball mini-game.
- **Title**: Remember This Day Forever
- **Description**: Successfully hit the ball 30 times in a row while playing Beachstickball.
- **Instructions**:
  - Discover Beachstickball next to the graveyard on the beach.
  - Hit the ball back as many times as possible.
- **Rewards**:
  - 10 hits: Golden Feather
  - 20 hits: Coins
  - 30 hits: Baseball cap and achievement

#### Parkour Master Card

- **Image**: A picture representing the races.
- **Title**: Parkour Master
- **Description**: Beat Avery at least once in all 3 races.
- **Instructions**:
  - Beat Avery twice on each of the 3 circuits.
  - Avery will challenge you near the Visitor Center.
  - Use a limited number of Feathers for each race.
  - Avery will improve after each race.
- **Race Details**:
  - **Race 1**: Start near the Visitor Center, finish at Mountain top, max 9 Feathers.
  - **Race 2**: Start at Royal Ridge, finish at Lighthouse, max 3 Feathers.
  - **Race 3**: Start near the graveyard, finish at Abandoned building, max 5 Feathers.

## Additional Cards

- **Crispy Card**: (Incomplete in the provided context)

## Styles

- **Background**: Dark theme for the body and navbar.
- **Card Themes**:
  - Warning (Yellow) for Hawk Peak and Remember This Day Forever.
  - Success (Green) for The End and Parkour Master.
- **Text Colors**:
  - White text for dark backgrounds.
  - Black text for light backgrounds.

## External Resources

- **Bootstrap CSS**: Bootstrap v5.3.2

## Custom CSS

- **File**: `styles/a_short_hike_details.css`

## Images

- **Source**: External URLs provided in the `src` attribute of `img` tags.

# Documentation for `apex_legends_details.html`

## Overview

This HTML file is a detailed page for the game Apex Legends, showcasing various achievements and their respective instructions and images.

## Structure

### Head Section

- **Title**: `Task'd - Apex Legends`
- **Meta Tags**:
  - Charset: `utf-8`
  - Viewport: `width=device-width, initial-scale=1, shrink-to-fit=no`
- **Stylesheets**:
  - Bootstrap CSS v5.3.2 from CDN
  - Custom stylesheet: `styles/apex_legends_details.css`

### Body Section

- **Class**: `bg-dark`

#### Header

- **Navigation Bar**:
  - **Brand Logo**: Image with `src="/pics/logo.jpg"`
  - **Brand Name**: `Task'd`
  - **Navigation Links**:
    - Home: `home.html`
    - Dashboard Dropdown:
      - Task'd Menu: `/Pages/task_dashboard.html`
      - Create Tasks: `/Pages/task_creation.html`

#### Main Content

- **Container**: Holds the main content cards.

##### Card: Apex Assault

- **Card Class**: `bg-warning border-dark mb-3`
- **Image**: Assault achievement image
- **Title**: `Apex Assault`
- **Description**: Win a game as an assault character.
- **Instructions**: Win a game as one of the assault characters: Ash, Ballistic, Bangalore, Fuse, Mad Maggie, or Revenant.
- **Images**:
  - Ash
  - Ballistic
  - Bangalore
  - Fuse
  - Mad Maggie
  - Revenant

##### Card: Apex Controller

- **Card Class**: `bg-success text-white border-dark mb-3`
- **Image**: Controller achievement image
- **Title**: `Apex Controller`
- **Description**: Win a game as a controller character.
- **Instructions**: Win a game as one of the controller characters: Catalyst, Caustic, Rampart, or Wattson.
- **Images**:
  - Catalyst
  - Caustic
  - Rampart
  - Wattson

##### Card: Apex Legend

- **Card Class**: `bg-warning border-dark mb-3`
- **Image**: Legend achievement image
- **Title**: `Apex Legend`
- **Description**: Win a game with 8 different Legends.
- **Instructions**: For this achievement, only battleroyal (BR) wins count.

## External Resources

- **Bootstrap CSS**: `https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css`
- **Custom CSS**: `styles/apex_legends_details.css`

## Images

- Images are sourced from `steamuserimages-a.akamaihd.net`.
