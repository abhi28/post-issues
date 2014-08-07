Php Script to create gitHub and BitBucket issues using APIs

It contains a Php script that is used to post issues to GitHub and BitBucket repositories by calling the APIs provided by GitHub and BitBucket respectively. The script can be extended to include other repositories as well by creating a class and a function to post issue for that repository.

Download the Php script from github repository

Setup Instructions

    Save the php file and then open command prompt. Go to the root folder of Php in wamp directory where php.exe file is present. Alternatively, if the environmental variable for php is set in the system then this is not required. Php.exe file is normally present in<Drive in which wamp is installed>\wamp\bin\php\<phpversion> eg: C:\wamp\bin\php\php5.3.8

    Use the following command to execute the script php.exe -f username <username> password <password> <"Issue Title"> <"Issue Description"> eg: php.exe -f C:/Users/abhi/Desktop/postIssues.php username abhi password secret https://github.com/example/test "My Issue Title" "These are the steps required" Script can also be executed by using the command : php.exe -f after step 1 and then manually entering the input parameters from the command line.

NOTE: This script uses CURL to connect to APIs, Please uncomment the extension=php_curl.dll extension in the php.ini file for windows and/or use the following commands in Linux(Ubuntu) sudo apt-get install php5-curl sudo /etc/init.d/apache2 restart to enable this script to execute
