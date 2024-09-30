# DevOps-Project-Bank-Application-Blue-Green-Deployment-Azure

Architecture diagram for project is shown below.

![image](https://github.com/user-attachments/assets/28116f75-c8c7-421a-b605-ba4b4a6f8c55)

Architechture diagram for Blue-Green deployment is shown below.

![image](https://github.com/user-attachments/assets/5038ed97-33cf-496d-bd82-81c867db6921)
![image](https://github.com/user-attachments/assets/31c6f8ad-1965-4831-928c-31692815a88d)
![image](https://github.com/user-attachments/assets/518aa884-6fe3-455c-9245-85de41f6af1f)

The source code was present in Azure Repos as shown in the screenshot attached below.
![image](https://github.com/user-attachments/assets/728b2ac6-f0df-4b17-b2a0-f864a45e1a6d)

Created Azure Artifacts Feed with the name of bankapp and provided contributor permission on it. Updated the pom.xml as shown in the screenshot attached below.

![image](https://github.com/user-attachments/assets/3b940c48-1d13-4ca8-9332-87c1200b7c19)

Service Connection has been created for SonarQube, Maven Azure Artifacts Feed and Docker Registry as shown in the screenshot attached below.

![image](https://github.com/user-attachments/assets/5d5a1636-8e38-4ec1-9817-ba6674f7343a)

Two Azure Pipelines has been created as shown in the screenshot attached below.

![image](https://github.com/user-attachments/assets/720c7d06-4bd2-4c6d-a9c0-fda6d6a3247a)

Access the Application after running the two Azure Pipelines are as shown in the screenshot attached below.

![image](https://github.com/user-attachments/assets/5bb12fe6-30c1-4d66-9d15-6a5400f9dc3d)
![image](https://github.com/user-attachments/assets/9b2fa119-7486-4996-a1c9-ea3649f5ec01)

Application Pod, Deployment and Service will be created as shown in the screenshot attached below.

![image](https://github.com/user-attachments/assets/82efd285-9442-4f47-a651-dad3e388ed65)

As per the requirement the login page (login.html) of the Bank Application has been changed and its name is changed from Goldencat to GoldenHawk and bankapp Azure Pipeline has been run. 
We can get the rollout and list the multiple versions of it as shown in the screenshot attached below.

![image](https://github.com/user-attachments/assets/7f308ccc-6904-4cfb-abf2-f6086dee5721)

For checking purpose I have changed the service type of bankapp from ClusterIP to LoadBalancer as shown in the screenshot attached below.

![image](https://github.com/user-attachments/assets/5070aa82-3244-47f6-80dc-999753d9fa7b)
![image](https://github.com/user-attachments/assets/0b076844-21d9-4b79-a8b8-4663c51d8335)

After checking when you get assured Application is working fine, changed the service type from LoadBalancer to ClusterIP as shown in the screenshot attached below.

![image](https://github.com/user-attachments/assets/a7ef5221-dfdd-4335-8961-6e064293292a)

Finally promote the rollout as shown in the screenshot attached below.

![image](https://github.com/user-attachments/assets/6cfd5362-c4e2-45cd-b8e0-bb8fd2e38dcb)

List the Rollout for stable and preview status as shown in the screenshot attached below.

![image](https://github.com/user-attachments/assets/978a4774-25ea-47f9-a616-a442096feba6)

Finally access the application as shown in the screenshot attached below.

![image](https://github.com/user-attachments/assets/62858b32-12c6-4626-8b44-5750564b8da5)
![image](https://github.com/user-attachments/assets/9602530d-819b-4718-bf31-9f0667df88f1)

After running the Azure pipelines the screenshot for SonarQube and Azure Artifacts are as shown in the screenshot attached below.

![image](https://github.com/user-attachments/assets/2a038c68-c52d-4cf1-be04-7d9a15ee190c)
![image](https://github.com/user-attachments/assets/b31f4941-faac-49a3-83bd-3d8a85f9ce55)

<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
```
Source Code:- https://github.com/singhritesh85/Bank-App.git

Helm Chart:-  https://github.com/singhritesh85/helm-repo-for-Blue-Green-Deployment.git
```
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
```
Reference:-  https://github.com/Goldencat98/Bank-App.git
```
