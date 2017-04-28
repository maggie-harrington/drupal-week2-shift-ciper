## Shift Cipher: Planning
###### Epicodus Drupal Week 2 Independent Project - Module Development

### Project Setup

* Download Drupal 7 core zip at https://www.drupal.org/project/drupal/releases/7.54

* Unzip and move to Desktop, rename project folder

* Delete .gitignore

* From within project folder:
`cp sites/default/default.settings.php sites/default/settings.php`
`chmod -R a+w sites/default`

###### MAMP:

* Change document root to project folder, Apache Port: '8888' and MySQL Port: '8889', 'start servers'

###### phpMyAdmin:

* 'Databases' > 'Create database' (database name: 'cipher'; collation: 'utf8_general_ci') > 'Create'

* 'Privileges' > 'Add user' (username: 'cipher'; password: 'cipher'; host: select 'local') > 'Go'

###### Drupal Web Interface:

* localhost:8888/install.php

* 'Select an installation profile' (Standard') > 'Save and Continue'

* 'Choose language' ('English') > 'Save and Continue'

* 'Database configuration' (Database configuration: 'MySQL, MariaDB, or equivalent'; Database name: cipher; username: 'cipher': password: 'cipher') > 'Advanced Options' (Database host: '127.0.0.1'; Database port: '8889') > 'Save and Continue'

* 'Configure Site' (Site name: 'Shift Cipher'; e-mail: 'maggie.harrington@gmail.com') > 'Site Maintenance Account' (username: 'cipher'; password: 'cipher') > 'Server Settings' (Default country; Default time zone) > 'Save and Continue'


### Project Stages:

* Set up basic blank Drupal site.

* Create custom module shift_cipher:

  * Create custom form with 3 text inputs: shift value, direction, phrase.

  * Add redirect to success page to display output.

  * Add validation to all input fields.

  * Write shift cipher code.

* Export database at the end of project and include the .zip file in a db-backup folder within in the sites directory. Include it with your repository.

* Download database .zip from github and import with phpMyAdmin to test.

* Submit to Epicenter before 5 pm!
