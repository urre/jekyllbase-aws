# Jekyllbase AWS

Fork of my Jekyll starter [Jekyllbase](https://github.com/urre/jekyllbase). Jekyllbase AWS is for deploying your Jekyll site to Amazon S3. 

## Features

Like my [Jekyllbase](https://github.com/urre/jekyllbase) but with the addition of using the Jekyll plugin [Jekyll Assets](https://github.com/jekyll-assets/jekyll-assets) (Assets pipelines for Jekyll). Used for nice finger printed assets.

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

### Build for production 

For use on [Amazon AWS](http://aws.amazon.com) on a S3 bucket. (Or host it your self on a VPS. I recommend [digitalocean.com](http://digitalocean.com))

	gulp prod


## Deploy

### Deploy to Amazon S3 (using [s3_website](https://github.com/laurilehmijoki/s3_website))

First read credentials via an ``.env`` file to ``s3_website.yml``. Do not version control your credentials.

	s3_website push