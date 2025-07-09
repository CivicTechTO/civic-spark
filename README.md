# civic-spark.ca

a static site for the civic-spark.ca event

## Setup

1. **Install Ruby and Bundler**

Make sure you have [Ruby](https://www.ruby-lang.org/en/documentation/installation/) installed. Then install Bundler:

```sh
gem install bundler
```

If you see that the version of bundler installed is lower than 2.6.9, you may need to update your bundler version:

```sh
bundle update --bundler
```

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
