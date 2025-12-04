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




