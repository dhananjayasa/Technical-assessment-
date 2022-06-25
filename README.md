# Technical-assessment-
DevOps Task

# Challenge #1 - Three-Tier-Architecture : Terraform (IaC) has been used to create a sample 3 tier architecture.

# Challenge #2 - metadata_retrieval.sh -
There are several ways to query the metadata within an AWS instance's to obtain an output 
For example-

wget -q -O - http://169.254.169.254/latest/dynamic/instance-identity/document 

or 

curl -s http://169.254.169.254/latest/dynamic/instance-identity/document

The above basically prints as json format, however there are other ways to get specific values instead of json format, such as 

curl -s http://169.254.169.254/latest/meta-data/instance-id 

or 

wget -q -O - http://169.254.169.254/latest/meta-data/instance-id 


# Challenge #3 - Javascript is used to write script in order to key value in a nested object function. e.g : $ node nested-object.js
