# Okiki Website

A responsive starter website built with HTML (HyperText Markup Language), CSS (Cascading Style Sheets), and JavaScript.

## Pages and features

- `index.html`: Home, About, Services, and Contact sections.
- `signup.html`: A demo sign-up form.
- `thank-you.html`: Confirmation page shown after the demo sign-up form is submitted.
- `css/style.css`: Colors, layout, responsive styling, and mobile navigation layout.
- `js/script.js`: Mobile menu, current footer year, demo contact message, and sign-up page redirect.
- About section image loads from Unsplash and requires an internet connection.

## Run it in Visual Studio Code

1. Clone or download this repository.
2. Open the repository folder in Visual Studio Code (VS Code).
3. Install the **Live Server** extension by Ritwick Dey if needed.
4. Open `index.html`, right-click in the editor, and select **Open with Live Server**.
5. Test the navigation, contact form, and sign-up-to-thank-you flow.

You can also open `index.html` directly in a browser, but Live Server is more convenient while editing.

## Important: demo forms only

The sign-up form does not register users, store details, or create real accounts. The contact form does not send email or store messages. The password field is only included to demonstrate a form layout. Do not enter a real password.

For real accounts, secure sign-in, and message delivery, connect an authentication provider or backend and a server-side form handler. Never store passwords in front-end JavaScript.

## Publish with GitHub Pages

After the code has been merged into `main`, open the repository's **Settings → Pages** on GitHub and choose the publishing source available for the repository. The entry page is at the repository root as `index.html`.