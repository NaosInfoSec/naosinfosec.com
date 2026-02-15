# Hack Notes
This is my Hack Notes repository.

## Run in local

First install ruby.

    sudo pacman -S ruby base-devel ruby-erb

Then check the version

    ruby -v

Now ensure that it is in path, include in .bashrc or .zshrc

    export PATH="/home/<user>/.local/share/gem/ruby/3.4.0/bin:$PATH"

Install the bundler

    gem install bundler

Make bundle work with local setup noroot

    bundle config set --global path "$HOME/.bundle"

Now, ensure you are in the folder project

    cd <jekyll-project>

Install the gems

    bundle install

And run

    bundle exec jekyll serve