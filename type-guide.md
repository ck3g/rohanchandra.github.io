---
layout: page
title: "Using Type Theme with Github Pages"
permalink: /project/type/github.html
hide: true
---
Use this guide if you are just getting started with Git (for forking, cloning, committing and pushing changes), Github Pages and/or Jekyll. If you are already familiar with these tools, instead use the [Type Theme documentation](/project/type.html#installing-type-theme).

## Step 1: Get your theme running online

In this step, we'll publish a theme on  [Github Pages](https://pages.github.com/) which allows free hosting from Github repositories and runs Jekyll.

First, visit the [Type Theme repository](https://github.com/rohanchandra/type-theme) on Github, and use the "fork" button to create your own copy of the theme.

![Fork button at the Type Theme repository on Github](/img/project/type/github-fork-btn.png)

Next, rename your repository by clicking the "settings" button in your newly created repository.

![Settings button in a the forked Github repository](/img/project/type/github-settings-btn.png)

Rename the repository to `username.github.io` (replacing "username" with your Github username) to use Github Pages to host your Jekyll website.

![Renaming a repository in the Github settings page](/img/project/type/github-rename-repo.png)

Visit [https://username.github.io](https://username.github.io) (again replacing "username" with your Github username) to see your Jekyll website live!

![Geometric pattern with fading gradient](/img/project/type/github-pages-website.png)

## Step 2: Install Jekyll and Git
*Skip this step if you already have Jekyll and Git installed.*

If you are running Linux or Mac OSX, visit the Jekyll docs for [instructions on installing Jekyll](http://jekyllrb.com/docs/installation/). If you're running Windows visit Julian Thilo's instructions for [installing Jekyll on Windows](http://jekyll-windows.juthilo.com/) as there are a few extra steps.

Also install Git, you may already have Git installed so in Terminal/Bash/Command Prompt type `git --version` to check if Git returns a version number. If not, visit the [Git downloads page](http://www.git-scm.com/downloads) and install Git.

If you prefer to use a GUI, consider also installing a [GUI client for Git](http://www.git-scm.com/downloads/guis). Screenshots will be included for the [Github for Windows](https://windows.github.com/) software (a similar [Mac version](https://mac.github.com/) is also available).

## Step 3: Cloning your repository

![Screenshot of clone URL and button to clone using GUI on Github repository](/img/project/type/github-clone-btn.png)

Create a copy of the repository on your computer by cloning.

To clone, in Terminal/Bash/Command Prompt type (replacing "username" with your own):

`git clone https://github.com/username/username.github.io.git`

Alternatively, if you're using a GUI use the 'clone' feature. Here's what that process in Github for Windows after signing in and selecting the add button:

![Clone button in Github for Windows GUI](/img/project/type/gui-clone.png)

## Step 4: Your first post

Open the `_posts` folder and make new file called "2015-01-01-my-first-post.md". Inside type the contents of your first post. In Jekyll posts are inputted with Markdown.

For example: 

<pre>
---
layout: post
title: My first post
---

Just testing posts in Jekyll
</pre>

To see your changes locally:

1. Save your new post
2. Run the Jekyll server by typing `jekyll serve` in Terminal/Bash/Command Prompt
3. Visit [http://localhost:4000](http://localhost:4000) in your browser view the site

Your new post should be visible on the front page of the theme.

## Step 5: Saving and sharing changes

Once you're happy with your new post, you can commit changes using Terminal/Bash/Command Prompt and push changes to make them public:

1. Add the new files to be tracked, by typing `git add *.md`
2. Commit changes, by typing `git commit -m 'add my first post'`
3. Push changes to the web, by typing `git push origin master`
4. Visit [https://username.github.io](https://username.github.io) to see your changes live

Here's what steps 1 to 3 look in Github for Windows using the GUI instead:

![Commiting changes in Github for Windows by adding title and selecting 'commit to master'](/img/project/type/gui-new-changes.png)

Step 1 and Step 2: Adding files to the commit with a title

![Syncing icon in Github for Windows with progress bar of sync](/img/project/type/gui-sync.png)

Step 3: Syncing in Github for Windows pushes changes to the repository online.

## Step 5: Customising Type Theme

Now that you've got Type Theme running, know how to make posts, preview Jekyll websites locally using `jekyll serve`, and save changes using "git push" or syncing in the GUI, you'll want to make some finishing touches to customise the theme.

The most important changes to make are:

1. Update the site configuration in `_config.yml` to match the URL your Jekyll website is hosted on (such as `https://username.github.io`)
2. Update your title in `_config.yml` to rename your Jekyll blog
3. Update social icons to match your own usernames

All the above changes are made by opening the `_config.yml` file in a text editor. Please visit the [Type Theme documentation](/project/type.html#customizing-type-theme) for the complete details on customising the theme with examples of configuration.
