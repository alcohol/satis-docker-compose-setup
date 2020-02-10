# Satis Docker Compose Setup

A simple repository template that aids in reproducing Satis build issues.

## How-To

Follow these steps:

- `git clone <repository> <directory>`;
- `cd <directory>`;
- verify `.env` contents are correct;
- add your `satis.json`;
  - make sure `homepage` is set to `http://satis-repository`;
- add your `composer.json`;
- `docker-compose up -d`;
- `docker-compose run satis build satis.json output -vvv`;
- `docker-compose run composer install -vvv`.
