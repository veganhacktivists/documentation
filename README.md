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

# Development Workflow

When you have free time to volunteer with us and take on something to work on, please feel free to reach out to your PL. We're ecstatic to hear from you and would be happy to tell you what needs to be done and how we can help you out. We try to keep the Trello boards as up to date as possible but you're encouraged to ping if you want the most up to date info.

Here's our ideal workflow:

```bash
git checkout master
git pull
git checkout -b feature/my-trello-card
git add .
git commit -m "All my beautiful activism :D"
git push origin feature/my-trello-card
```

Then go to the repository, make your pull request, check the files over, assign your PL, and sit back and relax. 😎

If you see something that needs to be done while you're working on the code (e.g. a navbar doesn't look right, etc.), *please make a Trello card*. Keeping the Trello board and all the bugs current is difficult and it would incredibly help.

# General Troubleshooting

### Out of Memory During Composer Install
Please set the environment variable:
`COMPOSER_MEMORY_LIMIT=-1`
You may need to persist this in your `.bashrc` (or equivalent).
If you're wondering why this is happening... https://github.com/composer/composer/issues/1898

### Can't Migrate Database or Run Database Commands
Check your .env and make sure the password, username, hostname, etc. are all correct and the database exists.

### CSS doesn't show up properly.
Make sure you've run yarn install and yarn run watch and that those succeed.

# Resources

Here's some quick links for your reference that might help your activism: [Awesome Laravel](https://github.com/chiraggude/awesome-laravel)
