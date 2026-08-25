*Project Objective

This project demonstrates how internet traffic reaches an EC2 instance through different AWS VPC networking components.

Architecture Flow
Internet User
     ↓
Internet Gateway
     ↓
Network ACL
     ↓
Route Table
     ↓
Security Group
     ↓
EC2 Instance

Step 1 : AWS account
*lunch VPC in aws :<img width="1600" height="739" alt="vpc lunch 2" src="https://github.com/user-attachments/assets/498c0d0d-1e5e-4241-b492-0d6727db6734" />
<img width="1600" height="739" alt="vpc lunch 1" src="https://github.com/user-attachments/assets/c9d025a1-d5ad-4064-a9e4-6daf6947802c" />
<img width="1600" height="753" alt="VPC LUNCH" src="https://github.com/user-attachments/assets/c5d42e0e-ad68-4376-90a5-960f4d1c394e" />
<img width="1600" height="643" alt="defaut creat by awsn1" src="https://github.com/user-attachments/assets/6e02cad5-a834-4799-b6b3-c78aaa169cc7" />
<img width="1600" height="594" alt="defaut creat by aws" src="https://github.com/user-attachments/assets/b00fccc9-81d4-4988-95d2-f49830689002" />

after the lunch by default the aws will create (Internet Gateway ,subnets private and public ,Route Tables)
*lunch EC2 Instances connect to ubuntu linux 
command 
chmod 400 ~/exaple.pem
ssh -i your-key.pem ubuntu@EC2_PUBLIC_IP
sudo apt update
python3 -m http.server 8000
  Security Group :<img width="1920" height="799" alt="{7F5ED93D-8788-4B84-A688-CC55DC101772}" src="https://github.com/user-attachments/assets/5364c40c-cdc1-4d00-a3d5-689a2af654ed" />
 output:<img width="697" height="468" alt="output" src="https://github.com/user-attachments/assets/b7ce53cd-b217-4bf0-8859-3b49c7f6bbfd" />
 now lets contral in Network ACL level:<img width="1600" height="703" alt="Nacl1" src="https://github.com/user-attachments/assets/070ff0dd-147d-43da-b3e3-fe63dfa620fe" />
 <img width="1600" height="655" alt="NAcl2" src="https://github.com/user-attachments/assets/68be1742-a3f2-4a1a-bbc1-c888b3925dad" />
 output : <img width="697" height="468" alt="output" src="https://github.com/user-attachments/assets/92735797-b04a-4dd2-9565-42aab2e57d9e" />






