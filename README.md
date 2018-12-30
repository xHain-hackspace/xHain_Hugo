# xHain hack+makespace Homepage

[![wercker status](https://app.wercker.com/status/4374b5664faf5920c218c1b06618581a/m/master "wercker status")](https://app.wercker.com/project/byKey/4374b5664faf5920c218c1b06618581a)

https://www.x-hain.de

# Getting started

## Install Hugo

### Mac OS
* Install brew (for installing the rest): ``/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"``
* Install go: ``brew install go``
* Install hugo: ``brew install hugo``

### For Windows/Linux:
* Install hugo: [Hugo Website](https://gohugo.io)

## Pull Submodules (eg. Theme)
* Initial pull submodule xhain-theme: ``git submodule update --init --recursive``
* Submodule update: ``git submodule foreach git pull origin master``

## Generate Site
* Run hugo to generate HTML: ``hugo``
* Run hugo for local development: ``hugo server``

# Content Editing

## New Post
* create new post (using archetypes): ``hugo new post/title.de.md`` or ``hugo new post/title.en.md``
* just edit new post in the "content"-folder

## Add Images

tbd.

# Development

tbd.

**Submodules**
Theme Version: 1.0.0