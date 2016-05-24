# LAB7
Circular Replication
# Circular-Replication
	How to Install MariaDB 5.5 on Ubuntu
	##Step #1: Add the MariaDB Repository##
	
	  sudo apt-get install software-properties-common
	  sudo apt-key adv --recv-keys --keyserver hkp://keyserver.ubuntu.com:80 0xcbcb082a1bb943db
	  sudo add-apt-repository 'deb http://mirror.jmu.edu/pub/mariadb/repo/5.5/ubuntu trusty main'
	  sudo apt-get update
	
	##Step #2: Install MariaDB##
	  sudo apt-get install mariadb-server
	                          ###README###
	    ---After this operation, 116 MB of additional disk space will be used.---
	    #   Do you want to continue? [Y/n]                                      #
	    #   Enter Y to continue.                                                #
	    --------------------------------------------------------------------------
	    sudo service mysql stop
	    
	  ##Step 3: Configure and Secure MariaDB for Use##
	    sudo mysql_install_db
	    sudo service mysql start
	    sudo mysql_secure_installation
	         -----------------------------------###README###--------------------------
	            ---You’ll be prompted to enter your current password. Enter the root MariaDB password set during installation:--------
	            -  Enter current password for root (enter for none):                                                                 
	            -  Then, assuming you set a strong root password, go ahead and enter n at the following prompt:                      -
	            -  Change the root password? [Y/n] n                                                                                 
	            -  Remove anonymous users, Y:                                                                                        
	            -  Remove anonymous users? [Y/n] Y                                                                                   
	            -  Disallow root logins remotely, Y:                                                                                 
	            -  Disallow root login remotely? [Y/n] Y                                                                             
	            -  Remove test database and access to it, Y:                                                                         
	            -  Remove test database and access to it? [Y/n] Y                                                                    
	            -  And reload privilege tables, Y:                                                                                   
	            -  Reload privilege tables now? [Y/n] Y                                                                             
	         ------------------------------------------------------------------------------
	
	  ##Step 4: Verify MariaDB Installation##
	    You can check the version of the MariaDB installation with the following command:
	      mysql –V
	    Enter the MariaDB command client:
	      mysql –p
	      ##Enter password:##
	    Exit the command line with the following command:
	      Exit
	    To stop MariaDB:
	      sudo service mysql stop
	    To start MariaDB:
	      sudo service mysql start
	    To check the status of MariaDB:
	      sudo service mysql status
	    To restart MariaDB:






