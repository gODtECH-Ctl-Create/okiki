# Okiki Website

A very simple website made with HTML (HyperText Markup Language) and a little CSS (Cascading Style Sheets).

## Files

- `index.html`: Home, About, Services, and Contact.
- `signup.html`: Demo sign-up form.
- `thank-you.html`: Thank-you page.

## First-time setup in VS Code

1. Install Git from <https://git-scm.com/download/win> if it is not already installed.
2. Open Visual Studio Code (VS Code) and press `Ctrl + Shift + P`.
3. Choose **Git: Clone** and enter:

   ```text
   https://github.com/gODtECH-Ctl-Create/okiki.git
   ```

4. Choose a folder on your computer, then click **Open** when cloning finishes.
5. Install the **Live Server** extension by Ritwick Dey.
6. Open `index.html`, right-click inside the editor, and choose **Open with Live Server**.

## Update your local copy

Use these steps whenever you want to download the latest version of the website from GitHub.

1. Open your existing `okiki` folder in VS Code.
2. Save any changes you want to keep. If you have local edits that are not committed, commit them or back them up before pulling.
3. Choose **Terminal → New Terminal**.
4. Run the following commands one at a time:

   ```bash
   git switch main
   git pull origin main
   ```

5. Your local files now include the latest changes from the GitHub `main` branch. If Live Server is running, check your browser; otherwise open `index.html` and select **Open with Live Server** again.

**Important:** Run `git pull origin main` inside the terminal with the current directory set to your cloned `okiki` project folder. Do not clone the repository again every time you want an update.

## Edit the website locally

- Edit `index.html` to change the page text, links, picture, or sections.
- Edit `signup.html` to change the sign-up form.
- Edit `thank-you.html` to change the thank-you message.
- Press `Ctrl + S` to save. Live Server should refresh the browser automatically.

## Send your local changes to GitHub

After editing and saving your files, run these commands in the VS Code terminal:

```bash
git status
git add .
git commit -m "Update website content"
git push origin main
```

These commands show your changed files, stage your changes, create a commit, and push the commit to GitHub. Only push directly to `main` if that is how you want to work and your repository allows it. If you prefer using a branch and pull request, create a branch before editing and push that branch instead.

If Git asks you to sign in, follow the GitHub authentication prompts. If `git pull` reports a conflict, resolve the marked files first and then commit the resolution.

## Test it

Click Home, About, Services, and Contact. Choose **Sign Up** and submit dummy details to see the thank-you page.

The sign-up form does not create accounts or save details. The contact email in the page is a placeholder. Replace it with your own contact email.
