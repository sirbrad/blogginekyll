# Blogginekyll

## What is it?
Blogginekyll is a super simple theme for a [Jekyll](https://github.com/mojombo/jekyll) blog. You can clone/fork it and start blogging right away!

You can see a [demo](http://bradleyfew.com/blogginekyll) here.

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

Firstly, it's probably best to go through the html and add the correct information for yourself. Here's a list of what needs changing;

- Page Title `/index.html#l3`
- Site Logo `/inclues/header.html#l3`
- Site Strapline `/inclues/header.html#l4 `
- About me section `/includes/footer.html#l3`
- Twitter handle `/includes/site-credits.html#l2` & `/includes/site-credits.html#l3` 
- Copyright information `/includes/site-credits.html#l4`

I'm going to investigate how the above could be automated.

Now start the Jekyll server `jekyll --server` and navigate too `localhost:4000` and your new blog is now running.

## Adding your personal touch

It's also unbelievably easy to customise the style of your blog. Open up `_setup.scss` in your editor and make changes to the variables and those changes will be made across the site.

Be sure to tell sass to watch for changes, I have a shell script for this. Navigate to a new tab in terminal and run `sh watch.sh`. #b000m

## Awesome, final words?

Sure, you're free to customise any of the code as much as you'd like. Contributions are welcome, and if you're using Blogginekyll for your site I'd love to see it so tweet me (@bradleyfew)!

