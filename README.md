# HTML Lists, Images and Links

## Learning Goals

- Identify ordered, unordered and definition lists
- Identify images
- Identify links
- Identify HTML validation tools

## Introduction

You might be wondering what else is available to use to build out full webpages
now that you are more familiar with the basics of HTML. How do you display an
image? How do you add a formatted list of topics? How do you link page elements
beyond text? Now you're ready to explore these fundamental tools. Here's a
high-level overview before you dive into practicing with the labs.

### Identify Ordered, Unordered and Definition Lists

When we want to present a list of items in a clear, readable format, we turn to
the HTML unordered list, represented by the `ul` tag.

```
<ul>
  <li>One item</li>
  <li>Another item</li>
</ul>
```

If it's important to distinguish a particular order of the items (as for a
recipe or ranking), we use an ordered list, or the `ol` tag.

```
<ol>
  <li>First item</li>
  <li>Second item</li>
</ol>
```

Notice the nesting of our items within the lists. Each `li` is a list item
contained in the larger `ul` or `ol` container.

Another type of list we can use is a definition list, which defines specific
types of items.

```
<dl>
  <dt>First term</dt>
  <dd>Term definition</dd>
</dl>
```

### Identify Images

To include an image in our page, we use an `img` tag.

```
<img src="myimage.jpg" alt="Alternative Text" title="Display Title"
width="800" height="600">
```

There are two notable things about the `img` tag: The first is that it does not
have a closing tag. The image tag closes itself. Secondly, it handles a lot of
_attributes_. Attributes are special keywords used on the tag to control the
element's behavior, or provide additional information about the HTML element.

The `alt` attribute provides descriptive text the browser can display if it
can't find the image file. The browser can also display the `title` text to give
the user more information about the image. The `width` and `height` attributes
define the size of the image that shows up in the browser. 

### Identify Links

You might be familiar with basic link structure already, but here are other ways
we can use them.

Beginning with a standard text hyperlink, we can wrap other elements inside of them.

```
<a href="http://example.com/">This is a link</a>
```

What if we want to link an image instead of text? We can replace the text within
the `a` tags with our image tag.

```
<a href="http://example.com/">
  <img src="myimage.jpg" alt="Alternative Text">
</a>
```

What about a link that will direct to an email address?

```
<a href="mailto:webmaster@example.com">Send an email</a>
```

Sometimes we might want to link to a specific location on the same
webpage. We can then target an element that we identified or classified earlier.

```
<p id="tips">Useful Tips Section</p>
<a href="#tips">Jump to the Useful Tips Section</a>
```

When considering what location links point to, you will choose between relative
or absolute links. A relative link directs to content within the same website.

```
<a href="about.html">This is a relative URL link</a>
```

An absolute link, on the other hand, links to external content and requires a
fully defined URL path. This is likely the type of link you see most often.

```
<a href="http://example.com/">This is an absolute URL link</a>
```

### Identify HTML validation tools

An HTML validator is used to check HTML markup elements for syntax errors.
Syntax errors, such as open tags, extra spaces, or forgotten quotation marks,
can cause a web page to look drastically different than the creator intended, or
render correctly in one browser, but not in another.

It's easy to forget a closing HTML tag or miss a piece of punctuation when
writing HTML. Fortunately, we have a tool that will check our markup for us and
point out any errors. To validate our HTML, we can use the [W3 HTML validator]
(http://validator.w3.org).

## Conclusion

Now that you've taken a first look at these new HTML elements, you'll be better
prepared to practice them in labs, where you'll learn more about each one and
how to use it effectively.

## Resources

* [HTML Fundamentals overview video](https://www.youtube.com/watch?v=tuDKQxfiXmY)
