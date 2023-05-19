# pytroll.github.io

This is the placeholder for the static pytroll website.

## Jekyll Theme

This site uses the Jekyll "minima" theme version 3.0. You can find information
about how it was customized and how it should be used here:

https://github.com/jekyll/minima

Everything is configured in `_config.yml` and the theme is further customized
in the `_includes`, `_layout`, and `assets` directories. The current major
customization is adding anchor icons to each section header using anchorjs.

## Local Development

To see what this website will look like in a local environment:

1. Create a conda environment with ruby installed:

   ```bash
   conda create -n pytroll_site "ruby<3.0" compilers
   conda activate pytroll_site
   gem install rb-inotify jekyll
   ```

2. Install the current site "package"

   ```bash
   bundle install
   ```

3. Run the development server:

   ```bash
   bundle exec jekyll serve
   ```

4. Open your browser and go to "localhost:4000".


Note: We must use ruby 2.6+ as the current version of github pages (225) has
dependencies that are 2.6+. We also don't explicitly install `rb-bundler` as
we used to because it is vendored into conda-forge's version of ruby 2.6.

