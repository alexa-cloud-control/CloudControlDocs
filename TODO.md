## The next steps...

### TaskCat

In order to properly run TaskCat for tests of infrasture and lambdas, it is needed to:  
* Run TaskCat as a Docker container
* Store, or send the summary files
* Refactor CF templates for parameters
* Be sure, all lambdas can be tested on infrastructure level
* Make possible to run the test in different regions

### Get rid of `sed` in travis config

This is more or less self-explanatory...

### Create proper lambda deployment handling

Currently code of lambda function is not redeployed, or deployed all the time. 
