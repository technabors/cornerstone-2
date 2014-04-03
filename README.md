# Cornerstone

Welcome to Cornerstone, the definitive resource for brand, content, visual, and interactive patterns for Rackspace. The goal of this project is to align the company around a specific style guide, and offer tools to help assist in that regard.

With that in mind, this project contains a documentation website that offers detail about the practices that should be followed, as well as the source code for a CSS framework that can be easily included in any web-based project.

It should be noted that Cornerstone is not meant to be a one-stop shop for creating control panels or highly interactive web projects. Instead, it's meant to serve as a foundation, helping to enforce best practices and encourage consistency.

## Getting started

Since this project contains both the documentation site and the code for the CSS, getting started depends on what you want to work on. Either way, you will need Ruby installed on your system.

One of the goals was to make this project as easy for people to contribute to as possible. In that spirit, there are only a few gems that you need to install in order to get up and running:

* [Sass](http://sass-lang.com/)
* [Jekyll](http://jekyllrb.com/)
* [Rake](http://rake.rubyforge.org/)

## Hack away!

We have created some Rake tasks which should help out. All of these tasks are meant to be run in the root project directory.

**Build Sass file**

```
rake sass:build
```

Compiles the `cornerstone.scss` file from the source `sass` directory and puts the result into the `site/css` folder. This allows you to do a quick one-time build and see the changes in the site.

**Watch Sass file**

```
rake sass:watch
```

Does the same thing as the `sass:build` task, but automatically re-compiles the `cornerstone.scss` file any time any of the source files in the `sass` directory change.

**Build Jekyll site**

```
rake site:build
```

Builds the Jekyll site based on the code located in the `site` directory. The destination of the built site is `site/_site`. This directory is ignored by git and should never be commited into version control.

**Serve Jekyll site**

```
rake site:serve
```

Does the same thing as `site:build`, but also serves the site using Jekyll's built in web server. This command will watch for any changes made in the `site` directory and automatically regenerate the site, as well.

## Contribute

Anyone is welcome to contribute to Cornerstone. We appreciate bug reports, feature requests, general discussions, and pull requests.

If you would like to make a code change, please keep the scope of the change as limited as possible. This makes it easier for the maintainers to review the changes and eventually merge the pull request.

## The Cornerstone Team

* [@troyswanson](https://github.com/troyswanson)
* [@vkarnes](https://github.com/vkarnes)
* [@roycestewart](https://github.com/roycestewart)
* [@elblakeo](https://github.com/elblakeo)
* [@technabors](https://github.com/technabors)

## License

<img src="http://632963c32a968e946ade-6a1f0be81bdf28a63f5fcf21842b6ecd.r29.cf1.rackcdn.com/arch-birdy.svg" height="65" align="right">

Copyright 2014 Rackspace Hosting, Inc.

Licensed under the Apache License
