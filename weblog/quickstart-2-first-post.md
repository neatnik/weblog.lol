---
Date: 2023-01-01 00:00
Type: Page
Location: /quickstart-2-first-post
---

# Write your first blog post using Markdown

Now that you understand what front matter is and a little bit about how Markdown works, you can write your first blog post. 

In case you closed your browser window between pages, here's how to get to your weblog (and a new post): 

1. Visit <https://omg.lol>
2. Click "Dashboard"
3. Click "Weblog"

(If you have more than one omg.lol address, click the one you want to use and then click "Weblog") 

You should be looking at an editing area with a fresh post ready to go. 

Let's start by coming up with a title to replace the default, perhaps replacing this: 

```
# Your new post
```

with this: 

```
# My first blog post
```

Remember, the `#` means "heading," and on weblog.lol it will also set the title for the post: The title is what you see in the title bar of your browser window, a list of recent posts, or in a list of articles in your RSS reader.  

Now let's move on to the text of your new post. 

Let's try replacing this: 

```
This is a new blog post. You can author it in _Markdown_, which is **awesome**.
```

With this: 

```
This is my first post on my new weblog, hosted by [omg.lol](https://omg.lol), which is **awesome**. omg.lol includes a bunch of features, including:

- this weblog service
- a URL shortener
- a Mastodon instance
- a pastebin
```

Some of that might look familiar to you: Using Markdown, wrapping text in `**` makes it bold. 

But what about this part: 

```
[omg.lol](https://omg.lol)
```

That's how you make a link in Markdown. If you know HTML, it would look like this:

```
<a href="https://omg.lol">omg.lol</a>
```

And what about this part: 

```
- this weblog service
- a URL shortener
- a Mastodon instance
- a pastebin
```

That's how you make a list in Markdown. In HTML it would look like this:

```
<ul>
  <li>this weblog service</li>
  <li>a URL shortener</li>
  <li>a Mastodon instance</li>
  <li>a pastebin</li>
</ul>
```

If you'd like to see for yourself, this is as good a time as any to save your progress and take a look at your new post, so look just under the text area you've been writing in:

![A screenshot of a web browser with a text area and a button that reads 'Save and Publish'](ss_weblog_save_publish.jpg)

... and click the "Save and Publish" button. 

You should get a green notification that your entry has been saved, and you'll see a new "View Live" button under the editing area. Go ahead and click that, and a new tab will open with your post. Here's what it will look like if you used our example text: 

![Screenshot of a web browser showing a web post](ss_weblog_first_post.jpg)

Take a quick look around: 

- You'll notice the generic "A Weblog" header, which is currently your blog's name. We're going to change that soon. 
- You'll see the title, which you set using Markdown's "heading" character at the start of a line (`#`).
- You'll see the content of your post, with some bold text you got from wrapping text in `**`, and you'll see a link you made with Markdown using `[omg.lol](https://omg.lol`. 
- You'll see the date and time in the lower right of the post. 
- You'll see a smaller heading with a list of recent posts. If you've been sticking to the script, you'll just see one -- the one you're looking at. 

Did something go wrong? It happens. Sometimes a typo messes up a link, or you forgot to add a title, or something else isn't quite right. Just close the tab, go back to the editing screen, and give it another shot: 

1. Make your changes. 
2. Click "Save and Publish"
3. Click "View Live"

## Add tags to your post

We've got one more thing to cover before we move on to personalizing your weblog: Adding tags. 

You might be familiar with the concept of tagging from Twitter, Mastodon, or Instagram. On a weblog, tags serve as a simple way to categorize content as you go. You can add or remove tags to a post as you wish, and weblog.lol will keep track and provide links to all the other posts that share tags. Unlike social media services, your tags will link to just the content on _your_ weblog, not anybody else's. 

To add tags to your post, we're going to need to revisit the front matter. 

Right now, the front matter from your first post will look something like this:

```
---
Date: 2023-02-08 23:05
---
```

Let's add a line, just underneath the date, and above the bottom set of dashes: 

```
---
Date: 2023-02-08 23:05
Tags: quickstart, practice, tutorial
---
```

Click "Save and Publish," then click "View Live." If you look down in the lower right corner of your post, just under the date, you'll see your tags. Go ahead and click on one of them and you'll see something like this:

![A screenshot of a browser window with a page listing tagged posts](ss_weblog_tagpage.jpg)

Not a lot there, but as you add more and more entries to your weblog over time, tags will provide a way to see posts that are related to each other via common tags. 

Two more things to remember about tags:

- On weblog.lol, tags aren't case sensitive. If you tag one post `tutorial` and another `Tutorial`, they'll show up on the same tag page.
- Tags can have spaces. 

## Make a brand new post

After you're done working on your first blog post, you can try out making one of your very own: Click the "New Entry" button underneath the text editing area and you'll have a fresh post ready to go. It works just like the first one you found when you started this guide: 

1. Type some text 
2. Click "Save and Publish"
3. Click "View Live"
4. Admire your work

Remember, you can always delete your practice posts, so there's no harm in experimenting. Also, once you're ready to start customizing your weblog a little more it'll be helpful to have a few placeholder posts hanging around so you can see how your previous post list and tag pages look. 

Now that you know how to write a post and add tags, it's time to learn about [how to personalize your weblog][qs3]


[qs1]: /quickstart-1-intro
[qs2]: /quickstart-2-first-post
[qs3]: /quickstart-3-personalize
[qs4]: /quickstart-4-pages
[qs5]: /quickstart-5-advanced-config
