---
layout: post
title: how to test jekyll website locally
---

>Test jekyll website just on GitHub Pages is unprofessional and can be dangerous. We highly recommend installing Jekyll to preview your site and help troubleshoot failed Jekyll builds.


Requirements
---

- *Install Ruby*: `$ sodu install ruby`

- *Install bundler*: `$ gem isntall bundler`

- *Update 'Gemfile' in foot directory*:

```
source 'https://rubygems.org'
gem 'github-pages', group: :jekyll_plugins
```

- *Install Jekyll and other dependencies from the GitHub Pages gem:*:`$ bundle install`

Test with your lcoal Jekyll site
---

- *Navigate to root directory:* `cd blog`

- *Run your Jekyll site locally:* `$ bundle exec jekyll serve`

    Navigate to: 'localhost:4200'

- **Recommend to use 'watch mood'** :

    ```
    $ jekyll server --watch
    ```

     Navigate to 'http://127.0.0.1:4000/` 

Keeping your site up to date
---
- *Add your changes and push to repo on GitHub*