# Static-Webpage
A static Webpage using HTML

## How to Use

1. **Upload the Code**: Save the provided HTML code as `index.html` and open it in a web browser to view the static web page.
2. **Customize Content**: Modify the HTML file to update content, links, and images as needed.

## Installation

1. **Create the HTML File**:
   - Save the provided HTML code as `index.html` in your project directory.
2. **Open in Browser**:
   - Open `index.html` in any web browser to view the web page.

## Project Structure

### HTML

The HTML file includes the following sections:

- **Header**: Contains the site logo and navigation links.
- **Main Content**:
  - **Intro Section**: Features a background image, heading, introductory text, and a call-to-action button.
  - **Blogpage Section**: Displays information about posts, genres, and interests with icons.
  - **About Me Section**: Contains a brief description and an image.
- **Footer**:
  - **Copy Section**: Copyright notice.
  - **Bottom Links Section**: Additional navigation and social media links.
  - **Pagination Links**: Links for navigating to previous and next pages.

### CSS

The embedded CSS styles are used to:

- Define the layout and appearance of various sections including the header, main content, and footer.
- Apply styling to text, buttons, and icons.

### Dependencies

- **Font Awesome**: Used for icons. Included via a CDN link.
- **Google Fonts**: Used for custom fonts. Included via a CDN link.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.

## Notes

- Ensure that all linked resources (e.g., images, other HTML files) are correctly placed in the specified directory paths.
- Modify the links in the `href` attributes of the anchor tags as needed for your file structure.

## Example Code

Here’s the provided HTML code:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Your Part-time Writer</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Sriracha&display=swap'); 

    body {
      margin: 0;
      box-sizing: border-box;
    }

    .header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      background-color: #f8f8ff;
    }

    .header .logo {
      font-size: 25px;
      font-family: 'Sriracha', cursive;
      color: #000;
      text-decoration: none;
      margin-left: 30px;
    }

    .nav-items {
      display: flex;
      justify-content: space-around;
      align-items: center;
      background-color: #f8f8ff;
      margin-right: 25px;
    }

    .nav-items a {
      text-decoration: none;
      color: #000;
      padding: 35px 20px;
    }

    .intro {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      width: 100%;
      height: 520px;
      background: linear-gradient(to bottom, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.5) 100%), url("https://cdn.wallpapersafari.com/69/12/NoPsgv.jpeg");
      background-size: cover;
      background-position: center;
      background-repeat: no-repeat;
    }

    .intro h1 {
      font-family: sans-serif;
      font-size: 50px;
      color: #fff;
      font-weight: bold;
      text-transform: uppercase;
      margin: 0;
    }

    .intro p {
      font-size: 20px;
      color: #b5b5b5;
      text-transform: uppercase;
      margin: 20px 0;
    }

    .intro button {
      background-color: #ff3300;
      color: #000;
      padding: 10px 25px;
      border: none;
      border-radius: 5px;
      font-size: 20px;
      font-weight: bold;
      cursor: pointer;
      box-shadow: 0px 0px 20px rgba(255, 255, 255, 0.4)
    }

    .blogpage {
      display: flex;
      justify-content: space-around;
      align-items: center;
      padding: 40px 80px;
    }

    .blogpage .work {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      padding: 0 40px;
    }

    .blogpage .work i {
      width: fit-content;
      font-size: 50px;
      color: #333333;
      border-radius: 50%;
      border: 2px solid #333333;
      padding: 12px;
    }

    .blogpage .work .work-heading {
      font-size: 20px;
      color: #333333;
      text-transform: uppercase;
      margin: 10px 0;
    }

    .blogpage .work .work-text {
      font-size: 15px;
      color: #6C6463;
      margin: 10px 0;
    }

    .about-me {
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 40px 80px;
      border-top: 2px solid #eeeeee;
    }

    .about-me img {
      width: 500px;
      max-width: 100%;
      height: auto;
      border-radius: 10px;
    }

    .about-me-text h2 {
      font-size: 30px;
      color: #333333;
      text-transform: uppercase;
      margin: 0;
    }

    .about-me-text p {
      font-size: 15px;
      color: #6C6463;
      margin: 10px 0;
    }

    .footer {
      display: flex;
      justify-content: space-between;
      align-items: center;
      background-color: #302f49;
      padding: 40px 80px;
    }

    .footer .copy {
      color: #fff;
    }

    .bottom-links {
      display: flex;
      justify-content: space-around;
      align-items: center;
      padding: 40px 0;
    }

    .bottom-links .links {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      padding: 0 40px;
    }

    .bottom-links .links span {
      font-size: 20px;
      color: #fff;
      text-transform: uppercase;
      margin: 10px 0;
    }

    .bottom-links .links a {
      text-decoration: none;
      color: #a1a1a1;
      padding: 10px 20px;
    }

a { text-decoration: none; display: inline-block; padding: 8px 16px; } 
a:hover { background-color: #ddd; color: black; } 
.previous { background-color: #f1f1f1; color: black; } 
.next { background-color: #04AA6D; color: white; } 
.round { border-radius: 50%; }
  </style>
</head>

<body>
  <header class="header">                                                                                                                                              
    <a href="#" class="logo">Random Scribbler</a>
    <nav class="nav-items">
      <a href="E:\HTML\RandomScribbler.html">Home</a>
      <a href="E:\HTML\about me.html">About</a>
      <a href="E:\HTML\Contact Me.html">Contact</a>
    </nav>
  </header>
  <main>
    <div class="intro">
      <h1>A Random scribbler</h1>
      <p>I'm a part-time writer.Love to share my life experience with others.</p>
      <button>Learn More</button>
    </div>
    <div class="blogpage">
      <div class="work">
        <i class="fas fa-book"></i>
        <p class="work-heading">Posts</p>
        <p class="work-text">I have worked on many projects and I am very proud of them. I am a very good developer and I am always looking for new projects.</p>
      </div>
      <div class="work">
        <i class="fas fa-anchor"></i>
        <p class="work-heading">Genres</p>
        <p class="work-text">I write under several niches.Not only some random topic, but also benificial/helpful topics in day-to-day life.</p>
      </div>
      <div class="work">
        <i class="fas fa-beer"></i>
        <p class="work-heading">Interests</p>
        <p class="work-text">I personally don't wanted to share this thing,but for the record I would love to write stories and do some phootography. </p>
      </div>
    </div>
    <div class="about-me">
      <div class="about-me-text">
        <h2>About Me</h2>
        <p>I am part-time writer as you all know. I staretd it as a hobby. But now,  you guys became family.Now, I would like to write for you guys.</p>
      </div>
      <img src="E:\HTML\bennefalls11.jpeg" alt="me" width="104" height="125">
    </div>
  </main>
  <footer class="footer">
    <div class="copy">&copy; 2023 Copyrights</div>
    <div class="bottom-links">
      <div class="links">
        <span>More Info</span>
        <a href="E:\HTML\RandomScribbler.html">Home</a>
        <a href="E:\HTML\about me.html">About</a>
        <a href="E:\HTML\Contact Me.html">Contact</a>
      </div>
      <div class="links">
        <span>Social Links</span>
        <a href="https://www.facebook.com/"><i class="fab fa-facebook"></i></a>
        <a href="https://twitter.com/?lang=en-in"><i class="fab fa-twitter"></i></a>
        <a href="https://www.instagram.com/accounts/emailsignup"><i class="fab fa-instagram"></i></a>
      </div>
    </div>
	<div>
<a href="#" class="previous">&laquo; Previous</a>
<a href="E:\HTML\RSpage1.html" class="next">Next &raquo;</a>

<a href="#" class="previous round">&#8249;</a>
<a href="E:\HTML\RSpage1.html" class="next round">&#8250;</a>
</div>
  </footer>
</body>

</html>
```
