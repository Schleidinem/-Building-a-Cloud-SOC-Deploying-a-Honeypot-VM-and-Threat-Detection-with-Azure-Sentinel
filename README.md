# 🚨 Building a Cloud SOC with Azure & Microsoft Sentinel  

## 📌 Project Overview  
This lab demonstrates how to set up a **home Security Operations Center (SOC)** in the cloud using **Azure** and **Microsoft Sentinel**.  
We configure a honeypot VM, forward logs to a central repository, and analyze **real-world attack data** with KQL queries and visualizations.  

## 🎯 Objectives  
- Deploy a honeypot VM in Azure  
- Configure a Log Analytics Workspace  
- Forward logs and integrate with Microsoft Sentinel  
- Query failed login attempts with KQL  
- Build an Attack Map to track real-time hacker activity  

## 🛠️ Tech Stack  
- Microsoft Azure (Free Subscription)  
- Virtual Machines (Windows Server)  
- Log Analytics Workspace  
- Microsoft Sentinel (SIEM)  
- KQL (Kusto Query Language)  
- PowerShell  

## 📂 Lab Steps  

1. **Azure Setup**
   
   - Created a Resource Group
     
<img width="975" height="413" alt="image" src="https://github.com/user-attachments/assets/38f1db11-9606-40a5-b9fb-e9917510cffd" />


   - Configured a Virtual Network
     
 <img width="975" height="326" alt="image" src="https://github.com/user-attachments/assets/08f57b7e-48b1-481b-80ca-cbc8c43c7793" />

 
   - Deployed a Virtual Machine (VM)
     
<img width="1364" height="535" alt="image" src="https://github.com/user-attachments/assets/e22f8acf-1f4f-4f1a-b446-f939d6e6887b" />

   - Added inbound security rule to allow internet traffic (honeypot setup)
     
<img width="975" height="391" alt="image" src="https://github.com/user-attachments/assets/e36ada44-07da-4327-a55a-5c35e9abc4b2" />

     
   - Disabled Windows Defender Firewall inside the VM
     
<img width="975" height="731" alt="image" src="https://github.com/user-attachments/assets/03109c8d-c411-4d72-959e-9c43ccb5a0a7" />

     
   - Verified connectivity via PowerShell (ping test)
     
<img width="975" height="500" alt="image" src="https://github.com/user-attachments/assets/13efcf8e-64c6-4765-bc41-4d654c9d39e3" />


2. **Log Repository & Sentinel**
   
   - Created a **Log Analytics Workspace**
     
 <img width="975" height="414" alt="image" src="https://github.com/user-attachments/assets/b48518cb-d9a6-4fb0-a0e2-23eb334b29e6" />

   - Connected VM to Log Analytics Workspace
     
  <img width="975" height="463" alt="image" src="https://github.com/user-attachments/assets/9924004e-9e93-478f-bfad-1b3e21a01080" />

  
   - Configured **Windows Security Events via AMA connector**
     
<img width="975" height="459" alt="image" src="https://github.com/user-attachments/assets/a2427039-4419-4706-b28c-044b533b8651" />

   - Integrated Sentinel with Log Analytics
     
<img width="975" height="463" alt="image" src="https://github.com/user-attachments/assets/dcb02a8c-8732-457f-bae5-634b1405a5a1" />


3. **Detection & Analysis**
    
   - Queried failed login attempts with **KQL**
     
<img width="975" height="438" alt="image" src="https://github.com/user-attachments/assets/a0684960-73fe-461d-97bf-4d15e1f38646" />

   - Created a **watchlist** in Sentinel for login attempts
     
<img width="975" height="450" alt="image" src="https://github.com/user-attachments/assets/572de23f-3aed-4734-9ae0-48113755571e" />

   - Built an **Attack Map** using Sentinel Workbooks to visualize attacker sources
     
<img width="1020" height="426" alt="image" src="https://github.com/user-attachments/assets/bcca68c4-5424-4a86-bb76-722d58a92d00" />
<img width="975" height="449" alt="image" src="https://github.com/user-attachments/assets/3144e2ad-9ccf-418b-93fe-8940e93a4779" />


  
## 📊 Results  
- Real-time attack data captured from exposed honeypot VM  
- Visualized failed login attempts and attack origins on an **interactive map**  
- Gained hands-on experience with SIEM and log analysis in Azure  

## 📜 Key Learnings  
- Fundamentals of cloud-based SOC setup  
- Using honeypots to collect real-world attack data  
- Practical SIEM skills with Microsoft Sentinel  
- KQL for log analysis and visualization  

---
