# 2.Scalable-Web-App-with-NLB-and-Auto-Scaling


##  Project Overview
This project demonstrates a **high-performance and low-latency scalable web application** using AWS services. It uses a Network Load Balancer (NLB) to efficiently handle large volumes of traffic with minimal delay.

---

##  Objective
To build a system that:
- Handles **very high-performance traffic**
- Provides **ultra-low latency**
- Automatically scales EC2 instances based on demand

---

## AWS Services Used

- :contentReference[oaicite:0]{index=0} – Hosts the web application  
- Network Load Balancer – Handles high-speed traffic with low latency  
- Auto Scaling Group – Automatically manages EC2 instances  
- Security Groups – Controls access and traffic rules  

---

## Architecture Overview

User → Network Load Balancer → Target Group → EC2 Instances (Auto Scaling Group)

---

## Implementation Steps

1. Auto Scaling Group
- Created launch template
- Configured min, max, desired capacity
- Attached scaling policy

<img width="602" height="79" alt="Picture2 2" src="https://github.com/user-attachments/assets/bc7301f1-04a5-4b35-969e-54198cf94401" />

<img width="602" height="268" alt="Picture2 1" src="https://github.com/user-attachments/assets/7d864677-2be4-4c13-8517-2c5b9d2fb4a1" />

<img width="631" height="190" alt="Picture2 4" src="https://github.com/user-attachments/assets/9d6e58a2-508a-4646-a00f-14ca9e8ec9aa" />


2. Target Groups
- Created target group for EC2 instances
- Registered instances automatically

<img width="602" height="95" alt="Picture2 3" src="https://github.com/user-attachments/assets/64c6773a-6e26-4f9c-aa02-cab8bd286d93" />



Output

- Application successfully running via **NLB DNS**
- Traffic distributed efficiently with **low latency**

<img width="810" height="188" alt="Screenshot 2026-04-29 145104" src="https://github.com/user-attachments/assets/fec73e97-d2c4-4384-80cf-5ec4cf266ae6" />

<img width="802" height="198" alt="image" src="https://github.com/user-attachments/assets/347ee3f3-d8de-4cd2-9cd1-1b0781f2ca61" />

<img width="798" height="195" alt="image" src="https://github.com/user-attachments/assets/255e5bb6-bc30-4385-8c69-e57c5665668b" />
