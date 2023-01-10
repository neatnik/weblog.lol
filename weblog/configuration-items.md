Date: 2023-01-01 00:00
Type: Page

# Configuration Items

_Note: This page is a work in progress._

Let’s take a look at each of the specific configuration items in your weblog. There’s a lot here, but one thing to keep in mind is that you don’t have to deal with all of this—just change whatever you feel like changing. You can leave as many of the default values alone as you’d like, and your weblog will work just fine.

<table>
<thead>
<tr>
<th>Item</th>
<th>Description</th>
<th>Default Value</th>
</tr>
</thead>
<tbody>

<tr>
<td>Weblog title</td>
<td>The title of your weblog, used with the <code>{title}</code> tag.</td>
<td>
<pre>
<code>Weblog title</code>
</pre>
</td>
</tr>

<tr>
<td>Weblog description</td>
<td>A description for your weblog, used with the <code>{description}</code> tag. Useful for Open Graph metadata (i.e. what shows up in different social sites when people link to your weblog).</td>
<td>
<pre>
<code>This is a weblog.</code>
</pre>
</td>
</tr>

<tr>
<td>Author</td>
<td>Your name. Used with the <code>author</code> tag.</td>
<td>
<pre>
<code>Your Name</code>
</pre>
</td>
</tr>

<tr>
<td>Canonical domain</td>
<td>When set to a valid domain name, this defines a canonical domain for your weblog. This means that if someone tries to visit your weblog through another means (e.g. foobar.omg.lol), they’ll be redirected to your canonical domain instead.</td>
<td>
<em>no default</em>
</td>
</tr>

<tr>
<td>Separator</td>
<td>A string that can be used to separate things, such as the weblog title and current post title within the <code>&lt;title&gt;</code> element. Used with the <code>separator</code> tag, and will not be rendered on page when contextually inappropriate.</td>
<td>
<pre>
<code>·</code> (interpunct)
</pre>
</td>
</tr>

<tr>
<td>Navigation</td>
<td>A comma-separated list of entries (specified by location) that are converted to proper links when the <code>navigation</code> tag is used. Can also include Markdown links and HTML links.</td>
<td>
<em>no default</em>
</td>
</tr>

<tr>
<td>Timezone</td>
<td>Configures the timezone that should be used for your weblog. Uses [TZ database name values](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).</td>
<td>
<pre>
<code>UTC</code>
</pre>
</td>
</tr>

<tr>
<td>Date format</td>
<td>A string of [date/time format characters](/date-time-formatting) that’s used with the <code>{date}</code> tag.</td>
<td>
<pre>
<code>F j, Y g:i A</code>
</pre>
</td>
</tr>

<tr>
<td>Feed post count</td>
<td>The number of weblog posts to include in your [feeds](/feeds).</td>
<td>
<pre>
<code>25</code>
</pre>
</td>
</tr>

<tr>
<td>Post path format</td>
<td>The format used for your post path, which will make up the portion of the URL between the domain and the post slug. Uses the same [date/time format characters](/date-time-formatting) as the <code>Date format</code> item above. Text enclosed in <code>"double quotes"</code> will not be parsed as date/time values.</td>
<td>
<pre>
<code>25</code>
</pre>
</td>
</tr>

</tbody>
</table>
