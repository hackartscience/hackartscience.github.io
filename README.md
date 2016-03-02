[hackartscience.com][http://hackartscience.com]
====================
This site, `http://hackartscience.github.io` aliased to `hackartscience.com` is hosted via [GitHub Pages][ghpages], and is generated from [markdown][markdown] via heavily scripted [Jekyll][jekyll], a blog-friendly high level tool for generating static websites.

Creating articles
-----------------

To create an article, add a `markdown` document to `_posts/`.
This new file should be named `<DATE>-<TITLE>`, for example `2016-02-03-my_article.md`.
Each file of this format in `_posts/` will be shown on the articles pages of the site in reverse chronological order.

Each article should include a *front matter* (some metadata which the site will use to contextualize the article), much like the following:

    ---
    layout: post
    title:  "My amazing article"
    banner: http://domain.com/picture.jpg
    excerpt_separator: <!--excerpt-->
    ---

The article itself should be written in the markdown language ([helpful cheatsheet][gh-markdown]), which is great at endowing text with some basic content organization tools like sections and itemized lists. The `excerpt separator` defines where to end snippets for article preview views (without it, the first paragraph is the excerpt).

Static resources stored externally
----------------------------------
Images and other resources ill-suited for a `git` repository are linked.
We host images and other external resources via `files.hackartscience.com`, a file server which we manage via `Samba` and a `OwnCloud`.

SSL Certificate
---------------
Unfortunately, GitHub Pages is not likely to offer SSL certificates for custom domains anytime soon.
We are working on a workaround, possibly something similar to [CloudFlare's SSL middle-manning][cloudflare_ssl].

[ghpages]: https://pages.github.com/
[hackartscience.com]: http://hackartscience.com
[jekyll]: https://jekyllrb.com/
[cloudflare_ssl]: https://konklone.com/post/github-pages-now-sorta-supports-https-so-use-it
[markdown]: http://kramdown.gettalong.org/
[gh-markdown]: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
