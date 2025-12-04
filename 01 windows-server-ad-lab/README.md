# Windows Server + Active Directory Home Lab
## Objective

Deploy a functional Active Directory environment to practice user management, domain administration, troubleshooting, and enterprise IT support tasks.

## Tools Used

VirtualBox

Windows Server 2019/2022 ISO (Evaluation)

Windows 10 ISO

Microsoft RSAT Tools


### 1. Install VirtualBox/VMWare

Install with default settings

Confirm virtualization support is enabled in BIOS


<img width="1920" height="1080" alt="1" src="https://github.com/user-attachments/assets/6f063e71-2b48-4d86-9eb6-3abd0fe46921" />

<img width="1920" height="1080" alt="2" src="https://github.com/user-attachments/assets/732e4b9f-cb11-4c66-adeb-690d3553b334" />



### 2. Create Windows Server VM

Name: DC-Server

RAM: 4GB

Storage: 40GB

Attach Windows Server ISO

Install and configure Administrator password


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/16a518df-e63b-4549-abd5-689b2cdfdd58" />

<img width="1024" height="768" alt="3" src="https://github.com/user-attachments/assets/c5323ae1-e6c8-4701-b9ad-dc984ad4c20b" />

<img width="1024" height="768" alt="5" src="https://github.com/user-attachments/assets/c661fd20-5199-48fe-86c6-a120b0cda269" />

<img width="1024" height="768" alt="6" src="https://github.com/user-attachments/assets/66658ba0-3b3a-41f6-aa68-31c5d524bdb9" />


### 3. Install AD DS

Server Manager → Add Roles and Features

Install Active Directory Domain Services


<img width="1024" height="768" alt="7" src="https://github.com/user-attachments/assets/c86a3eb1-22b4-4b97-8559-f8bf54e1c3af" />

<img width="1024" height="768" alt="8" src="https://github.com/user-attachments/assets/21dc53b8-629f-402f-b4b7-d9ed6920e4c1" />

<img width="1024" height="768" alt="9" src="https://github.com/user-attachments/assets/456a659c-a45c-4f3a-abda-cdeaa03e05d7" />


### 4. Promote Server to Domain Controller

Choose Add a New Forest

Domain: myhomelab.local

Reboot


<img width="1024" height="768" alt="10" src="https://github.com/user-attachments/assets/6a7f654f-9404-4c01-ab18-956d9072b3b3" />

<img width="1024" height="768" alt="11" src="https://github.com/user-attachments/assets/ffed4b9b-2dfc-4140-92ff-747758593ef5" />

<img width="1024" height="768" alt="12" src="https://github.com/user-attachments/assets/99e5260d-56c7-4a0a-b957-9a3b642edc0b" />


### 5. Create OU, Groups, and Users

Open AD Users and Computers

Create users (ex. j.santos, m.reyes)

Create groups and assign membership


<img width="1024" height="768" alt="14" src="https://github.com/user-attachments/assets/982c1ecb-85ca-436c-bbc5-0ce2b91c051c" />

<img width="1024" height="768" alt="15" src="https://github.com/user-attachments/assets/8c74ebaf-dd6b-4916-9161-3a465864ded3" />

<img width="1024" height="768" alt="16" src="https://github.com/user-attachments/assets/42a13273-ec4b-4e09-b018-576b1d5aee0a" />

<img width="1024" height="768" alt="17" src="https://github.com/user-attachments/assets/0a789656-f3fa-44b4-8102-1ac87c8e38fb" />


### 6. Deploy Windows 10 Client VM

Install Windows 10

Set NIC to same network


<img width="1024" height="768" alt="19" src="https://github.com/user-attachments/assets/38f0081e-afe3-45c7-888a-f746f0ef67eb" />

<img width="1024" height="768" alt="20" src="https://github.com/user-attachments/assets/0482adcc-dd5d-4e64-9ce6-4b299c0009ce" />


### 7. Join Domain

System → Rename this PC → Join Domain

Use domain admin credentials


<img width="1024" height="768" alt="21" src="https://github.com/user-attachments/assets/26bc8cc5-0441-41d4-a12a-b13f9958bd83" />

<img width="1715" height="926" alt="22" src="https://github.com/user-attachments/assets/3bfc9344-faa1-4197-a167-5af4083a9cc1" />

<img width="1022" height="771" alt="23" src="https://github.com/user-attachments/assets/70b7e0eb-f791-4846-9e99-885964d1b1a5" />

### 8. IT Support Task Simulations

Password reset
Open Server Manager -> Click Tools -> Select Active Directory Users and Computers


<img width="1024" height="772" alt="1" src="https://github.com/user-attachments/assets/a6a5a53b-216d-4378-9bff-a17b38bc6f18" />


Selec the OU -> Search User -> Right Click - Choose Reset Password


<img width="1019" height="769" alt="2" src="https://github.com/user-attachments/assets/60e4a533-8166-4a9e-a8a3-b91b8e375200" />

<img width="1024" height="777" alt="3" src="https://github.com/user-attachments/assets/223afcc5-ffab-44dc-98d7-4fc4a8d1c5d1" />

<img width="1021" height="766" alt="4" src="https://github.com/user-attachments/assets/ac93cafe-981a-4a98-8e59-bdcbc2feec29" />

<img width="1019" height="729" alt="5" src="https://github.com/user-attachments/assets/e5712b6d-23cc-4b89-82b0-0fede2f8be8c" />

Unlock account

Change group membership

Folder permission management

Logon script testing



