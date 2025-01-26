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
To stop the container, run this, docker compose down.

Step 7:
To remove everything in the container, run this:
docker compose down --volumes --rmi all OR
docker system prune -af [this remove everything and the container]

 
