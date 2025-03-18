we create 2 EC2 instances, 1 acts as master where jenkins is installed and 2nd as agent to execute builds
![image](https://github.com/user-attachments/assets/e51bb9d8-dc77-4c9b-8400-fc6f92e80e71)
![image](https://github.com/user-attachments/assets/0550940e-1487-4fe9-b75d-a2d65399ef58)

now let's install jenkins and dependencies in the master instance using the bash file jenkins.sh.

![image](https://github.com/user-attachments/assets/d33f04b7-b021-4969-92d4-037def7efdd1)

setting up jenkins
![image](https://github.com/user-attachments/assets/11a0cb80-d804-4b36-9f28-a42349b8808d)
creating jenkins agent
![image](https://github.com/user-attachments/assets/42c95472-5c23-41a1-98c2-2826cc18c6ca)
![image](https://github.com/user-attachments/assets/175c8b8c-725c-4614-bd76-c726297d8015)

now copy this code and paste in node system
![image](https://github.com/user-attachments/assets/dd54129a-bfb0-4eb2-ba9c-042f71bc7ea1)
agent connected
![image](https://github.com/user-attachments/assets/05e5efbf-0277-4ae2-b60c-6422db0b706e)

now lets execute basic build using pipeline in master system


build success in agent system
![image](https://github.com/user-attachments/assets/0f1e988c-ff12-4ac7-a53a-9d5090876221)




