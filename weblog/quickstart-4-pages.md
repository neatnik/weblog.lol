---
Date: 2023-01-01 00:00
Type: Page
---

# Making Pages

So far we've covered [the basics of weblog.lol posts][qs1], [how to write a blog post with Markdown][qs2], and [how to personalize your weblog with the configuration file][qs3]. If we were to stop there you'd have a working weblog. In this section, though, we're going to round it out by learning how to create pages. 

If posts are the core of most weblogs, pages help you round things out: Unlike posts, pages exist outside what people often think of as the "feed" of a weblog -- the stream of regular posts -- and provide a way to share more long-lived or less date-bound information. 

Pages are great for: 

- Telling people what your weblog is about. 
- Telling people more about you. 
- Providing links to resources, favorite sites, etc. 

On weblog.lol, the default templates for pages differ a little from posts: 

- They don't show tags. 
- They don't show the publishing date/time. 
- They don't show the recent pages list. 

You can put these things back in if you feel like it, but for purposes of this quick start we're going to work with them in their default form, which is pretty common to most weblog designs. 

We're also going to offer examples centered around a common use for pages on weblogs: The "About" page. "About" pages often include a little biographical or personal information, an overview of what the weblog is about, and sometimes how the weblog is made (such as what tools the author uses).

## Make your first page

Let's start by going to your main weblog.lol page. To get there:

1. Visit <https://omg.lol>
2. Click "Dashboard"
3. Click "Weblog"

(If you have more than one omg.lol address, click the one you want to use and then click "Weblog") 

Once you're there, you should see the familiar new blog post screen. 

You use the new post screen to make pages, as well. You just have to add some metadata to the front matter. 

Looking at the new post editing area, the front matter should look like this:

```
---
Date: 2023-02-13 19:17
---
```

To start working on your new page, you need to add a line to the front matter to set the `Type` of content you're working on. Add a line under the `Date`, setting the `Type` to "Page," like this:

```
---
Date: 2023-02-13 19:17
Type: Page
---
```

Before we save it let's also change the title and text of the page to something a little more appropriate for this exercise. The main body of page should look like this:

```
# Your new post

This is a new blog post. You can author it in _Markdown_, which is **awesome**.
```

As you may recall, starting the beginning of the first line in a post (or page) with `#` sets the title. Let's make a few small changes: 

```
# About this weblog

This is a new page we are authoring in _Markdown_, which is **awesome**.
```

Once you've made the changes, let's save it and see how it looks:

- Click the "Save and Publish" button, just underneath the editing area. 
- Click the "View Live" button. 

Your new page will open in a new tab:

![Screenshot of a web browser showing our new page.](ss_weblog_new_page.jpg)

As we noted in the introduction, this looks a little different from a regular blog post: 

- There's no date. 
- There's no list of recent posts. 
- There's no list of tags. 

When you're done looking around, close the tab and let's learn one more thing about pages. 

## Customize your new page's URL

Every web page has a "URL" -- its address, which you can find in the location bar of your browser.  Depending on whether you followed along or decided to go your own way, you may have noticed that your new page has a URL like this:

`https://YOURADDRESS.weblog.lol/about-this-weblog`

The part of the URL after the right-most `/` is often referred to as the "slug."

Once upon a time in the early web it was not uncommon for web pages to have less readable URLs. You may remember seeing things like:

`http://somesite.com/section?234&article_id=12345`

or

`http://anothersite.com/1a235fc69088bz`

These kinds of URLs didn't work very well for people and over time it became more and more common to make URLs a little more human (and search engine) readable. 

As it stands, `https://YOURADDRESS.weblog.lol/about-this-weblog` isn't the worst URL in the world. It's human-readable, and it's relatively easy to share by quickly writing it down or just saying it to someone. We can make it a little bit more easy to share, and also make it easier to guess. 

Your page's front matter should currently look something like:

---
Date: 2023-02-13 19:17
Type: Page
---

We can change the URL by adding the `Location` setting to the front matter. Most "About" pages have the very simple slug of "about," so let's use that:

---
Date: 2023-02-13 19:17
Type: Page
Location: /about
---

You may have noticed the leading `/` in the `Location` setting. If a `Location` setting starts with `/` that means the URL will be relative to the "site root" (the topmost directory) of your weblog. 

See for yourself by clicking "Save and Publish" and then clicking "View Live." Your new page will open in a new tab and you can review the new URL in your browser's location bar: 

`https://YOURADDRESS.weblog.lol/about`

That's a little shorter, a little easier to share, and more in line with what people expect for an "About" page URL if they decide to just type it into their browser for some reason. 

## A few more notes on custom locations 

You are no doubt wondering, if you didn't just go find one of your blog posts and try it yourself, if the `Location` setting works for blog posts, as well. It does, indeed. If you don't like the default URL structure of weblog.lol posts, however, we're going to cover how to change that in the next section. 

You can also create custom locations a few "directory" levels deep, to help organize your weblog a little better if you're going to have numerous pages about multiple topics. For instance, suppose your interests are botany and skateboarding. You could set custom locations for each page about those topics in a way that creates a directory structure for your weblog: 

- `Location: /plants/interesting-links`
- `Location: /plants/my-house-plants`
- `Location: /plants/care-tips`

and 

- `Location: /skateboarding/my-collection`
- `Location: /skateboarding/trick-videos`



## Next steps

It's pretty easy to make pages on weblog.lol. You might have noticed, however, that your new page wasn't linked anywhere on your weblog. [The next section][qs5] -- looking at some advanced options in your configuration file -- will help with that by teaching you how to create a navigation menu for your site. 


[qs1]: /quickstart-1-intro
[qs2]: /quickstart-2-first-post
[qs3]: /quickstart-3-personalize
[qs4]: /quickstart-4-pages
[qs5]: /quickstart-5-advanced-config


