# hunters sandbox

Instructions: 

* Get rid of Fish , if you have Fish installed in your terminal
* Install rvm and rails together in order.  RVM is Ruby Version Manager. ( rvm.io ) 
> \curl -sSL https://get.rvm.io | bash -s stable --rails 

* FOLLOW INSTRUCTIONS AFTER INSTALLING RVM 

* Verify that RVM is working: 
> rvm list 


* Fork and clone this repo 
* cd into directory
* Tell the app to use Ruby 2.2.3
> rvm use 2.2.3

* Install packages (dependencies)
> bundle install

* If the above installation fails, run the following two commands:
> gem install bundler
> gem install puma -v 2.13.4 --with-opt-dir=/usr/local/opt/openssl


* Auto generate databases 
> rake db:create
* Run the Rails app
> rails s

* If the app fails to start due to an incorrect version of ruby, ensure that it is using 2.2.3 
> rvm use 2.2.3
and issue the following command
> gem pristine —all

* Your app is now running but you won't be able to do anything if you don't run the migrations. 
* The error you get when you run the app should give you a clue as to how do migrations. 

* Go to Pivotal tracker to see the user stories to complete: 
https://www.pivotaltracker.com/n/projects/2065691

You won't be able to edit them or press "start", but you need to complete all stories. 
When finished, submit a pull request to the original repo here. 


