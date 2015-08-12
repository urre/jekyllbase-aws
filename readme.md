# Jekyllbase

Fork of my Jekyll starter [Jekyllbase](https://github.com/urre/jekyllbase). Jekyllbase AWS is for deploying your Jekyll site on Amazon S3. 

## Setup

Install Ruby Gems with Bundler

	bundle install 

Install NPM dependencies

	npm install

Install Bower dependencies

	bower install

## Develop

With a single command you have the site spinning locally at [http://localhost:3000/](http://localhost:3000/). [BrowserSync](http://www.browsersync.io) injects and reloads on file changes (Sass files, Markdown files and html files/includes).

    gulp

## Build

### Build for production for use on AWS or separate hosting/VPS. 

	gulp prod

Note: If using this alternative you can use Jekyll Assets for fingerprinted files. Include ``head-jekyll-assets.html`` and ``footer-jekyll-assets.html`` instead of ``head.html`` and ``footer.html`` in the default template

## Deploy

### Deploy to Amazon S3 (using [s3_website](https://github.com/laurilehmijoki/s3_website))

First read credentials via an ``.env`` file to ``s3_website.yml``. Don't version control your credentials.

	s3_website push