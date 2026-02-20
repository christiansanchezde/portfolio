# R&D Engineer Portfolio

A minimalist, dark-mode portfolio theme built for Software Engineers and Researchers. This site is built using **Jekyll** and hosted on **GitHub Pages**.

It features a custom CSS Grid layout, overriding the default Jekyll 'Architect' theme to provide a modern, sidebar-based navigation and a "Terminal/IDE" aesthetic.

## 🚀 Tech Stack

*   **Static Site Generator:** Jekyll
*   **Templating:** Liquid
*   **Styling:** CSS3 (Grid, Flexbox, CSS Variables)
*   **Font:** Inter (Body) & JetBrains Mono (Headers/Code)
*   **Data Management:** YAML (`_data/projects.yml`)

## 📂 Project Structure

*   `_data/projects.yml`: Centralized list of projects (Name, Description, Tech Stack, URL).
*   `_layouts/default.html`: The main HTML skeleton implementing the sidebar layout.
*   `assets/css/style.css`: Custom dark mode styling and responsive overrides.
*   `index.md`: The main content page (About, Skills, Publications).

## 🛠 Local Development

You can run this site locally using either Ruby or Docker.

### Option 1: Native Ruby (Standard)

1.  **Prerequisites:** Ensure you have Ruby and Bundler installed.
2.  **Install dependencies:**
    ```bash
    bundle install
    ```
3.  **Serve the site:**
    ```bash
    bundle exec jekyll serve
    ```
4.  Open `http://localhost:4000` in your browser.

### Option 2: Docker (Cleanest Method)

If you don't want to install Ruby on your machine, you can run the site in a container.

1.  **Run the command:**
    ```bash
    docker run --rm \
      --volume="$PWD:/srv/jekyll" \
      -p 4000:4000 \
      jekyll/jekyll \
      jekyll serve
    ```
    *(**Windows Users:** If using PowerShell, replace `$PWD` with `${PWD}`)*.

2.  Open `http://localhost:4000` in your browser.

## 🎨 Customization

1.  **Profile Info:** Edit `_config.yml` to change your name, email, and social links.
2.  **Projects:** Add or remove entries in `_data/projects.yml`.
3.  **Content:** Edit `index.md` to update your Bio, Skills, or Publications.
