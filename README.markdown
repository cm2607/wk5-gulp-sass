## What's here

I have created a very basic starter file for using gulp and sass. I also set up the project to have a help file structure.

## Gulpfile

The gulpfile has three functions. One to turn your Sass files into css; one to watch your Sass files for changes; and one to define a default task to run when you type `gulp` in the command line.

Note: You also can use the sass task directly from the command line by typing `gulp sass`. This skips the watch task and it doesn't run.

## Folder structure

As you start using more build tools and whatnot, you quickly realize that you don't want people who visit your site to access this stuff. In other words, you shouldn't be able to browse to your Sass files from the browser.

Also, separating out your working, build files, from the final files helps keep your repo more organized and easier to work with going forward.

That's why you'll see folder structures like the one in this repo.

The `src` directory stands for "source". This is where you put files that will be used to build other files.

The `dist` folder stands for "distribution". These will be files that you make publicly available.

You could also call these folders "private" and "public" if that is clearer.

## Never edit your `dist` files

Once you start using build tools, you will need to remind yourself to *never edit files in your dist folder*. So, if you're working with Sass, you only edit the Sass files, never the CSS files directly. 
