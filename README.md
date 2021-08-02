<h1>Ruby-Capybara</h1>
Simple Repository Using Selenium WebDriver With Ruby-Capybara

STEP 1: Add in your BROWSERSTACK_USERNAME and BROWSERSTACK_ACCESSKEY in the config files both single.config and parallel.config. Alternatively you canexport the environment variables for the Username and Access Key of your BrowserStack account

export BROWSERSTACK_USERNAME= <BROWSERSTACK_USERNAME> export BROWSERSTACK_ACCESS_KEY= <BROWSERSTACK_ACCESSKEY>

STEP 2: To install in all the dependencies : bundle install

STEP 3: To run feature files in parallel, I have created task named all inside the Rakefile and i have passed in those profiles that I wished to execute in parallel
NAME OF PROFILES BEING PASSED IN all profile: parallel,parallel1
Feature files running in parallel : single.feature, single1.feature
 Command that could be used for execution of that profile is : rake -m all
