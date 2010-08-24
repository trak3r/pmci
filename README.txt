WHAT ARE THE PREREQUISITES?

* The Parallel Tests gem
* A git-based Rails project configured to work with the Parallel Tests gem


HOW DO I INSTALL IT?

1. Copy the "ci" script into the root of your Rails project.
2. Change the e-mail address in the script.


HOW DO I RUN IT?

./ci <branch name> <another branch name> <...>

(Replace "<branch name>" with the branch name you want to test, like "master".)


WHAT DOES IT DO?

Every X seconds it compares the local repository to the remote repository.
If there are changes it pulls the new version and runs Parallel Test.
If any tests fail, it e-mails the output to you.


WHY?

My test suite got so large it was taking over TEN MINUTES to run on my poor little Macbook Pro, so I incorporated the Parallel Test gem and set up a test environment on my 16-core staging server and saw the test time drop to LESS THAN ONE MINUTE.  So I wrote this little script to just loop forever, running tests and sending me reports when stuff breaks.