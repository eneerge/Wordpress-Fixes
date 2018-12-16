# Wordpress-Fixes

## Renaming wp-login.php causes redirect error when trying to login
Reproduce by:
1. Rename wp-login.php to something.php
2. Now when attempting to log in something.php, you will receive a redirect error (Error Too Many Redirects)

To temporarily fix:
1. Open dev-tools and change the <form> tag to post to something.php instead of the old wp-login.php

To perm fix:
1. Modify wp-login.php to pull the correct php page.
