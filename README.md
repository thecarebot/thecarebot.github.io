[The Carebot blog](https://thecarebot.github.io/)

### Setup

1. Clone this repo to your local machine: 
`git clone https://github.com/yourusername/yourusername.github.io.git` 

2. Establishe a virtual environment (not necessary, but nice in case you want to try something out):
`mkvirtualenv carebot-site`

3. Open the directory. You are ready to go.
`cd carebot-site`

### Publishing New Blog Post

1. Create a new file under `_posts`. 

2. Ensure the first lines of the file contain
```
	---
	layout: post
	title: The Tile Of Your Post Goes Here
    date: YYYY-MM-DD HH:MM:SS -0400
	---
```

Note: Use 24-hour formatting for times (i.e.: 16:00 for 4pm). The portion at the end of the date is the [timezone](https://www.timeanddate.com/time/zone/usa/washington-dc). 

3. Save the file following the same naming convention as other files `YYYY-MM-DD-tile-of-post.md`

4. `git add .` to add the file you changed. 

5. `git commit -m "your commit message here"` to indicate what you are publishing or changing

6. `git push` to push the new post to [The Carebot blog](https://thecarebot.github.io/)

### Running a local server for this blog

If you want to preview the blog before going live, follow these instructions. Complete the above **setup instructions** first.

1. Run `sudo gem install github-pages` to install Jekyll and plug-ins in one fell swoop. This mirrors the plug-ins used by GitHub Pages on your local machine including Jekyll, Sass, etc. This will allow you to reliably see the same thing you'd see on the live site.

2. Run `jekyll serve` to serve the site.

3. View the local site at [http://127.0.0.1:4000](http://127.0.0.1:4000)

Note on working locally: The site uses web fonts, which will not load if you are working offline. Even when working locally, the local site will look for web fonts in a remote URL.

***

Note: In the event this is not self-evident, only people authorized to change this repo can publish blog posts. 