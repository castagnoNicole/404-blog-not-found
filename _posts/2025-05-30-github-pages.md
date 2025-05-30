---
title: "How to Create a Blog with GitHub Pages"
categories:
  - Blog
tags:
  - GitHub Pages
  - Jekyll
  - markdown
---
Ever wanted to start your own blog without paying for hosting or dealing with complex setups? 
GitHub Pages is a free and easy way to publish your blog online. Here’s a step-by-step guide to get you started—even if you’re new to coding or web development.

## What is GitHub Pages?
GitHub Pages lets you host static websites straight from a GitHub repository. It’s free, integrates with your GitHub account, and is perfect for blogs, portfolios, or project sites. Most GitHub Pages blogs use Jekyll, a static site generator that turns simple Markdown files into a full-featured website.

### Step 1: Create a GitHub Account
If you don’t have a GitHub account yet, sign up at github.com. 
Your username will become part of your blog’s URL, so choose something you like.

### Step 2: Create a Repository for Your Blog
- Log in to GitHub.
- Click the `+` icon in the upper right and select `New repository`.
- Name your repository with the title of your blog.
- Set the repository to Public

### Step 3: Enable GitHub Pages
- Go to your new repository’s Settings.
- In the sidebar, click Pages under “Code and automation.”
- Under Build and deployment, choose Deploy from a branch.
- Select the branch you want to publish. Every time you commit on that branch Github will re-deploy the website.
- Save your settings.

Your site will be live at `https://yourusername.github.io/blog-title` after a few minutes.

### Step 4: Add Your Blog Content
Most GitHub Pages blogs use Jekyll, which works with Markdown files. You can:
- Add blog posts by creating files in the `_posts` directory.
- Each post should be named like `YYYY-MM-DD-title.md`.
  - (e.g., 2025-05-30-my-first-post.md).
- Write your posts in Markdown, which is simple to learn and great for formatting text, code, and images.

### Step 5: Customize Your Blog
- Pick a Jekyll theme to change the look and feel. You can find themes on the Jekyll Themes site. *I'm using Minimal mistakes*
- Edit the `_config.yml` file to change your blog’s title, description, and settings.

### Step 6: Publish and Update
Every time you push changes to your repository (add posts, edit content, etc.), GitHub Pages automatically rebuilds and updates your blog.
You can preview your changes locally if you install Jekyll, but for most users, editing directly on GitHub is enough.

**Small tip** If you want to know the status of deployment go to: `https://github.com/your-username/blog-title/deployments` or click on "Deployments" (see picture below)
{: .notice--success} 

![alt]({{ site.url }}{{ site.baseurl }}/assets/images/deployments.png)
{: .half}

## Why I chose GitHub Pages for my blog?
- Free hosting — no ads or hidden costs.
- Easy to update — just push to GitHub.
- No server maintenance — focus on writing, not sysadmin tasks.
