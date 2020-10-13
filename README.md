# Vegan Hacktivists Documentation

<h4 align="center">Welcome to The Vegan Hacktivists 👋</h4>

# Tech Stack

This documentation should get you up and running with our tech stack:
Laravel (PHP) with best practices and as little as possible on top. Bootstrap or Tailwind (depending on the project, Tailwind for new projects).

For adding interactivity we use [Livewire](https://laravel-livewire.com/) and [Alpine.js](https://laravel-livewire.com/docs/2.x/alpine-js). If you're looking for examples of how to use these, check these out.
(https://www.alpinetoolbox.com/examples/)

# Running Laravel

### Start here.

Do you have Laravel set up for the code challenge or know *exactly* what you're doing? If so, skip this section. 🤠

Are you on Windows? Use this.

[Laravel Homestead](https://laravel.com/docs/8.x/homestead)

Do you have a Mac? Use this.

[Laravel Valet](https://laravel.com/docs/8.x/valet)

Are you on a Linux distribution? Use this.

[Laravel Valet Linux](https://cpriego.github.io/valet-linux/)

Are you a Docker person? Use this.

[Laradock](https://laradock.io)

Are you struggling to get the others set up and want something really easy (with the caveat that we can't really help much)?

[XAMPP](https://www.apachefriends.org/index.html)

# Building Our Projects

First check the README for the project you were assigned to. Likely there might already be something there.

Otherwise, here's the general process:

`.env` needs to be filled with your MySQL details.

```bash
cp .env-example .env
composer install
yarn install
yarn run watch
```

# General Troubleshooting
If you get an error about Composer running out of memory, please set the environment variable:
`COMPOSER_MEMORY_LIMIT=-1`
You may need to persist this in your `.bashrc` (or equivalent).
If you're wondering why this is happening... https://github.com/composer/composer/issues/1898
