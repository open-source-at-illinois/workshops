# Open Source at Illinois Workshop Page

This is the workshop page for Open-Source at Illinois. This is based off of the [Minima](https://github.com/jekyll/minima) Jekyll theme, on the dark skin.

### Adding workshops

Workshops are written as Markdown files.
To add a workshop, add a markdown page into `_posts` with the filename `YYYY-MM-DD-Your-Workshop-Title.md`, where `YYYY-MM-DD` is the date you would like to associate with your post.

If you would like to specify information about the specifc page/workshop, then include it between a pair of triple-dashes (this information is called [front matter](https://jekyllrb.com/docs/front-matter/)):
```
---
layout: post
title: Javascript Workshop
author:
- Person 1
- Person 2
---
```
Be sure to include `layout: post` so that the workshop is rendered correctly. To learn more, see the other posts in this repository, or see some of the [example posts](https://github.com/jekyll/minima/blame/master/_posts/2016-05-20-this-post-demonstrates-post-content-styles.md) on the Minima repository.

### Testing
To test how it will appear on the website:

(Note: you will need a [working ruby installation and you will need to install Jekyll on your computer](https://jekyllrb.com/docs/installation/).)

Run `bundle exec jekyll serve` and navigate to the URL that appears in the command line.


### Code Highlighting 

See [here](https://github.com/jekyll/minima/blame/master/_posts/2016-05-20-welcome-to-jekyll.md) for an example of how to implement code highlighting in blocks.
See [here](https://github.com/rouge-ruby/rouge/wiki/List-of-supported-languages-and-lexers) to see how to enable code highlighting for the language of your choice.
