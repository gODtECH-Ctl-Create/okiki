# My Okiki Website Project

## Introduction

In this project, I created a small website called **Okiki** using HTML (HyperText Markup Language) and a little CSS (Cascading Style Sheets). I kept the code simple so a beginner can read it and understand how a basic website works.

The website has a Home section, About section, Services section, Contact section, a Sign Up page, and a Thank You page.

## Files I created

- `index.html` contains the main website.
- `signup.html` contains the sign-up form.
- `thank-you.html` contains the message shown after the form is submitted.

## How I built the website

### 1. I started with the basic HTML structure

Each HTML page starts with this structure:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Okiki</title>
</head>
<body>
  <!-- Page content goes here -->
</body>
</html>
```

- `<!DOCTYPE html>` tells the browser that this is an HTML5 document.
- `<html lang="en">` says the page language is English.
- `<head>` contains page information that is not displayed as the main page content.
- `<meta charset="UTF-8">` helps the browser display text correctly.
- The viewport setting helps the page fit phone and computer screens.
- `<title>` sets the text shown on the browser tab.
- `<body>` contains the visible page content.

### 2. I added the navigation bar

In `index.html`, I used links inside a `<nav>` element:

```html
<nav>
  <a href="#home">Home</a>
  <a href="#about">About</a>
  <a href="#services">Services</a>
  <a href="#contact">Contact</a>
  <a href="signup.html">Sign Up</a>
</nav>
```

The links beginning with `#` move the visitor to a section on the same page. For example, `href="#about"` moves to the section with `id="about"`.

The Sign Up link is different because `href="signup.html"` opens another HTML file.

### 3. I created the sections on the home page

I used headings and paragraphs to add content. For example:

```html
<section id="home">
  <h1>Welcome to Okiki</h1>
  <p>A simple place to find helpful services and support.</p>
  <a href="signup.html">Get Started</a>
</section>
```

- `<section>` groups related content together.
- `id="home"` gives the section a name that the navigation link can find.
- `<h1>` is the main heading.
- `<p>` is a paragraph.
- `<a>` creates a link.

I repeated this idea for the About, Services, and Contact sections.

### 4. I added a picture to the About section

I used an image element:

```html
<img
  src="https://images.unsplash.com/photo-1521737711867-e3b97375f902?auto=format&fit=crop&w=600&q=80"
  alt="People working together">
```

The `src` attribute tells the browser where to find the image. The `alt` attribute describes the image for people who cannot see it and for situations where the picture does not load. The picture is hosted online, so the browser needs an internet connection to load it.

### 5. I added a small amount of CSS

I placed the CSS inside the `<style>` element in the `<head>` of `index.html`. CSS changes how the page looks.

For example:

```css
body {
  font-family: Arial, sans-serif;
  margin: 0;
  line-height: 1.6;
}
```

- `font-family` chooses the text style.
- `margin: 0` removes the browser's default outside space around the page.
- `line-height` adds space between lines of text.

I also used CSS to give the navigation bar a light background, add space around sections, limit the width of the picture, and make the Sign Up links look like simple buttons. I kept the design basic on purpose.

### 6. I created the sign-up form

In `signup.html`, I added a form with a name field, an email field, and a button:

```html
<form onsubmit="event.preventDefault(); window.location.href='thank-you.html';">
  <p><label>Name: <input type="text" required></label></p>
  <p><label>Email: <input type="email" required></label></p>
  <button type="submit">Sign Up</button>
</form>
```

- `<form>` groups the fields together.
- `<label>` describes each field.
- `type="text"` lets someone enter their name.
- `type="email"` asks the browser to check that the email looks like an email address.
- `required` means the field must be filled before the form can be submitted.
- `type="submit"` makes the button submit the form.

The `onsubmit` instruction is a small piece of JavaScript (the language used to add behavior to a web page). `event.preventDefault()` stops the browser from submitting the form in its normal way. `window.location.href='thank-you.html'` then opens the Thank You page.

### 7. I created the Thank You page

In `thank-you.html`, I used a heading, a paragraph, and a link:

```html
<h1>Thank you very much!</h1>
<p>Thanks for visiting Okiki.</p>
<a href="index.html">Back to Home</a>
```

This page confirms that the demo form was submitted and gives the visitor a way to return to the home page.

## What I learned

I learned how to make a web page with headings, paragraphs, links, pictures, and a form. I also learned how a navigation link connects to a section, how simple CSS changes the look of a page, and how a form can open another page.

