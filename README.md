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

## How to initialise

```
bundle add jekyll --version 3.8.5 # The version is taken from githubs recomendations
bundle exec jekyll new . --force # Force since there is already this file in the dir
```

Commit the changes to \_config.yml. Some extra files are generated that are not
needed (example .md files etc.).

See here: https://jekyllrb.com/tutorials/using-jekyll-with-bundler/
and here: https://help.github.com/en/github/working-with-github-pages/creating-a-github-pages-site-with-jekyll


## Start it

```
bundle install
bundle exec jekyll serve
```

## Updating with bundle


```
bundle update github-pages
```
