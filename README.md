# Open Source at Illinois Workshop Page

This is the workshop page for Open-Source at Illinois. This is based off of the [Minima](https://github.com/jekyll/minima) Jekyll theme, on the dark skin.

### Adding workshops

Workshops are written as Markdown files.
To add a workshop, copy `TEMPLATE.md` in `_workshops` as a new file. Be sure to change the filename to something appropriate for your workshop (the shorter, the better), and fill out the entries of the workshop.

### Testing
(You don't need to do this, but if you want to, here're the instructions)

You will need a [working ruby installation and you will need to install Jekyll on your computer.](https://jekyllrb.com/docs/installation/)

Before all, in your workshop file, add the line `published: true` in between the two triple-dash lines, like so:

```
published: true
title: "My workshop"
# stuff...
```

Then, run `bundle exec jekyll serve` and navigate to the URL that appears in the command line.


### Code Highlighting 

See [here](https://github.com/jekyll/minima/blame/master/_posts/2016-05-20-welcome-to-jekyll.md) for an example of how to implement code highlighting in blocks.
See [here](https://github.com/rouge-ruby/rouge/wiki/List-of-supported-languages-and-lexers) to see how to enable code highlighting for the language of your choice.
