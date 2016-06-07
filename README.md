# I'M NOT CRAZY
Although this is a site with static webpages, it is rendered with Jekyll and Grunt.

Jekyll (and therefore Liquid) is used as the templating system. GitHub Pages supports Jekyll if you
commit your Jekyll site to the repo (including \_layouts, \_includes, etc), but I did feel like doing that. Why? well:

* Custom plugins cannot be used. While I've never had a particular reason to use Ruby, I could always learn and there exists the
  possibility of using custom plugins in the site's build.
* I would have to add two `---` at the top of each `.sass` and `.coffee` file. And I'm lazy.

I have a ton of different grunt tasks:
* grunt-contrib-coffee, grunt-contrib-sass - Compiling CoffeeScript and SASS, respectively.
* grunt-contrib-copy - Copying files from different project locations of my computer to sync projects.
* grunt-prettify - Since Jekyll is pretty weird about where rendered html should be placed, I've resorted to this grunt task.
  Up until recently, if you tried viewing the html of the rendered pages you would have a hard time because there were too many
  newlines and sometimes indents were in weird places. That shouldn't be much of a problem anymore.
