Infrastructure setup
====================

This is just a readme file that specifies how to run these configurations in order to install stuff on my developer (and not only) machine.

Install Spark
-------------

This will download, copy to opt and install Spark. It will set the required environment variables, deploy the configs and start your master and slaves.

	ansible-playbook -i hosts playbooks/install_spark.yml --ask-sudo-pass --ask-pass

> Note: This setup is mostly written for running Spark on your local machine. You might need to modify these scripts a bit if you wish to run Spark on a cluster. Mostly the changes would be in the config files - the `slaves` config file should be populated and live only on the master.