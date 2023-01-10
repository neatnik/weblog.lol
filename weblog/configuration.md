---
Date: 2023-01-03 02:46
Type: Page
---

# Configuration

OK, so: this page is going to cover _a lot_ of stuff. But here’s the thing: you don’t really need to know about or act on _any_ of it. Your weblog will happily serve content even if you don’t touch your configuration at all. You can skip this entirely and go do something else if you’d like.

If you’d like to customize your weblog, though, configuring it is a great place to start. You can customize as much or as little of your weblog as you wish.

## Reference configuration file

We make a [reference configuration file](https://github.com/neatnik/omg.lol/blob/main/weblog/weblog-default-configuration.conf) available to anyone who might accidentally goof up their configuration and need to restore it. This file also defines the default configuration, so if you’re ever wondering what a default is, you can refer to it to find out. As defaults are updated, this file is also updated.

## Comments

You can comment any line by using `#`, `//`, or `;` at the start of the line.

## Configuration patterns

Configuration is defined as a key/value pair, with a colon and a space separating the key and value. For example:

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

_To be continued..._