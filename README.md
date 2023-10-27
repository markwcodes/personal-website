# Personal Website App

### 🚧 This site is under construction 🚧

Please see the [infra repo](https://github.com/markwcodes/personal-website-infra) for everything **infrastructure** and **platform** related to this project.

[![CI Status](https://github.com/markwcodes/personal-website/actions/workflows/ci.yml/badge.svg)](https://github.com/markwcodes/personal-website/actions)

## Overview

[mark.wilson.codes](https://mark.wilson.codes) was created to provide an online presence and as a demonstration of DevOps and web development skills. There will be a strong focus on DevOps and back-end web development, with a few interactive demos down the line.

The name also tells you who I am and what I do!

For the web framework, I have chosen [Laravel Jetstream](https://jetstream.laravel.com) as it provides out-of-the-box user authentication, easy Vue prop hydration via Inertia.js, and back-end routing handled by Laravel.

Cost is a key consideration, and therefore I have chosen to use DigitalOcean as my cloud environment. A similar setup on AWS would be around 5x the cost of DigitalOcean.

## Setup Instructions

### Running the site locally

This site runs locally in docker utilising configuration from [Laravel Sail](https://laravel.com/docs/sail).

1. Copy the environment file example `.env.example` to `.env`
2. Install php/composer locally, and run `composer install`
3. Add the `sail` alias to your .zshrc/.bashrc file:\
   `alias sail='[ -f sail ] && sh sail || sh vendor/bin/sail'`
4. Configure and bring up your docker containers:

``` bash
sail up && \
sail artisan key:generate && \
sail artisan migrate && \
sail npm install && \
sail npm run dev
```

5. Edit your `/etc/hosts` file and add\
   `127.0.0.1  markwcodes.test`
6. The site should now be accessible at [markwcodes.test](http://markwcodes.test)
