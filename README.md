# Open Source at Illinois Workshop Page

This is the workshop page for Open-Source at Illinois. This is based off of the [Minima](https://github.com/jekyll/minima) Jekyll theme, on the dark skin.

### Workshop Submission process
- Fork the repository and clone your own forked repository.
- Add a workshop by following the instructions in "Adding workshops" below.
- Submit a pull request to get it published!

### Adding workshops
First, make sure you are NOT the master branch. This is because the submission process gets way messier if you directly make commits to master. You can do this by running this in the terminal in the repo:

```
# Example if you're making a workshop on cooltech
git checkout -b cooltech-workshop
```

(Feel free to name your branch something appropriate.)

Then, to actually add a workshop, copy `TEMPLATE.md` in `_workshops` as a new file. Be sure to change the filename to something appropriate for your workshop (the shorter, the better), and fill out the entries of the workshop. When you're done, add the file, commit it, push it to your fork, and open up a PR!

If you have any questions about the process or would like help, send a message into the Discord.


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
