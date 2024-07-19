# Setting up Hugo and deploying on Vercel

This guide will walk you through the process of setting up a Hugo site and deploying it on Vercel, using the sample content from the [hugo-template](https://github.com/bsidio/hugo-template) repo and the [hugo-coder](https://themes.gohugo.io/themes/hugo-coder/) theme.

## Prerequisites

- [Node.js](https://nodejs.org/) installed on your machine
- [Homebrew](https://brew.sh/) installed (for macOS users)
- A [GitHub](https://github.com/) account
- [Git](https://git-scm.com/) installed on your machine

## Installation

1. Install the Vercel CLI globally:
   ```
   npm i -g vercel
   ```

2. Log in to Vercel using your GitHub account:
   ```
   vercel login --github
   ```

3. Install Hugo using Homebrew (for macOS users):
   ```
   brew install hugo
   ```

## Setup

1. Clone the hugo-template repo:
   ```
   git clone https://github.com/bsidio/hugo-template.git
   ```

2. Navigate to the cloned directory:
   ```
   cd hugo-template
   ```


3.1 Add the hugo-coder theme as a Git submodule:

   ```
   git submodule update --init --recursive

   ```
   To add new theme
   ```
   git submodule add https://github.com/luizdepra/hugo-coder.git themes/hugo-coder
   ```

4. Edit the `hugo.toml` file and set the `theme` property to `"hugo-coder"`:
   ```toml
   theme = 'hugo-coder'
   ```

5. Create a new content file:
   ```
   hugo new content/about.md
   ```

6. Start the Hugo server with drafts enabled:
   ```
   hugo server --buildDrafts
   ```

7. Open your browser and navigate to `http://localhost:1313` to see your site.

## Deploying on Vercel

1. Initialize your Hugo site as a Git repository (if not already done):
   ```
   git init
   ```

2. Add and commit your changes:
   ```
   git add .
   git commit -m "Initial commit"
   ```

3. Deploy your site to Vercel:
   ```
   vercel
   ```

   Follow the prompts to configure your deployment settings.

4. Once the deployment is complete, you'll receive a URL where your site is live.

That's it! You've successfully set up a Hugo site with the hugo-coder theme and deployed it on Vercel using the sample content from the hugo-template repo.