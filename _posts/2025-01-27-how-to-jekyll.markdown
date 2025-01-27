---
layout: post
title:  "How to quick-start a Jekyll blog"
date:   2025-01-27 12:23:42 +0100
categories: jekyll
---

I love Jekyll.

I've used it around 2020 to create an underground game review blog, and I loved how simple it is to maintain a site Jekyll.

Jekyll is not really a "blogging" tool. Rather, it's a static site generator that happens to be great for blogging. By now it's a bit dated, but it's still possible to set up a site with Jekyll insanely fast if you want to.

So as I'm just now setting up my own "frog does tech" blog, I thought I might as well write down a quick-start guide on creating a Jekyll blog, especially that I have not done it in a while.

Here goes.

## 1. Install prerequisites for Jekyll

### Install ruby.
Jekyll is a Ruby Gem. If you don't know what that is, gems are basically self-contained libraries of Ruby code you can execute without injecting the code itself into your program. To run a gem, you need to have Ruby installed on your device.

Jekyll requires Ruby version 2.5.0. Type `ruby -v` into your terminal right now and hit enter. If you have version 2.5.0 or above, you're good. If you get a big ugly red error, most likely you don't have Ruby installed. Go to Ruby's site and grab the right distribution [here](https://www.ruby-lang.org/en/downloads/). If you are on Windows like me, you can just use [RubyInstaller](https://rubyinstaller.org/downloads/).

### Update your Ruby Gems

If you already have Ruby installed, but you have not updated the gems for a while, you can do that by running this in your terminal:

```
gem update --system
```
This should update your gems, and give you a nice `RubyGems system software updated` message at the end.

## 2. Install Jekyll

Install the Jekyll gem in your terminal:

```
gem install jekyll bundler
```

That is going to install Jekyll proper on your device. It should return a nice `x gems installed` message for you at the end. Once it does that you're ready to create a Jekyll site.

## 3. Create a Jekyll site

Go to the parent folder where you want to create your site and terminal this in:

```
jekyll new sitename
```

That will create a `sitename` folder with the project files inside. Once the process is done, you're ready to go.

## 4. Run your empty Jekyll site

Go into the folder where you created your new Jekyll site. Type this into the terminal:

```
bundle exec jekyll serve
```

Now open your browser and go to `127.0.0.1:4000`. This is your new site. It looks lame and empty, but there is a few things you can do about that.

## 5. Customize your site

Go to the `_config.yml` file in the project folder.

This has a bunch of global settings for your blog. The file is pretty self explanatory, you can edit the title and description of your site, add you email and social links.

You can edit those settings and then run the site again with `bundle exec jekyll serve`.

## 6. Write your first article

In the `_posts` folder, Jekyll is going to store posts to display in the blog feed. There should be a sample article there right now.

You can go ahead and edit that, and also make duplicates of that file for any new post that you want to add to the site. Every post should have the same filename format (yyyy-mm-dd-some-title) and a `.markdown` extension. This way Jekyll will be able to process your posts into static HTML pages.

Once you edit your post, or add a new one, you will be able to access it from the "Posts" feed on your site's home page.

## 7. There is more

Jekyll has a bunch of other possibilities. If you look into the `_config.yml` file, you will see that the default theme for your site is `minima`. But there are other themes you can apply to your site.

You can also override the theme layout and styles to create your own custom (or semi-custom) theme.

All of that is outside of the scope of this article. I may create an article in the future going into more Jekyll customization.

## 8. Hosting your site

The beauty of Jekyll as a static site generator is that you can just grab the `_site` folder and host that anywhere as a static site. You can for example upload it to a GitHub repository and host with GitHub pages, or host it with pretty much any other service or hosting provider.

Again, since it's a static site, (almost) nothing can go wrong.

## Summary

By now you (and I as well) should have a Jekyll website ready to start blogging. Jekyll has aged a bit since I first used it, and I will likely look for alternatives to it soon. For now though, I'm happy I was able to bootstrap my blog lightning-fast.

Time to get blogging now. Rrrrrribit!