# Personal website - al-folio template

Preparation to install

```
sudo apt-get install ruby-full
conda install jupyter
vi $HOME/.bashrc
export GEM_HOME=$HOME/.gem
source $HOME/.bashrc
```

Install

```
gem update --system
BUNDLE_FORCE_RUBY_PLATFORM=1 bundle install
```

How to build a local site

```
bundle exec jekyll serve
# if the site is not autoregenerated when making changes, try
bundle exec jekyll serve --force_polling --livereload
```

---

If there is an error when installing `mini_racer`, see https://github.com/alshedivat/al-folio/issues/691

```
vi Gemfile
# comment out mini_racer
sudo apt-get install nodejs
sudo apt-get install imagemagick
```
