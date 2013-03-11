# Blogginekyll

## What is it?
Blogginekyll is a super simple theme for a [Jekyll](https://github.com/mojombo/jekyll) blog. You can clone/fork it and start blogging right away!

## Why did you build it?
We as developers are notoriously *bad* at designing. I thought I'd help out by building something that looks good (I hope).

## Getting started
Sold? Ok awesome heres how to get started!

#### What you'll need

You'll need to install [Jekyll](https://github.com/mojombo/jekyll) if you don't already have it.

```
gem install jekyll
```
While you're at it, you'll also need [sass](http://sass-lang.com/) and [pygments](http://pygments.org/), information can be found on their sites.

Once everything is installed, fork or clone [Blogginekyll](https://github.com/sirbrad/blogginekyll).

## Making it your own

You'll need to add your own information, ie what you wish to call your blog, strapline and about section. I set up an interactive rake task to help with this so run `rake build`.

## Adding your personal touch

It's also unbelievably easy to customise the style of your blog. Open up `_setup.scss` in your editor and make changes to the variables and those changes will be made across the site.

Be sure to tell sass to watch for changes, I have a shell script for this. Navigate to a new tab in terminal and run `sh watch.sh`. #b000m

## Awesome, final words?

Sure, you're free to customise any of the code as much as you'd like. Contributions are welcome, and if you're using Blogginekyll for your site I'd love to see it so tweet me (@bradleyfew)!

