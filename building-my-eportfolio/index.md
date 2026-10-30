---
layout: single
title: "Building my E-Portfolio"
permalink: /building-my-eportfolio/
author_profile: true
toc: true
toc_label: "Guide Contents"
---
## 1. Documenting How I Built My E-Portfolio
### Introduction
I created this e-portfolio to showcase my education, professional experience, skills, and academic projects in supply chain management and analytics. This guide explains how I built and customized my website using GitHub Pages.

### Set Up My GitHub Repository
#### GitHub Account
I created a GitHub account, JohanLacea, to manage the files for my e-portfolio.
#### Portfolio Repository
My portfolio repository is named JohanLacea.github.io. This repository contains the files used to build the website, set up the theme, and images.  
[View my GitHub Repository](https://github.com/JohanLacea/JohanLacea.github.io)

### Adding and Updating Theme
#### I started with the Minimal Theme
I initially built my e-portfolio using the Minimal theme:

1. Open [Minimal theme](https://github.com/pages-themes/minimal)
2. Click **Code**, then **Download ZIP** to download the theme files.
![Minimal download screenshot](/assets/img/Minimal.png)
3. Extract the downloaded ZIP file.
4. Copy the extracted theme files and folders to existing local repository, in my case [JohanLacea.github.io](https://github.com/JohanLacea/JohanLacea.github.io).
5. Click **Commit Changes** and push them to GitHub.
6. Visit the portfolio to check that the theme has published correctly.

#### Switching to Minimal Mistakes Theme
After building the initial portfolio with Minimal, I switched to Minimal Mistakes. I used the theme documentation to guide the transfer into my existing repository and then personalized the settings.

1. Open the [Minimal Mistakes repository](https://github.com/mmistakes/minimal-mistakes)
2. Click **Code**, then **Download ZIP** to download the theme files, and extract them.
3. Review the [Quick-Start Guide](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/), including **Remove the Unnecessary**, to select the files and folders to transfer into the existing repository. Keep the portfolio content and images.
4. Follow the steps in the [To install as a remote them:](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/#remote-theme-method)
In `_config.yml`, activate the remote theme and choose the color scheme:

   ```yaml
   # theme: "minimal-mistakes-jekyll"
   remote_theme: "mmistakes/minimal-mistakes@4.28.1"
   minimal_mistakes_skin: "mint"
   ```

   The remote theme setting loads the specified version from GitHub. The alternative `theme` line stays commented out, and `mint` selects the green color scheme. Keep the required `jekyll-include-cache` entry in the existing `plugins` list.
   ![Quick start screenshot](/assets/img/Quick_Start.png)
5. Personalize the site title, masthead heading, and author information in `_config.yml`. I added my name, profile image, biography, and location.
6. Update the settings at the top of `index.md`:
   
      ```yaml
      ---
      layout: single
      title: false
      author_profile: true
      toc: true
      toc_label: "Table of Contents"
      toc_icon: "cog"
      header:
        image: /assets/img/header.jpg
      ---
      ```
      These settings select the single layout, hide the automatic page title, display the author sidebar, enable a table of contents, and add my homepage banner. Below these settings, I used Markdown headings, paragraphs, and bullet points to organize my professional summary, professional experience, education, certifications, and LinkedIn link.
      
      It should look similar to this:
      ![Screenshot of index](/assets/img/Index.png)
7. Commit and push the changes to GitHub, then check the published portfolio's appearance, content, and links.

Here is a screenshot of my e-portfolio:
![Profile screenshot](/assets/img/Profile.png)

## 2. Creating the Guide Subpage
1. Create a folder in the repository, I named mine `building-my-eportfolio`, and add an `index.md` file inside it.
2. Add these settings at the top to define the title, address, layout, author sidebar, and table of contents:

   ```yaml
   ---
   layout: single
   title: "Building my E-Portfolio"
   permalink: /building-my-eportfolio/
   author_profile: true
   toc: true
   toc_label: "Guide Contents"
   ---
   ```
3. Write the guide below the settings, including instructions and screenshots. Commit and push the changes, then check the published page.

## 3. Linking the Guide from My Homepage
1. Open the homepage `index.md` in the main repository directory.
2. After adding a **Projects** section, add this to the existing homepage:

```markdown
* [E-Portfolio Guide](/building-my-eportfolio/)
```
3. Commit and push the changes, then test the link on the published homepage. 