# A shiny new website!
The World Wide Web hypertext repository for [cscabal.com](http://cscabal.com)

# How to Write Posts

## Getting Started

- Install Ruby
    - This will come with `gem`
- `$ gem install bundler`
    - If you already had `bundler` installed, run `gem update bundler` - we need at least v1.14
- `$ bundle install`
- Add yourself to the `authors` section of `_config.yml`

## Creating a New Page

In the `_posts` directory, create a new file fith the name in the following format: `YYYY-MM-DD-title-here.md`.
At the top of the file, add and fill in the following header:

```
---
author: erik
title: My First Post
---

# Markdown Goes Here
```

## Running the Site Locally

```
$ bundle exec jekyll serve
```

This will serve the website at [http://127.0.0.1:4000](http://127.0.0.1:4000)
