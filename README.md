# Note-App
This repo having Two-Tier application "Note-App".
1. Fronted & Backend - Python, HTML
2. Database - MySql

Dashboard of Note-App:

![Note-App](https://github.com/ashubambal/Note-App/assets/92073828/5543408f-2d28-4a3b-86bd-dc0cfb5d5989)

Step 1 : Clon this repo on your local machin.
	https://github.com/ashubambal/Note-App.git

Step 2 : Then use below command to run container
	docker-compose up

Step 3 : Now container is ready to use so issue below command and go inside the container.
	To check running container -> ubuntu@ip-x-x-x-x:~/Note-App$ docker ps
	To go inside the container -> ubuntu@ip-x-x-x-x:~/Note-App$ docker exec -it <container_id> bash
 
	Login to the MySQL database -> bash-4.2# mysql -u root -p
	Enter password: your_password
	Issue below command once you logon successfull.
		
  	mysql> USE your_database;
	mysql> CREATE TABLE messages (
	    		id INT AUTO_INCREMENT PRIMARY KEY,
   			message TEXT
		);

Step 4 : exit
