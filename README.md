
## Description

Web App with custom module for encryption using custom forms with data validation.
This website was generated with [Drupal 7.54](https://www.drupal.org/project/drupal/releases/7.54).

## Server Ports:

Apache port set to 80
MySQL port set to 3306

## Planning

|Status| Objective |
|------|-----------|
|DONE| Create vanilla drupal 7 project.|
|TODO| Create custom module with simple display test.|
|TODO| Create a form with three fields: shift value, direction and phrase input.|
|TODO| Create the business logic for the cipher encryption.|
|TODO| Create logic for punctuation and exception handling.|
|TODO| Create display page by formatting the output. |


## Setup
1. Clone repository from https://github.com/elmunoz42/cipher.git
2. Set up connection to database system in MAMP (see bellow)
3. Import database from repo in phpMyAdmin (see bellow)
4. Create database admin in phpMyAdmin (see bellow)
5. Include settings.php with database access info

### Database connection
1. In MAMP > Preferences:
 - Apache Port: `80`
 - MySQL Port: `3306`
 - Document root: **`<repo_pathname>`**
2. Click 'Start servers'

### Import database
* Visit **`localhost:8888/phpMyAdmin`** in browser
* Click 'Import' tab
 - Character set: utf-8
 - File: **`<repo_pathname>/sites/db-backup/<backup_filename>`**

### Create database admin
* Visit **`localhost:8888/phpMyAdmin`** in browser
* Click 'Privileges' tab for `cipher`
* Add user
 - Name: `cipher`
 - Password: `cipher`
 - Host: Local
 - All privileges for `cipher`


## Technologies Used

* MySQL
* Drupal

## Drupal 7 Modules Used
* Cipher (custom module)

## Known Bugs

_No known bugs._

## Support

_Please contact elmunoz42@gmail.com with questions or concerns._

### License

*MIT License*

Copyright (c) 2017 _**Carlos Muñoz Kampff**_
