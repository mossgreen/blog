---
title: How to Test Jekyll Website Locally
search: true
categories: 
  - Jekyll
---


> Test jekyll website just on GitHub Pages is unprofessional and can be dangerous. We highly recommend installing Jekyll to preview your site and help troubleshoot failed Jekyll builds.


Requirements
---

- Install Ruby: `$ sodu install ruby`

- Install bundler: `$ gem isntall bundler`

- Update 'Gemfile' in project directory:

    ```
    source 'https://rubygems.org'
    gem 'github-pages', group: :jekyll_plugins
    ```

- In project directory, update dependencies:`$ bundle install`

Run it
---

- Navigate to root directory: `cd blog`

- Run your Jekyll site locally on 'watch mood': 

    ```yaml
    $ bundle exec jekyll serve --watch
    ```

- Navigate to: 'localhost:4200' or 'http://127.0.0.1:4000/'

- If you update something, when you hit "Save", it will automaticly update

End
---
- Add your changes and push to repo on GitHub