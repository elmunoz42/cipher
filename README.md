
## Description

Web App with custom module for encryption using custom forms with data validation.
This website was generated with [Drupal 7.54](https://www.drupal.org/project/drupal/releases/7.54).

## Server Ports:

Apache port set to 80
MySQL port set to 3306

## Planning

|Status| Objective |
|------|-----------|
|DONE| 1) Create vanilla Drupal 7 project.|
|DONE| 2) Create custom module with simple display test.|
|DONE| 3) Create a form with three fields: shift value, direction and phrase input.|
|TODO| Create the business logic for the cipher encryption.|
|TODO| Create logic for punctuation and exception handling.|
|TODO| Create display page by formatting the output. |

## Specifications
|Spec# | Behavior           | Input           |         Output |
|------|--------------------|-----------------|----------------|
|1     |User inputs a word and sees the resulting encrypted message| "hello" | "khoor"|

## Encryption Information
The encryption takes in three values: shift value, direction and phrase input to be encrypted.
The shift value is the number of places to shift each letter over.
If the shift direction is "right" then you will add the shift value. For example: "a" with a shift value of 1 and a direction of right would become "b". A shift direction of "left" with a shift value of 1 would turn "b" into "a".
If the shift amount takes you over the bounds of the alphabet then cycle back to the beginning. For example: a shift value of 3 with the direction of right would turn "z" into "c".
Any spaces or punctuation in the input phrase should be ignored and reproduced in the final result without being shifted.
Your final result should be in all lowercase.

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
