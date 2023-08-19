# ansible-task-2

Solution #1   - Using Dynamic Include

		 hosts
		 main.yml
			 - Debian.yml (Ubuntu Commands)
			 - RedHat.yml (CentOS Commands)

Solution #2 - Group Variables / Conditionals

		 group_vars/
			 centos:	apache_name: "httpd"
					 apache_user: “apache”
			 ubuntu:	apache_name: "apache2"
					 apache_user: “www-data”
		hosts
		main.yml
