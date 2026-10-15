# Okiki Website

A responsive starter website built with HTML (HyperText Markup Language), CSS (Cascading Style Sheets), and JavaScript.

## Pages and features

- `index.html`: Home, About, Services, and Contact sections.
- `signup.html`: A demo sign-up form.
- `thank-you.html`: Confirmation page shown after the demo sign-up form is submitted.
- `css/style.css`: Colors, layout, responsive styling, and mobile navigation layout.
- `js/script.js`: Mobile menu, current footer year, demo contact message, and sign-up page redirect.
- The About section picture loads from Unsplash and requires an internet connection.

## Clone and run the project in Visual Studio Code

### 1. Install Git

Git is the version control system used to download the repository and send code changes to GitHub.

1. Open Visual Studio Code (VS Code).
2. Select **Terminal → New Terminal**.
3. Run:

   ```bash
   git --version
   ```

4. If a Git version is shown, continue. If Git is not recognized, install Git for Windows from <https://git-scm.com/download/win>, then restart VS Code.

### 2. Clone the repository

You can clone using the VS Code interface:

1. Press `Ctrl + Shift + P` to open the Command Palette.
2. Search for and select **Git: Clone**.
3. Paste the repository URL:

   ```text
   https://github.com/gODtECH-Ctl-Create/okiki.git
   ```

4. Press Enter and choose a folder on your computer where the project should be saved.
5. When prompted, click **Open** to open the cloned repository in VS Code.

Alternatively, run these commands in the VS Code terminal from the folder where you keep projects:

```bash
git clone https://github.com/gODtECH-Ctl-Create/okiki.git
cd okiki
```

If you use the terminal method, open the folder in VS Code with **File → Open Folder** and select the new `okiki` folder.

### 3. Switch to the website branch

If the website pull request has not yet been merged, the website changes are on the `feat/simple-website` branch. Switch to that branch to get those files:

```bash
git fetch origin
git switch --track origin/feat/simple-website
```

If Git says the local branch already exists, use:

```bash
git switch feat/simple-website
```

Check the current branch:

```bash
git branch --show-current
```

It should show `feat/simple-website` while you are working on that branch. If the pull request has been merged and the changes are on `main`, you can instead use `git switch main` followed by `git pull origin main`.

### 4. Install Live Server

1. In VS Code, press `Ctrl + Shift + X` to open Extensions.
2. Search for **Live Server** by Ritwick Dey.
3. Click **Install**.

### 5. Start the website

1. In the Explorer panel, open `index.html`.
2. Right-click inside the editor.
3. Choose **Open with Live Server**.
4. Your browser should open an address similar to `http://127.0.0.1:5500`.

If that option is not visible, confirm the extension is installed and that you opened the project folder, not just an individual file.

### 6. Test the pages

- Click Home, About, Services, and Contact in the navigation bar.
- Check that the About picture loads. An internet connection is needed for this image.
- Click **Sign Up**, enter dummy test details, and submit the form.
- Confirm the Thank You page opens and its home button returns to the main page.
- Save code changes with `Ctrl + S`. Live Server should refresh the browser automatically.

### 7. Send your changes to GitHub

After editing files, check the working tree:

```bash
git status
```

Stage the changes:

```bash
git add .
```

Create a commit:

```bash
git commit -m "Update Okiki website"
```

Push the current branch to GitHub:

```bash
git push
```

If Git asks you to set the upstream branch on your first push, use:

```bash
git push -u origin feat/simple-website
```

If Git requests authentication, follow the GitHub sign-in prompt. Review your updates on GitHub before merging them into `main`.

## Important: demo forms only

The sign-up form only redirects to the Thank You page. It does not register users, save details, or create accounts. The contact form shows a confirmation in the browser but does not send email or store messages. Do not enter a real password.

For real accounts and secure sign-in, connect an authentication provider or a secure backend. For contact message delivery, connect a server-side form handler or form service. Never store passwords in front-end JavaScript.

## Publish with GitHub Pages

Once the website files are on `main`, open the repository's **Settings → Pages** on GitHub and select the appropriate publishing source. The entry page is at the repository root as `index.html`.
