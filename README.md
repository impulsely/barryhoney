# Barry Honey, the bees knees

Barry Honey is a locally owned and operated apiary and honey business located in Fosters, Alabama.

## Running Locally

Make sure you have Python [installed properly](http://install.python-guide.org). Also, install the [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli) and [Postgres](https://devcenter.heroku.com/articles/heroku-postgresql#local-setup).

```sh
$ git clone git@github.com:impulsely/barryhoney.git
$ cd barryhoney

$ pipenv install

$ createdb barryhoney

$ python manage.py migrate
$ python manage.py collectstatic

$ heroku local
```

Your app should now be running on [localhost:5000](http://localhost:5000/).

## Deployment

First, push changes to github:

```sh
$ git add -A
$ git commit -m 'Meaningful message here'
$ git push origin master
```

Then open heroku.com and deploy from github.

This is a much cleaner deployment method than deploying directly to heroku from your local codebase.
