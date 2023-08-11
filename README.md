# Note-App
This repo having two-Tier application called "Note-App".

1. Fronted and Backend: Python, HTML
2. Database: MySql

Dashboard of Note-App:

![Note-App](https://github.com/ashubambal/Note-App/assets/92073828/5543408f-2d28-4a3b-86bd-dc0cfb5d5989)

Step 1 : Clone this repo on your local machine or on an AWS EC2 instance.

	git clone https://github.com/ashubambal/Note-App.git

Step 2 : Use the "docker_installation_script.sh" script to install Docker on your local machine and then reboot the system.

	./docker_installation_script.sh
 	sudo reboot

Step 3 : Install docker-compose and then issue the docker-compose command to create the container.

	sudo apt install docker-compose -y
 	sudo docker-compose up -d

Step 4 : Now the container is ready to use, so issue the below command and go inside the container.
  
  	docker ps
	docker exec -it <container_id> bash
 	
Step 5 : Login to the MySQL database.

  	mysql -u root -p
	Enter password: your_password
	
Step 6 : Issue the below command once you logon successfully.
 
	USE your_database;
	CREATE TABLE messages (
	    id INT AUTO_INCREMENT PRIMARY KEY,
	    message TEXT
	);

Step 7 : Exit
