# pytroll.github.io

This is the placeholder for the static pytroll website.

## Local Development

To see what this website will look like in a local environment:

1. Create a conda environment with ruby installed:

   ```bash
   conda create -n pytroll_site ruby compilers ridk rb-inotify rb-jekyll rb-bundler
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
