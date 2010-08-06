WHAT ARE THE PREREQUISITES?

* The Parallel Tests gem
* A git-based Rails project configured to work with the Parallel Tests gem


HOW DO I INSTALL IT?

Copy the "ci" script into the root of your Rails project.

***
*** CHANGE THE E-MAIL ADDRESS IN THE SCRIPT TO *YOUR* E-MAIL ADDRESS
***


HOW DO I RUN IT?

./ci master

(replace "master" with the branch name you want to test.)


WHAT DOES IT DO?

Every X seconds it compares the local repository to the remote repository, and if there are changes it pulls the new version and runs Parallel Test.


WHY?

My test suite got so large it was taking over ten minutes to run on my pool little Macbook Pro, so I added the Parallel Test gem to my project and set up a test environment on my 16-core staging server and watched the testing time drop to less than one minute.