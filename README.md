Jenkins is using an official Jenkins image from dockerhub.

The goal is to create a basic jenkins repository that I can reference in the future for usability.

## Getting your docker image from Github

# Step 1

Create a new folder and turn it into a git repository
> git init

# Step 2

Add a remote branch.  Git remote add origin (URL link found in the code section of Github).

# Step 3

Git fetch and pull the branch.

# Step 4

With Docker Desktop installed, open up Powershell as admind and run:
> wsl --unregister docker-desktop

# Step 5
Run Docker Destop as admin and go into the terminal on the ower righthand of the screen.

# Step 6
Navigate to the directory containing your pulled repository.  You may need to change drives depending on where you stored it.

Local C Drive:
>cd theDirectoryContainingYourRepository

On a different drive (d for example):
>d:
>cd theDirectoryContainingYourRepository

# Step 7
Ensure that you are in the repository you pulled by checking for the docker-compose.yml file.

# Step 8
Run the docker compose command.
>docker compose up

# Step 9 
Go to the containers section of the Docker Desktop application and select jenkins_testing.  Click the dropdown menu.

# Step 10
Notice that there are two ports.  Select http://localhost:8080/ and copy paste that link into your main browser.

# Step 11
It will walk you through account setup.  If you need to enter the directory of the active run the following in the Docker Application Terminal: 
> docker exec -it <container_name> bash

# Step 12 
You may be asked to locate the password or secret credentials at the browser screen.  Locate that directory by finding it inside of the directories contained within the docker in the step above.

# Step 13 
Log in and enjoy using Jenkins from this Docker setup.

## Getting your docker image from DockerHub

Coming Soon...  An alternative way to pull the image.  Straight from DockerHub.
