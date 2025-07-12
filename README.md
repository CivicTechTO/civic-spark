# civic-spark

a static site for the civic-spark event

## Setup

1. **Install Ruby and Bundler**

Make sure you have [Ruby](https://www.ruby-lang.org/en/documentation/installation/) installed. Then install Bundler:

```sh
gem install bundler
```

If you find this command installs a version of bundler older than 2.6.9, you are likely using an obsolete version of Ruby. If you are using MacOS, the system Ruby version is too old to install the latest bundler, and it will fail to install the required gems. You will need to [install a newer version of ruby](https://www.moncefbelyamani.com/how-to-install-xcode-homebrew-git-rvm-ruby-on-mac/).

2. **Install Dependencies**

Navigate to the project directory and install the required gems:

```sh
bundle install
```

3. **Run the Local Server**

Start a local development server:

```sh
bundle exec jekyll serve
```

Or use [incremental regeneration](https://jekyllrb.com/docs/configuration/incremental-regeneration/), which is faster but not stable:

```sh
bundle exec jekyll serve  --incremental
```
