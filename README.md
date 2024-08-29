This is an example of the dependant workflows for the GutHub Actions

Files description:
 - e2e-test-1 and e2e-test-2 files contains actual jobs setup for running the tests
 - e2e file defines the testing strategy and eligibility for the workflows to run
   It also conditionally runs the dependant workflow depending on the branch name
 - For the cases when different config files are defined for the different environments 
   this workflow is checking the ref name and generating the correct name for the Cypress config