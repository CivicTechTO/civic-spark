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

Additional System Dependency: `libvips` `jekyll_picture_tag` depends on `libvips` for image processing. You’ll need to install it before running Jekyll locally.

If using **macOS**, you can get libvips from [homebrew](https://brew.sh)

```sh
brew install vips
```

For **Windows** or otherwise, please resolve and update the readme with your method.

3. **Run the Local Server**

Start a local development server:

```sh
bundle exec jekyll serve
```

Or use [incremental regeneration](https://jekyllrb.com/docs/configuration/incremental-regeneration/), which is faster but not stable:

```sh
bundle exec jekyll serve  --incremental
```

---

## Image Gallery and Lightbox

The documentation page has been configure with jekyll_picture_tag for responsive, lazy-loaded documentation images, and BaguetteBox.js for lightbox navigation.

### Adding Documentation Images

Place images in: `assets/documentation/` They will automatically appear in the gallery on the wrap-up page (wrapup.md). Filenames are sorted reverse alphabetically. See the include: [gallery.html](_includes/gallery.html) for the configuration.
