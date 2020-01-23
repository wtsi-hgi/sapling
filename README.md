This is an Ansible playbook which fetches a chunk of mpistat data from S3 and automatically runs a Treeserve instance on it. In order to work, the following variables have to be declared in the shell environment:
 - `S3_AWS_ACCESS_KEY` : `access_key` in `.s3cfg`
 - `S3_AWS_SECRET_KEY` : `secret_key` in `.s3cfg`
 - `S3_GROUP_NAME` : The name of the Unix group whose mpistat data should be fetched from S3
 - `S3_SANGER_URL` : `host_base` in `.s3cfg`

 `python-pip` needs to be installed on the host for the playbook to work. 
