# Ryan Eric Angelo — Personal Starter Site

This repository is a lightweight starter for a personal static website for Ryan Eric Angelo. It contains a single-file static page (`index.html`) with a minimal, responsive design and optional links you can customize.

## Project structure

```text
.github/
├── workflows/
│   └── static.yml      # (optional) GitHub Actions workflow to deploy to GitHub Pages
index.html               # Main static page
```

### index.html

Open `index.html` and update the visible name, links, or copy to personalize the site. The file uses simple, modern CSS and respects the user's color-scheme preference.

## Deployment

This project can be hosted on GitHub Pages. If the repository includes `.github/workflows/static.yml`, pushing to the `main` branch will trigger the workflow and publish the site.

## Local development / Preview

Quick ways to preview locally:

- Open `index.html` directly in a browser.
- Or run a tiny HTTP server from the repo root:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## How to customize

1. Edit `index.html` to change the name, links, or styles.
2. Commit and push your changes to `main` (or your chosen branch).
3. If using GitHub Pages + Actions, the site will be deployed automatically on push.

## Simple edits for beginners

If you're new to websites, here are a few very small, safe edits you can make in `index.html`.

1. Add or edit links

- Open `index.html` in a text editor. Look for a commented block that looks like this:

<!-- <div class="links">
			<a href="https://blog.mankoo.ca" class="link">Blog</a>
			<a href="https://www.linkedin.com/in/sumeetsinghmankoo/" class="link">LinkedIn</a>
		</div> -->

- To make the links visible on the page, remove the `<!--` at the start and the `-->` at the end. Then change each `href` to the web address you want and change the link text (the words between `>` and `</a>`).

  Example (after uncommenting and editing):

  <div class="links">
  	<a href="https://yourblog.example" class="link">Blog</a>
  	<a href="https://www.linkedin.com/in/yourprofile/" class="link">LinkedIn</a>
  </div>

  Save the file and refresh the page in your browser to see the links.

2. Change the name shown on the page

- At the top of `index.html` you'll see an `h1` element, for example `<h1>Ryan Eric Angelo</h1>`.
- Edit the text between `<h1>` and `</h1>` to change the displayed name, then save and refresh.

3. Change colors (very small tweak)

- In the `<style>` section near the top of `index.html` there are CSS variables inside `:root` like `--accent-color`.
- Change `--accent-color: #3d5afe;` to another hex color (for example `#ff6b6b`) and save to see a different accent color for links and hover effects.

4. Preview locally (two easy ways)

- Easiest: double-click `index.html` to open it in your browser.
- Slightly more advanced (recommended): from the project folder run `python3 -m http.server 8000` and visit `http://localhost:8000`.

5. Publish (very short)

- If this repository is on GitHub and already set up with a workflow in `.github/workflows/static.yml`, pushing to `main` will usually publish the site to GitHub Pages automatically.
- If you're unsure, I can help set up GitHub Pages or walk you through the steps.

Tip: before making edits, you can make a copy of `index.html` (e.g., `index.html.bak`) so you can restore it if something looks off.

## Notes

- The layout is intentionally minimal so it's easy to fork and extend.
- If you add more pages, update the workflow (if present) to include them in the deployed site.

## Author

Ryan Eric Angelo
