## Setup the fabot project by Laravel

 Step 1: Open any project  VCS  Checkout from Version Control Git
 
 Step 2: Enter the project URL that is copied from GitHub, Project Name, then click OK
 
 Step 3: Type the command in the Terminal composer install 
 
 Step 3.a: When you get the  issue (facebook/webdriver 1.6.0 requires ext-curl * -> the requested PHP extension curl is missing from your system), run the following commands
 		   sudo apt-get update
 		   sudo apt-get install php7.1-curl (For those who uses php7.1)
 		   Then again run composer install

 Step 4: Now type the command in the terminal npm install (//Optional)
 
 Step 5: Run the command cp .env.example .env
 
 Step 6: Generate the key php artisan key:generate
 
 Step 7: Now set the database
 	    Create a database.sqlite file
 	    DB_CONNECTION=sqlite
 	    DB_DATABASE= Path of the database.sqlite file
 	    View -> Tool Windows -> Database -> Set up the sqlite connection
 Step 8: Run php artisan migrate
 
 Step 9: Run php artisan migrate:refresh --seed
 
 Step10: Views -> layouts ->app.blade.php -> Make sure it is flash.error
 
 Step 11: Run phpunit
 	