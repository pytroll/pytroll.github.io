# pytroll.github.io

This is the placeholder for the static pytroll website.

## Jekyll Theme

This site uses the Jekyll "minima" theme version 3.0. You can find information
about how it was customized and how it should be used here:

https://github.com/jekyll/minima

Everything is configured in `_config.yml` and the theme is further customized
in the `_includes`, `_layout`, and `assets` directories. The current major
customization is adding anchor icons to each section header using anchorjs.

## Deployment

The site is built and deployed by the GitHub Actions workflow in
`.github/workflows/pages.yml` on every push to the `main` branch. Pull
requests are built, but not deployed, to check that the site still builds.
The repository's Settings -> Pages -> "Build and deployment" source must be
set to "GitHub Actions".

The site is built with Jekyll 4 and the gem versions in `Gemfile.lock`. Any
Jekyll plugins the site uses must be added to the `Gemfile` and to `plugins:`
in `_config.yml`.

## Local Development

To see what this website will look like in a local environment:

1. Create a conda environment with ruby installed (ruby 3.2 or newer is
   required, the GitHub Actions workflow uses 3.4):

   ```bash
   conda create -n pytroll_site "ruby>=3.2" compilers
   conda activate pytroll_site
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

To update the gems used to build the site run `bundle update` and commit the
updated `Gemfile.lock`.
