# GCEScripts
Ansible & Python Scripts To Manage Google Cloud Instances and Resources.


Useful links:

http://docs.ansible.com/ansible/latest/list_of_cloud_modules.html#google

https://cloud.google.com/compute/docs/tutorials/python-guide

http://docs.ansible.com/ansible/latest/guide_gce.html


Procedure:

Install Ansible

Install python

Install python-pip

Install libcloud ("sudo pip install apache-libcloud --upgrade")

Install/Upgrade requests module ("sudo pip install requests --upgrade")

Install/Upgrade pycrypto module ("sudo pip3 install pycrypto --upgrade") *REQUIRES THE WHOLE CONF ABOVE WITH PYTHON3

Set the global env variables:

GCE_EMAIL

GCE_PROJECT

GCE_CREDENTIALS_FILE_PATH in the /etc/environment file.

Copy the gce.py and the gce.ini file in the Ansible inventory directory, populate the gce.ini file with the env variables.

Launch gce.py --list to test the listing of the google cloud instances.


