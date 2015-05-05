WHAT ARE THE PREREQUISITES?

* A git-based Ruby on Rails project


HOW DO I INSTALL IT?

Clone this repository


HOW DO I RUN IT?

From inside your repository directory:

EMAIL=<your_email_address> <path_to_pmci>/ci <branch name <another branch name <...>>>

Replace "<branch name>" with the branch name you want to test, like "master".


WHAT DOES IT DO?

* Every X seconds it compares the specified branch(es) to the remote repository.
* If there are changes it pulls the new version and runs the tests.
* If any tests fail, it e-mails you the output.
