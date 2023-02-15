---
Date: 2023-01-01 00:00
Type: Page
---

# Personalizing your weblog

Now that you've written a blog post or two and familiarized yourself with Markdown a little, it's time to make your weblog a little more your own. We're going to do that by learning how to use your weblog's configuration page. 

You can find the configuration page by visiting the main weblog.lol page. To get there:

1. Visit <https://omg.lol>
2. Click "Dashboard"
3. Click "Weblog"

(If you have more than one omg.lol address, click the one you want to use and then click "Weblog") 


Once you're there, you should see a new blog post screen. Look below the blog post's text area for a button that says "Configuration" and click it. You'll see a text area that looks a lot like the blog post editing area. Feel free to click inside that text area and look around. 

## Configuration file basics

weblog.lol uses what's commonly referred to as a "configuration file" to customize your weblog. If you're used to using programs with a settings window of some kind, this is a little different: You don't click buttons or check boxes to change the settings, but instead edit text. 

You might have noticed that the text you're looking at is similar to the front matter of a blog post. Front matter and the configuration file behave similarly, using pairs of setting names and values. 

For instance, similar to how you set the date in a post's front matter using the setting name `date` and a date value:

`Date: 2013-02-10 13:45`

... you can set your weblog's title using the setting name `Weblog name` and some text:

`Weblog name: A Pretty Fine Weblog`

Using the configuration file, you can: 

- Set your weblog's name. 
- Set your weblog's description.
- Set your weblog's timezone. 
- Change how your weblog shows the date and time. 

... and much more. 

In case you didn't notice, there's a space between the colon and the configuration value for each setting. Make sure to keep that in there. In other words:

```
;; correct 
Weblog name: A Pretty Fine Weblog
```

```
;; incorrect
Weblog name:A Pretty Fine Weblog
```

You may have just noticed some lines starting with `;;`. Let's cover that. 

### Understanding comments 

There is one other thing to know about the configuration file before we start poking around, and that's the idea of "comments."

Simply put, any line that begins with `;;` or `//` is a comment. That means weblog.lol will ignore that line when it's deciding how to configure your weblog. 

You can use comments to add notes to your configuration file to keep track of what does what or try new things out by commenting out one line and adding another that's a little different just to see what happens without forgetting what the original line looked like in case you need to switch back. 

Here's an example of how you can use comments: 

```
;; tell marketing to pick a better name for this weblog
Weblog name: A Blog Full of Things You Should Buy Right Now
```


## What if I mess something up? 

If you're new to configuration files, or just a normal human being who occasionally makes a typo or forgets the right name for something, there's a chance you'll make a mistake and mess up your weblog. Or, you might just make a bunch of changes to your weblog's configuration and decide you don't like them. There are two ways to handle this:

1. You can always copy and paste your configuration file into a text editor (like Apple's Notes or Windows' Notepad) and save it. That's a good practice once you've made a few changes no matter what. 
2. You can copy the original configuration file from our site repository on GitHub and get back to a completely default state. 

If you need to do the latter: 

1. [Visit our copy on GitHub](https://github.com/neatnik/weblog.lol/blob/main/configuration/configuration.txt).
2. Click on the button that says "Raw" at the top of the configuration file text.
3. Select all the text and copy it. 
4. Paste the text back into your configuration file on weblog.lol. 

Now that you know how to get back to a good state you can start poking around a little without worrying too much. 

## Personalize your weblog's title

Your weblog's title is the simplest thing to change in your configuration that you'll be able to observe immediately. It's also the very first option you can set in the configuration file, so let's start there. 

Your weblog's title is what people see at the top of the page when they visit your blog. It's also what they see in browser tabs, RSS readers, and any preview widgets on social media. To set it: 

1. Look for the line that reads `Weblog title: weblog.lol` 
2. Change the text after `Weblog title: ` to your weblog's title. 
3. Click "Save & Publish" 

You'll get a notification that your weblog is rebuilding. It might take a little time for that to happen: Each page has to be updated with your weblog's new title. 

You can see the results a couple of ways: 

- Visit your weblog's homepage: `https://YOURADDRESS.weblog.lol`
- Click on one of the posts in the "Posts" list underneath the configuration file editing area, then click "View Live."

Either way, at the top of your page you'll see your new weblog title in the upper left of the page. 

## Set your weblog author and description

Just like you changed the title, you can change your weblog's author and description. 

The author setting turns up in your weblog's RSS feeds, and you can also use it in your weblog templates if you want to add a byline to your blog posts, or put your name in a copyright notice. 

By default it looks like this:

```
Author: Your Name
```

As with the `Weblog title` setting, you can modify it by changing the text after the colon. 

Your weblog description is also something you won't see very often. It also shows up in your RSS feeds and can be added to templates. Some people like to use their weblog description as a subtitle in their templates, but that's a step beyond what we're trying to accomplish today. 

By default, it looks like this:

```
Weblog description: This is a weblog.
```

Go ahead and change it to whatever suits you. 

## Set your weblog's timezone

Finally, we're going to end these very basic customizations by setting your weblog's timezone. 

As we noted at the beginning of this guide, your weblog defaults to the UTC timezone. When it makes a blank post the time will reflect UTC. To get it to show your timezone, you'll need to change the `Timezone`
setting.

To make this change, you'll first need to know what to call your timezone. [Wikipedia has a helpful reference][timezones]. Visit that page and scroll down to the "List" section and start looking for your country and major city in the "TZ database name" column. Once you've found it, copy the value. It will look something like `America/Los_Angeles` or `Africa/Cairo `.

By default, the configuration file looks like this:

```
Timezone: UTC

```

Replace `UTC` with the value you copied. 

## Next steps

We're going to take a break from the configuration file for now, but will be coming back to it later in this guide to change some advanced settings. You can [skip ahead if you like][qs5], or move on to the next section, where we'll [learn how to make a page][qs4].



[timezones]: https://en.wikipedia.org/wiki/List_of_tz_database_time_zones

[qs1]: /quickstart-1-intro
[qs2]: /quickstart-2-first-post
[qs3]: /quickstart-3-personalize
[qs4]: /quickstart-4-pages
[qs5]: /quickstart-5-advanced-config
