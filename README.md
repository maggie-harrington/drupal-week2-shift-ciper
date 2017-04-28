# Shift Cipher

#### Epicodus Drupal Week 2 Independent Project - Module Development

#### _By Maggie Harrington_
##### _4-28-17_


## Description

##### _A basic Drupal site with a custom module which encrypts user input using a Shift Cipher. The form input is validated before the result is calculated._

##### Project Objectives/Requirements:

* Create a custom module that presents a form with 3 text inputs.
* One input should be a _shift value_, the second a _direction_, and the third the _phrase_ to be encrypted.
* Redirect user to a second page to show the result - the encoded phrase.
* The shift value is the number of places to shift each letter over.
* If the shift direction is "right" then you will add the shift value. For example: "a" with a shift value of 1 and a direction of right would become "b". A shift direction of "left" with a shift value of 1 would turn "b" into "a".
* If the shift amount takes you over the bounds of the alphabet then cycle back to the beginning. For example: a shift value of 3 with the direction of right would turn "z" into "c".
* Any spaces or punctuation in the input phrase should be ignored and reproduced in the final result without being shifted.
* Your final result should be in all lowercase.
* Be sure to validate all input before calculating the result. Here are the validation rules:
  * The shift value must be a positive integer.
  * The shift direction must be either "left" or "right".
  * The only special characters that should be allowed in your input phrase are spaces and punctuation.

##### This project demonstrates the following skills:

* Create a basic Drupal site.
* Create a custom module.
* Use forms to collect input.
* Use form validation.
* Redirect to a success page to display output.


###### Please see PLANNING.md in the root level of the project folder if you would like additional details on my process in creating this project.


## Setup/Installation Requirements

##### Requirements:

* MAMP (see https://www.mamp.info/en/downloads/ for installation details)


##### Clone Project:

* Open the terminal and enter `cd Desktop`

* Enter `git clone ` and copy/paste the project link: https://github.com/maggie-harrington/drupal-week2-shift-cipher

* Enter `cd drupal-week2-shift-cipher`


##### Import Database and Configure:

* In MAMP Preferences, change document root to project folder listed above. Make sure Apache Port is set to 8888 and MySQL Port is set to 8889.

* In your web browser, open phpMyAdmin: http://localhost:8888/MAMP/index.php?page=phpmyadmin&language=English

* Click the 'Import' tab, leave the default settings and make sure the character set is 'utf-8'.

* Click the 'Choose File' button next to 'Browse your computer' and navigate to sites/db-backup/cipher.sql.zip , then click 'Go'.

* Select the 'Privileges' tab and click 'Add User', then enter 'cipher' for both the username and password.

* Navigate to localhost:8888 in your web browser to view the project. (Make sure to keep the terminal window containing the server open while the project runs.)


## Support and contact details

If you run into any issues or have questions, ideas or concerns, please feel free to contact me at maggie.harrington@gmail.com


## Technologies Used

Written using Drupal, MAMP, phpMyAdmin, Atom, and Git.


## MIT License

Copyright (c) 2017 Maggie Harrington
