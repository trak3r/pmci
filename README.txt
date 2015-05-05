WHAT ARE THE PREREQUISITES?

* A git-based Ruby on Rails project


HOW DO I INSTALL IT?

1. Clone this repository
2. Run it (preferally in a "screen" session for remote servers)


HOW DO I RUN IT?

From your repository directory:

<path_to_pmci>/ci <branch name> <another branch name> <...>

(Replace "<branch name>" with the branch name you want to test, like "master".)


WHAT DOES IT DO?

Every X seconds it compares the specified branch(es) to the remote repository.
If there are changes it pulls the new version and runs the tests.
If any tests fail, it e-mails you the output.
