ITI - Docker Lab 🐋
Task 1: Working with Docker Hello-world Image
Objective
Learn how to run a container using the hello-world image and manage containers and images.

Steps
1. Run a Container with hello-world Image
   docker pull hello_world
   ![image](https://github.com/mennazm/docker-lab-day-1/assets/91394925/32a2977d-015d-49af-9c8d-1248be433f12)

   docker run hello-world
   docker ps -a
  
   
3. Check Container Status and Explain
4. Start the Stopped Container
5. Remove the Container
6. Remove the Image
Task 2: Running Container with Ubuntu Image
Objective
Run an Ubuntu container in interactive mode, create a file inside it, and manage containers.

Steps
1. Run Ubuntu Container in Interactive Mode
2. Create a File inside the Container
3. Stop and Remove the Container
4. Check File Status
5. What happened to hello-docker file?
6. Remove All Stopped Containers
7. Bonus: Remove All Containers in One Command
Task 3: Creating a Custom Nginx Docker Image
Objective
Create a custom Docker image using Nginx and a local HTML file.

Steps
1. Create a Local HTML File
2. Write Dockerfile and Copy the HTML file to the Docker Image
3. Run Container with New Image
4. Test the Container, open your browser and navigate to http://localhost:8088 to check if everything is okay
