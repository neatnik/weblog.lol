---
Date: 2023-01-01 00:00
Type: Page
Locaton: /quickstart-1-intro
---

# weblog.lol quick start guide

Welcome to the weblog.lol quick start guide. With this guide, we're going to show you how to go from a blank page to a working weblog, covering just enough to get you going. 

Along the way you're going to learn: 

- What front matter and Markdown are. (this section)
- [How to write your first blog post][qs2].
- [How to personalize your weblog][qs3]. 
- [How to create a page for your weblog][qs4]
- [How to customize your weblog's navigation and URL structure][qs5].

## How to use this guide

If you like to learn by following along with a video, we also have a [getting started video you can watch][video]. It's just 36 minutes long and covers much of what we cover here. 

We're also going to take a very "learn by doing" approach here: You should follow along with the examples, make changes, try things out, and save your work now and then to see how it looks live. One of the great features of weblog.lol is the ability to save your work and see your changes right away, and fix any mistakes or glitches just as quickly.

You don't have to use our examples, but if you decide to experiment a little the guide will build on itself from section to section. That will mean some screenshots and configuration examples will depend on you starting from scratch and following along closely.

## Getting ready to write your first blog post 

If you haven't done anything with your weblog.lol account yet, there is not a lot to see. You can take a look by visiting your weblog using your omg.lol address: 

`https://YOUR ADDRESS/weblog.lol`

If you haven't made a post yet, your browser will show something like this:

![A screenshot of a web browser showing a 'not found' page](https://raw.githubusercontent.com/neatnik/weblog.lol/main/images/ss_weblog_blank.jpg)

It isn't very inspiring, but we're going to fix that. Let's start by getting you to your weblog.lol homepage: 

- Visit <https://omg.lol>
- Click "Dashboard"
- Click "Weblog"

(If you have more than one omg.lol address, click the one you want to use and then click "Weblog") 


You should be looking at a page with a new post ready to go in the editing area: 

![A screenshot of a browser with a text editing area and a new blog post ready to go.](https://raw.githubusercontent.com/neatnik/weblog.lol/main/images/ss_weblog_new.jpg)

If you're used to using a word processor, or if you've edited web content in the past using a WYSIWYG tool, making a post on weblog.lol will be a change of pace. 

Let's take a look at that new post, because it includes two things you'll be learning much more about as we work through this guide: front matter, and Markdown. 

### What's front matter? 

At the very top of that post, there's a section marked off by dashes: 

```
---
Date: 2023-02-08 23:05
---
```

That's the "front matter." Every post you write will need to have it, but it doesn't appear directly on your weblog: It just provides the information weblog.lol needs to display your posts in the right order, include tags, and set a few other options you'll learn about later. The information found in the front matter is commonly referred to as "metadata." 

You don't need to know much more than that for now, and weblog.lol will always fill that part in for you when you start a new post, so just remember that the front matter for each post is not optional.

Right now, you'll notice that the front matter for this new post includes only a single line for the post's date and time. 

You might have also noticed that the date and time don't match your location. That's because weblog.lol starts out using UTC until you tell it your timezone. We'll cover updating that a little later in the guide. For now, you can:

- Set the correct date and time in the front matter on the new post, or ...
- [Skip ahead][qs3] to the timezone section and fix it right away. 

If you prefer to wait, just remember to set your weblog's timezone before you write many posts because they'll need to be updated by hand if they're written before you set it. 

Moving on past the front matter, let's look at the rest of the post, which we'll refer to as "the body." By default, it looks like this:

```
# Your new post

This is a new blog post. You can author it in _Markdown_, which is **awesome**.
```
That raises at least one question:

### What's Markdown?

... and why is it awesome?

During the early days of the web if you wanted to write content you had a few choices:

One, you could use HTML. HTML is what we call a "markup" language. Instead of clicking a "bold" or "italics" button, HTML uses markup -- you have to add special text to your content to format it.  HTML is very expressive -- there are lots of ways to format text, link to stuff, etc. --  but it's also a little fussy and hard to read, especially if you're just writing prose and not doing actual web design. 

Two, you could use some sort of WYSIWYG editor on a web page, similar to a word processor. If you've used WordPress or some web forums where you can click on a little "B" to make text bold or a link icon to make a hyperlink, you've seen a WYSIWYG editor in action. 

Markdown was invented to make it easier to write for the web if all you want to do is write prose -- blog posts, pages, etc. Markdown is designed to let you format text with very little typing, using a sort of shorthand that people used to use in plain text email all the time. In the years since it was first introduced Markdown has become quite popular with bloggers and just about anybody who needs to write content that will show up on the web at some point.  

To get an idea of what Markdown's about, let's look at the post again, line by line:

```
# Your new post
```

When you write in Markdown, that opening `#` means "level 1 heading." If you've written in HTML in the past, that's the same as the `<h1>` tag. 

In weblog.lol, it also sets the title of your post, as we'll see shortly. 

Moving along:

```
This is a new blog post. You can author it in _Markdown_, which is **awesome**.
```

In Markdown, surrounding text with `_` characters italicizes it, and surrounding text with `**` makes it bold. 

If you were to write the same sentence in HTML, it would look like this:

```
<p>This is a new blog post. You can author it in <em>Markdown</em>, which is <strong>awesome</strong>.</p>
```
And once it's published, it will look like this:

> This is a new blog post. You can author it in _Markdown_, which is **awesome**.

#### Optional: More on Markdown
This is just a small taste of Markdown. If you'd like to learn about a few more formatting options, we recommend [this quick reference][mdref]. 

If you're _very_ familiar with Markdown, you'll be interested to know we use the [CommonMark][] specification. Until we have a more complete operator's manual available, [here's a list of extensions we use][extensions] as well as a link to more information. 


## Next steps

Now that you understand what front matter is and a little bit about how Markdown works, let's move on to [writing your first blog post](quick-start-first-post.md). 



[qs1]: /quickstart-1-intro
[qs2]: /quickstart-2-first-post
[qs3]: /quickstart-3-personalize
[qs4]: /quickstart-4-pages
[qs5]: /quickstart-5-advanced-config

[video]: https://www.youtube.com/watch?v=kcEKdxGABGU
[mdref]: https://commonmark.org/help/
[CommonMark]: https://commonmark.org
[extensions]: https://docs.paste.lol/weblog-markdown-extensions.md/markup