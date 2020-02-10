# Satis Docker Compose Setup

A simple repository template that aids in reproducing Satis build issues.

## How-To

Follow these steps:

- `git clone git@github.com:alcohol/satis-docker-compose-setup.git`
- `cd satis-docker-compose-setup`
- verify `.env` contents are correct
- add your `satis.json`
  - make sure `homepage` is set to `http://satis-repository`
- add your `composer.json`
  - make sure the `url` for your custom Composer repository is set to `http://satis-repository`
- `docker-compose up -d`
- `docker-compose run --rm satis build satis.json output -vvv`
- `docker-compose run --rm composer install -vvv`
