## Rangsiman Ketkaew's website.

https://rangsimanketkaew.github.io

<br>

```sh
# Linux (Ubuntu)
sudo apt-get install ruby ruby-full
# macOS:
brew install ruby

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

If you have error about loading bundle, please remove all old versions of gem using `gem cleanup` and then run `gem install bundler` again.
