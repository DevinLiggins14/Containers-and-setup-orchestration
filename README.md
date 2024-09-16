# Containers-and-setup-orchestration
<h2>Description</h2>
The purpose of this project is to demonstrate how to setup Docker containers as well as handling container orchestration with Kubernetes
<br />
<p align="center">
<img src="https://github.com/user-attachments/assets/c88ff460-84c8-42f7-867d-8438f9811b6b"/>

<h2>Languages and Utilities Used</h2>

Bash, Docker, Kubernetes 

<h2>Environments Used </h2>

- <b>CentOS Linux release 8.5.2111
 10</b>

<h2>Project walk-through:</h2>
<p align="center">
Download the necessary docker packages : <br/>
<img src="https://github.com/user-attachments/assets/082acfbd-2abe-4cea-a7ab-209d7f847c98"/>
<br /> <br />Run the command docker --version to confirm <br />  
<br />
   <br/> Start and enable Docker service <br/> 
<img src="https://github.com/user-attachments/assets/50f5c106-6f09-45fa-a8c9-786676ebf8df"/>
<br />
<br />Now create and move into a directory that will contain the dockerfile for the webapp <br/>
 <br/>
<img src="https://github.com/user-attachments/assets/36e6af31-ed51-4f28-aebd-02b8caffe146"/>
<br />
<br /> Create a docker file with the following contents <br/> 
 <br/>
 <img src="https://github.com/user-attachments/assets/be3e4748-a46b-4590-a161-b8fc45291117"/>
<br/>
 Using an official Python 3.8 slim image, the provided Dockerfile ensures a lightweight runtime environment. The working directory inside the container is set to /usr/src/app, and all files from the current directory are copied there. To enable access from the host system to the web server of the container, port 8000 is left open. The command python -m http.server 8000 instructs the container to launch a basic Python HTTP server on port 8000 when it starts up. This configuration offers an easy way to test and launch a simple web application and is perfect for serving static web content.
 <br/> <br/>
<br/>

<br/>Add an index.html file in the current dir to add the webapp contents <br/>
<img src="https://github.com/user-attachments/assets/eadeb66c-1c8e-41a9-9e7a-f93e4e28a7c3"/>
<br/>
<br/>
<br/>Run docker build -t webapp_image . to create a docker image out of the dockerfile <br/> 
<br/>
<img src="https://github.com/user-attachments/assets/74cf0348-1000-4e6f-a3d0-688967f08eb0"/>
   <br/>
   <br/> Confirm the newly created docker image <br/> 
   <br/>
   <br/>
<img src="https://github.com/user-attachments/assets/fa42daea-298b-4472-9e67-e4e0d9554735"/>
<img src="https://github.com/user-attachments/assets/9866c694-1aa8-463f-9b7c-d9baed2fc0ed"/>
<br />
<br />
<br/> Run a container using the webapp image and mapping ports to expose 8000 <br/>
<img src="https://github.com/user-attachments/assets/ad463dc0-1c68-4614-be77-dc7ab6c438e2"/>
<br/>
 <br/> Type http://<YOUR_SERVER_IP>:8000 into the search bar to view the app! <br/>
<img src="https://github.com/user-attachments/assets/7f696e1d-5676-4064-af1f-06d7b7e3d86c"/>
<br />
<br />
 <br/>
<img src=""/>   <br/>
<img src=""/>
<br />
<br />
 <br/>
<img src=""/>
<img src="/>
<br />
<br />
 <br/>
<img src=""/>   <br/>
<img src=""/>
<br />
<br />
 <br/>
<img src=""/>
<img src="/>
<br />
<br />
 <br/>
<img src=""/>   <br/>
<img src=""/>
<br />
<br />
 <br/>
<img src=""/>
<img src="/>
<br />
<br />
 <br/>
<img src=""/>   <br/>
<img src=""/>
<br />
<br />
 <br/>
<img src=""/>
<img src="/>
<br />
<br />
 <br/>
<img src=""/>   <br/>
<img src=""/>
<br />
<br />
 <br/>
<img src=""/>
<img src="/>
<br />
<br />
 <br/>
<img src=""/>   <br/>
<img src=""/>
<br />
<br />
 <br/>
<img src=""/>
<img src="/>
<br />
<br />
 <br/>
<img src=""/>   <br/>
<img src=""/>
<br />
<br />
 <br/>
<img src=""/>
<img src="/>
<br />
<br />
 <br/>
<img src=""/>   <br/>
<img src=""/>
<br />
<br />
 <br/>
<img src=""/>
<img src="/>
<br />
<br />
 <br/>
<img src=""/>   <br/>
<img src=""/>
<br />
<br />
 <br/>
<img src=""/>
<img src="/>
<br />
<br />
 <br/>
<img src=""/>   <br/>
<img src=""/>
<br />
<br />
 <br/>
<img src=""/>
<img src="/>
<br />
<br />
 <br/>
<img src=""/>   <br/>
<img src=""/>
<br />
<br />
 <br/>
<img src=""/>
<img src="/>
<br />
<br />
 <br/>
<img src=""/>   <br/>
<img src=""/>
<br />
<br />
 <br/>
<img src=""/>
<img src="/>
<br />
<br />
 <br/>
<img src=""/>   <br/>
<img src=""/>
<br />
<br />
 <br/>
<img src=""/>
<img src="/>
<br />
<br />
 <br/>
<img src=""/>   <br/>
<img src=""/>
<br />
<br />
 <br/>
<img src=""/>
<img src="/>
<br />
<br />
 <br/>
<img src=""/>
