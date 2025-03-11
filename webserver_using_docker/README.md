in this project we implement CI/CD pipeline to host webserver using docker

first we create Dockerfile, html file and push it remote repo
![image](https://github.com/user-attachments/assets/be40b4c6-ada4-4f0a-b828-260584a7d40b)

install nginx, docker, jenkins for pipeline in your ec2 instances (you can use bash file to avoid manual task)

once jenkins installed make sure to give permission using command 
sudo usermod -aG docker jenkins (it adds jenkins user to docker group)

maintain credentials of git and dockerhub in jenkins for accessing git and dockerhub
![image](https://github.com/user-attachments/assets/a4c831f9-df7d-4670-ab4a-49c36760c6bb)

create a pipleine to clone repo, create docker image, push to dockerhub account and run container.

challenges:
since the contents is inside of another directory, it throws an error while creating docker image.
so modified the script by adding the source and build context
![image](https://github.com/user-attachments/assets/9b4b42dd-975c-4705-bda7-a03401654f00)

in Dockerfile port is mentioned so while creating container maintain the same port number

now build the pipeline 
![image](https://github.com/user-attachments/assets/c025d2a5-3bf2-4e11-babf-05c57157d310)


ypu can see the result by accessing the publicip with port 
![image](https://github.com/user-attachments/assets/d14edaa1-65ef-46e9-9053-7a5898add824)
