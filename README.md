## AWS CloudFormation Examples

Example template for configuring AWS autoscaling with ansible-pull via cloudformation

One template in the cf-templates folder
- elb-autoscaling-ansible-example-w-git-keys.json
- elb-autoscaling-ansible-example.json


For the example we're pulling the playbooks from the following repo
https://github.com/ansible/ansible-examples

You do need to specify the full path to the playbook for example
e.g /var/lib/playbooks/tomcat-standalone/site.yml


Based on the playbook you want to run, you'll also need to update the AnsibleHost parameter.  For example if you wanted to run the tomcat-standalone playbook, you'd use tomcat-servers, based on the site.yml playbook.


If you're experimenting with the git-keys version because eventually you want to use your own private bucket.

You will also need to update the MYBUCKET to point to you're own bucket and keys

No promises any of this will work for you.  Some tweaking may be needed.  
