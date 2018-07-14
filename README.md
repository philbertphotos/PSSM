# Password Manager

##### A Standalone Self Service Web Application for Changing Passwords in Active Directory

## Features
 * Lets users change and reset their passwords without the involvement of administrators.
 * Users have to go to a link sent to their email address to reset their forgotten passwords.
 * Generate strong passwords with the press of a button.
 * Enforce minimal password strength for new passwords.
 * Many configuration options to fine tune the application.

# Requirements

* PHP 5.6+ on the webserver.
* The PHP module for the database you wish to use must be installed on the webserver:
* MySQL/MariaDB
* Access to a mail server for sending emails.

**Note**: The application has currently **NOT** been tested with Microsoft SQL Server databases. In theory, it should work, because the simple select/update and function syntaxes are similar. Though I would appreciate it if anyone can confirm that it does.

# Installation

* Download the latest version of the application from the GitHub repository.
* Fill the [config.php](config.php) file with your configuration details.
* If using functions for database interactions, create them in the database.
 * [Definition examples of the functions used by the applications can be found here.](db_function_examples.md)
* Upload the application's files to the webserver.
* Optional but suggested: move the [config.php](config.php) file outside of the webserver's public directory and store the absolute filesystem path to it in the [configlink.php](configlink.php) file.

# [License](LICENSE)

Password Manager is released under the MIT license.
