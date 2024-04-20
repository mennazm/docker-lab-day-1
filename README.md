# ITI - Docker Lab 🐋

## Task 1: Working with Docker Hello-world Image
### Objective
Learn how to run a container using the hello-world image and manage containers and images.

### Steps
#### 1. Run a Container with hello-world Image
```bash
  docker pull hello-world
  docker run hello-world

```
#### 2. Check Container Status and Explain
```bash
![image](https://github.com/mennazm/docker-lab-day-1/assets/91394925/d007f836-529f-41fd-8342-b92fbe9adf01)
![image](https://github.com/mennazm/docker-lab-day-1/assets/91394925/0c15e915-3946-40ea-97bc-1efedf575030)

its not running

```
#### 3. Start the Stopped Container
```bash
 docker start friendly_ellis
```
#### 4. Remove the Container
```bash
docker rm friendly_ellis

![image](https://github.com/mennazm/docker-lab-day-1/assets/91394925/80dd649a-1477-4a99-8bab-ce7fdcbc1512.)

```
#### 5. Remove the Image
```bash
```
docker rmi hello-world
![image](https://github.com/mennazm/docker-lab-day-1/assets/91394925/377d952b-9ed1-4529-b281-b2ee28c16cdd)

---

## Task 2: Running Container with Ubuntu Image
### Objective
Run an Ubuntu container in interactive mode, create a file inside it, and manage containers.

### Steps
#### 1. Run Ubuntu Container in Interactive Mode
```bash
```![image](https://github.com/mennazm/docker-lab-day-1/assets/91394925/6d593303-1275-4567-98e2-68d2a61f6e7c)
docker run -it ubuntu
#### 2. Create a File inside the Container
```bash
touch  hello-docker 
```
#### 3. Stop and Remove the Container
```bash
![image](https://github.com/mennazm/docker-lab-day-1/assets/91394925/96e7bcf8-5943-4c9c-bd0e-5a5414ca3ef7)
docker stop jolly_borg

docker rm jolly_borg
```
#### 4. Check File Status
```bash
not found
```
#### 5. What happened to hello-docker file?
```bash
not found
```
#### 6. Remove All Stopped Containers
```bash
![image](https://github.com/mennazm/docker-lab-day-1/assets/91394925/2bd1b3dc-755f-4fd0-b5b2-71343ba6c65c)

```
#### 7. Bonus: Remove All Containers in One Command
```bash
```
 docker container prune -f
---
## Task 3: Creating a Custom Nginx Docker Image
### Objective
Create a custom Docker image using Nginx and a local HTML file.

### Steps
#### 1. Create a Local HTML File
```bash
docker pull nginx


```
#### 2. Write Dockerfile and Copy the HTML file to the Docker Image
```bash
![image](https://github.com/mennazm/docker-lab-day-1/assets/91394925/4e85ae42-a27f-43ff-94a1-6f2b31df03ff)

```
#### 3. Run Container with New Image
```bash
![image](https://github.com/mennazm/docker-lab-day-1/assets/91394925/57beff08-4c20-4236-8c57-7fb3a9c0413a)

docker build -t custom-nginx .
```

#### 4. Test the Container, open your browser and navigate to http://localhost:8088 to check if everything is okay
```bash
![image](https://github.com/mennazm/docker-lab-day-1/assets/91394925/130a901d-e651-4554-a028-9673dd6c1df6)

```
