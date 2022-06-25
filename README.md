# Technical-assessment-
DevOps Task
# metadata_retrieval.sh -
There are several ways to query an instance's metadata and obtain an output in AWS.
For example-
wget -q -O - http://169.254.169.254/latest/dynamic/instance-identity/document 
or 
curl -s http://169.254.169.254/latest/dynamic/instance-identity/document

The above basically prints as json format, but there are other ways to get specific values instead of json format, such as 
curl -s http://169.254.169.254/latest/meta-data/instance-id 
or 
wget -q -O - http://169.254.169.254/latest/meta-data/instance-id 
