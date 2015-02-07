## Introduction

This site includes a wiki of various How-Tos created by @pastcompute.
* The articles cover all manner of unrelated things that I had to at some point and may need to again, or I think other people might find useful.
* They are written fairly non-verbosely; this site is designed to be a memory jogger for performing various technical tasks, rather than explaining how
* Some will be referenced from my blog, [blog.oldcomputerjunk.net](http://blog.oldcomputerjunk.net), the blog article will probably describe why or how 

Visit: http://pastcompute.github.io

### Notes

#### Installing github-pages on Debian Wheezy

```
sudo apt-get install ruby-dev -twheezy
sudo gem install github-pages
sudo gem install bundler
```

#### Creating a new github-pages

Ref: https://pages.github.com/
Ref: https://help.github.com/articles/creating-project-pages-manually/

1. Create a repository, e.g. https://github.com/pastcompute/pastcompute.github.io
2. Hello world is simply `index.html`

* For _project_ pages, the second reference states to use a banch called `gh-pages`.
* Github pages are rendered from `master` branch and parsed through Jekyll
* Jekyll can be disabled by creating a root file called .nojekyll

#### Pages syntax

Pages need the triple dash prefix

```
    ---
    title: This is my title
    layout: post
    ---
```

#### Local testing

Run `bundle exec jekyll serve` and go to http://localhost:4000

