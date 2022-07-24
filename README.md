# Technical-assessment-
DevOps Task

# Challenge #1 - Three-Tier-Architecture : Terraform (IaC) has been used to create a sample 3 tier architecture.

# Challenge #2 - metadata_retrieval.sh -

#The script will give the result two ways-
• Running script without argument - In the script at line 14- if [ $# -eq 0] which means it will check to see if the argument has been passed along with script, if no arguments are passed to script, the conditions will satisfy, and the full metadata is displayed.

• Running script with argument - Passing the argument while running the script during runtime, example - sh metadata_retrieval.sh accountId or sh metadata_retrieval.sh accountId instanceId.

This argument will pass in the while loop and set the values in the key variable,(reference in the line number 7 key="$OPTARG" and if conditions not satisfy then else conditions passing as key to filter out the metedata. For example "$OPTARG" is the argument what we passing during running the script(accountId)


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
