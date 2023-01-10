Date: 2023-01-01 00:00
Type: Page

# Configuration Basics

Weblog.lol uses a simple but powerful configuration engine. Rather than configure your weblog through a pre-defined user interface, you configure it through a _file_. This allows for tons of flexibility, including the ability to configure things that you create entirely on your own.

## Reference configuration file

We make a [reference configuration file](https://github.com/neatnik/omg.lol/blob/main/weblog/weblog-default-configuration.conf) available to anyone who might accidentally goof up their configuration and need to restore it. This file also defines the default configuration, so if you’re ever wondering what a default is, you can refer to it to find out. As defaults are updated, this file is also updated. If your configuration file is missing a specific configuration item, your weblog will always use the default (since that’s a better option than it breaking entirely).

## Comments

You can comment any line by using `#`, `//`, or `;` at the start of the line.

## Configuration patterns

Configuration items are defined as a key/value pair, with a colon and a space separating the key and value. For example:

```
Weblog title: A Weblog
```

This sets your weblog title to “A Weblog”. It also means that anywhere you use `{%weblog-title}`, within your template or the body of an entry, the text “A Weblog” will be displayed on the rendered page.

If the value of a configuration item needs to span multiple lines, the _bumpers_ `<<[` and `]>>` are used. For example:

```
Evergreen grocery list: <<[
<ul>
  <li>A loaf of bread</li>
  <li>A container of milk</li>
  <li>A stick of butter</li>
</ul>]>>
```

## Configuration templates

Some weblog features make use of configuration templates, where you can define specific types of output within a small template. For example:

```
Search results format: <<[
<h2>Results for “$search”</h2>
<p>$search_results_message</p>
[post:begin]<h3><a href="$location">$title</a></h3>
<p>$date</p>
<p>$snippet</p>[post:end]
]>>
```

These templates use `begin` and `end` indicators for any repeating content, and `$variables` for any special content that would be included. In the example above, `[post:begin]` and `[post:end]` signal the content that would be repeated for any post included in the search results, and `$location` and `$title` are variables for Location and Title respectively.

<i class="fa-solid fa-fw fa-circle-right"></i> [Next, we’ll look at some specific configuration items.](/configuration-items)