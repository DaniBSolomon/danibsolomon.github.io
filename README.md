# A website for danielle

## setup

so!!!!!! to set up your site, fork this [repository](https://github.com/nathanwentworth/danielle) (button at the top left) and then go into settings and rename it to `yourusername.github.io` (so like, daniellesolomon.github.io or whatever your username is!), then scroll down and under "github pages" click on the source dropdown and select master and save. then your site *should* be live under the url that it shows if everything goes well!

## config

now, the first thing you'll wanna edit is your _config.yml file! that contains lots of variables that affect things about your site. first, change title to whatever you want. navpages should be the pages you want to link to! that's in the format of "Title of Link": "url/to/link/to". if you want it to be a local page, such as your /about/ page, just put the word "about". if you want it to be an external url, like "https://google.com", then put the full url, including the http(s) part. then, change the actual /img/social.jpg to be something else! this will be displayed when you share your site on social media and stuff (like in those fancy twitter cards, or when you share a site in facebook messenger). this can be kinda anything. i'd recommend just doing an illustration you really like that you've made! 

if you want to change site styles, there's some basics in there! so you can change background color, text color, and link color. you can also change how rounded the corners of things are, and the max width of the site. 

## posts

once you've done that, you're going to want to look at the _illustration and _games folders! those contain your "posts". if you want to make a new game entry i highly recommend just copy and pasting the content that it's in one already. the stuff in between the sets of --- are your page variables. the only things you need are the title and image! title is just any string of characters (if there's special stuff, throw some quotes around them, like `title: "here's the title"`). image is just a file name of the image you want to use. that pulls from the img folder in the root! if you make subfolders then you just should write the file like `foldername/filename.png` (make sure you omit the first slash! the code has that in for you). if you want to upload more images go to the img folder, and then "upload files" at the top right and select whatever you want to upload. if you want to make a folder inside there, just do "create file" and then in the filename section add your folder name with a slash after it, and it'll create that folder. you should save a text file in any new folder you make because otherwise git won't save the folder (don't worry, the text file won't cause any issues. i do it all the time in unity projects, i just add files called "blank.txt" and the whole contents are just the word "blank"). ([if you need further instructions](https://stackoverflow.com/a/18791455)). 

if you make a new game project, make sure the filename is in the format yyyy-mm-dd-title-here.md (so, year-month-day-title.md, or `2017-07-20-my-cool-game.md`). it must be in that format! jekyll sorts the posts by date newest to oldest, so that's kinda how you're sorting things. 

your illustration page is kinda different in that it's just one file! that's called illustration.md. to edit that, simply click on the file and start editing the stuff below the ---s images are linked like `![alt title text](/file/name)`. posts are written in markdown format, [which you can read up on here](https://daringfireball.net/projects/markdown/syntax)! it's pretty straightforward. you can also just look at the files that i have in there currently and build off of those. (when adding images to posts, make sure there's a line of whitespace in between them, otherwise they get inlined and look bad. so do:

image

image

*not*

image
image

it's important!)

also, this seems counterintuitive, but due to the way i'm getting the homepage thumbnails, make sure you edit the `image` variable in the single post in _illustrations when you want to change that homepage thumbnail. for games it pulls from the newest post, but since illustrations is just that illustration.md file in the root, it can't pull from it in the same way! 

# Further Reading

[Jekyll Documentation](https://jekyllrb.com/docs/home/)

[Markdown Documentation](https://daringfireball.net/projects/markdown/syntax)