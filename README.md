# Odd Profile

This profile is used as the base profile for all of our Drupal 10/11 sites.
This profile contains base functionality needed on most websites.

## Getting started

The best way to use this profile is to install it with the help of composer.

```
composer require oddhill/oddprofile
```

## Configuration files

Run the following commands to remove any site specific information from the
configuration files when they have been changed.

```
find ./config/install/ -type f -exec sed -i '' '/^uuid: /d' {} \;
find ./config/install/ -type f -exec sed -i '' '/_core:/{N;d;}' {} \;
```
