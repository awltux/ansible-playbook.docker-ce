# Deploy docker-ce and apply hardening.

Use generic Makefile and Vagrantfile to deploy docker-ce.
Make is the primary interface.

Default environment is vagrant but others could be added under the environment dir.
To start a Vagrant VirtualBox instance just run:
make vagrant-up

Once VM's have been started, apply the playbook using:
make vagrant-reload

Debug the deploy script using:
make debug=true vagrant-reload

Other environments could be added under the environment dir and deployed to directly.
make env_name=production ansible-deploy
