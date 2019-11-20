# My website

This website uses the [Agency Jekyll theme](https://github.com/y7kim/agency-jekyll-theme).

# Setup

## Installing bundle (to be able to install jekyll)

```
sudo pacman -S ruby
```

```
gem update
gem install bundle
```

Add this to .zshrc:
```
export PATH=$PATH:$HOME/.gem/ruby/2.6.0/bin
```

## Setup bundle

```
bundle init
bundle install --path vendor/bundle
```

## Start the page

```
bundle update
bundle install
bundle exec jekyll serve
```

## How the initialisation of the repo was made (for documentation only)

```
bundle add jekyll --version 3.8.5 # The version is taken from githubs recomendations
bundle install
bundle exec jekyll new . --force # Force since there is already this file in the dir
rm 404.html about.md index.md _posts/*welcome-to-jekyll.markdown
```

Commit the changes to \_config.yml. Some extra files are generated that are not
needed (example .md files etc.).

See here: https://jekyllrb.com/tutorials/using-jekyll-with-bundler/
and here: https://help.github.com/en/github/working-with-github-pages/creating-a-github-pages-site-with-jekyll


