## Rangsiman Ketkaew's website.

https://rangsimanketkaew.github.io

#### Running a website locally

I do not recommend installing ruby directly via `apt-get` or `brew`. I suggest using `rbenv` instead to manage the version of ruby.

```sh
# Linux (Ubuntu)
sudo apt-get install rbenv
# macOS:
brew install rbenv ruby-build

# Install ruby and set the version
rbenv init
rbenv install 3.2.3
rbenv global 3.2.3  # (for this machine)
rbenv local 3.2.3   # (for this directory)

# Instlal bundler
gem install bundler

# Build website
cd rangsimanketkaew.github.io
bundle install
bundle exec jekyll server

# Build website with google analytics included
# (google analytics tag will be included in index.html of the built site)
JEKYLL_ENV=production bundle exec jekyll serve
```

#### Q&A

- If you have error about loading bundle, please remove all old versions of gem using `gem cleanup` and then run `gem install bundler` again.

- I suggest adding the following command `eval "$(rbenv init - zsh)"` to an environment script, e.g., `.zshrc` for macOS.
