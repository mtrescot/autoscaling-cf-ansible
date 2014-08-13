## AWS CloudFormation Examples

Example template for configuring AWS autoscaling with ansible-pull via cloudformation

One template in the cf-templates folder
- elb-autoscaling-ansible-example-w-git-keys.json


For the example we're pulling the playbooks from the following repo
https://github.com/ansible/ansible-examples

You do need to specify the full path to the playbook
e.g /var/lib/playbooks/tomcat-standalone/site.yml

You'll also need to update the MYBUCKET to point to you're own bucket and keys

No promises any of this will work for you.  Some tweaking may be needed.  
