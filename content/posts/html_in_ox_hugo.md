+++
title = "How To Add HTML To Your Hugo Website"
author = ["santi"]
date = 2020-08-07
draft = true
weight = 1004
+++

Ever since I decided to redesign my website with ox-hugo, my mind has been blown.

I've had to work with a couple of workarounds to do exactly what I need.

Among this things I wanted to find a way to include HTML into my org-file.

Initially I thought I'd be able to get away with the following due to org-mode functionality.

`#+BEGIN_SRC HTML`

I'd write HTML code in between this tags.

`#+END_SRC`

**Of course this didn't work** since ox-hugo exports to markdown and markdown doesn't support this feature.


## How To Do It? {#how-to-do-it}

I wasn't able to find anything in the documentation, but thanfully I stambled upon an amazing [short blog-post](~/Zotero/storage/289Z3CW7/hugo-raw-html-shortcode.html), which taught me exactly how to include HTML. This tutorial is made with Hugo using Markdown, thankfully it works exactly the same for ox-hugo without any extra steps.

The following steps are fully attributed to the author of the blogpost [Ana Ulin](https://anaulin.org), so thanks to Ana for this.

The way to do it is how to your hugo directroy
in my case I have mine in

/home/user/hugo/santiyounger

go to layouts

in there create a new folder called "shortcode"

then create a file and call it rawhtml.html

edit the file with your favorite editor ;)
and add the following to it:

```nil
<!-- raw html -->
{{.Inner}}
```

now go to your org mode file where you edit your ox-hugo webiste.

Choose a place where you want to insert some HTML
open the HTML with:

`{{< rawhtml >}}`
and end it with:
`{{< /rawhtml >}}`

I found this extremely useful for migrating my old blog-posts into this new ox-hugo website set-up, since most of my old content was formatted in in HTML.

Of course the reason why you might need this is to work with css. Which is one of the biggest reasons to set this up.
