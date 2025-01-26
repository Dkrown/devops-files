# devops-files
Devops projects

Step 1:
Install Docaker locally.

Step 2:
Clone this repo and run this: docker build -t my-jenkins .

Step 3:
'cd' into 'devops-file' directory.

Step 4: Start jenkins, run this: docker compose up -d

Step 5:
Open jenkins web UI [http://localhost:8080].

Step 6:
Run this command in the terminal to get the jenkins password after the web UI loaded:
docker exec -it my-jenkins bash [this command ope a shell inside 'my-jenkins' container.

Step 7:
Inside the shell [my-jenkins container], run this command to get the password and copy it:
cat /var/jenkins_home/secrets/initialAdminPassword

Step 8:
Exit the 'my-jenkins container', by run this:
exit

Step 9:
To stop the container, run this, docker compose down.

Step 10:
To remove everything in the container, run this:
docker compose down --volumes --rmi all OR
docker system prune -af [this remove everything and the container]

 
