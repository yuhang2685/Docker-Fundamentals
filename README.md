## Docker-Fundamentals
Introduction to Docker | Installation | Basic Commands

Author: Dr. Yuhang Zhao

### 1. What is Docker?
`Docker` is software container platform.

Where does `Docker` operate?:
`Deployment` stage among the stages of `Design` / `Development` / `Deployment` / `Testing` / `Release`.

Nowadays software has many components (Front-end / Back-end / DB / Dependencies). 
It is requrired to run in many different platforms (which has its own configurations, e.g., OS, installed libraries, dependenies).

Hopefully you may have seen "shipping containers" before.
Similarly, developer packs up an app with all it needs, such as libraries and other dependencies as one package.
`Docker` is responsible for shipping the package to different platforms and run.


### 2. How Docker works?

![HowDockerWorks](https://github.com/yuhang2685/Docker-Fundamentals/blob/master/How%20Docker%20works.png)

- `Dockerfile` - Describes steps to create a `Docker image`. It is like a recipe with all ingredients and steps necessary in making your dish.
- `Docker image` - Contains app requirements and dependencies. They are templates used to create `Docker containers`.
- `Docker container` - Runtime instance of `Docker image`. Run `Docker image` to obtain it.
- `Docker Hub` - Online cloud repository for `Docker images`.

`Docker images` can be pulled to Test Environment or Staging Environment.
The app is ensured to behave same in different environments.

#### Note the difference to virtual machine:
![DiffToVM](https://github.com/yuhang2685/Docker-Fundamentals/blob/master/VM%20and%20Docker.png)

- `VM`: There are multiple VMs in the hosting server, each has its OS and fixed resource allocation. Overhead.
- `Docker`: There are multiple containers where each has app and dependencies / libraries.

#### Client-server architecture:

"`commond line interface - Docker Deamon`" which enables containers to be manipulated through commands / `RESTful API`.

### 3. What are benifits of Docker?
#### 1. Build only once:
An application inside a container can run on "ANY" system has Docker installed.
No need to build and configure application for different platforms.

#### 2. Portability:
Can be run on `local system`, `Amazon ec2`, `Google Cloud`, `VirtualBox`...

#### 3. Version Control:
Has build in version control system allowing to commit changes to image.

#### 4. Isolation:
Application works on its own container, and does not interferes with others.

### 4. Installation:
Following the installation steps in 
"Docker Beginner Tutorial 5 - How to install DOCKER on WINDOWS ? Step by Step" 
by Automation Step by Step - Raghav Pal.
https://www.youtube.com/watch?v=ymlWt1MqURY

#### Validate installation:

In `Docker terminal`, run 
- `docker --version`

![HowDockerWorks](https://github.com/yuhang2685/Docker-Fundamentals/blob/master/Docker%20Installed.png)

- `docker run hello-world`

![HowDockerWorks](https://github.com/yuhang2685/Docker-Fundamentals/blob/master/Hello-world.png)

- `docker images`

![HowDockerWorks](https://github.com/yuhang2685/Docker-Fundamentals/blob/master/Docker%20Images.png)

### 5. Basic commands:
See "Docker Basic Commands" 
by Automation Step by Step - Raghav Pal at
https://www.youtube.com/watch?v=HqBMEmoAd1M

Another good resource is "Exploring Docker [1] - Getting Started" by Traversy Media at https://www.youtube.com/watch?v=Kyx2PsuwomE

### Reference:
"Docker Beginner Tutorial", by Automation Step by Step Raghav Pal.
https://www.youtube.com/watch?v=wi-MGFhrad0&list=PLhW3qG5bs-L99pQsZ74f-LC-tOEsBp2rK
