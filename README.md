Infrastructure setup
====================

This is just a readme file that specifies how to run these configurations in order to install stuff on my developer (and not only) machine.

Install Spark
-------------

This will download, copy to opt and install Spark. It will set the required environment variables and you should be up and running with a local
installation of Spark. 

	ansible-playbook -i hosts playbooks/install_spark.yml --ask-sudo-pass