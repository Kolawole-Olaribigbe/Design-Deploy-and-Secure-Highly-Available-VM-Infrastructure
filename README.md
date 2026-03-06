# Design-Deploy-and-Secure-Highly-Available-VM-Infrastructure

Name: Kolawole Olaribigbe

Step 1: Create a resource group
<img width="1365" height="581" alt="Screenshot 2026-02-16 165917" src="https://github.com/user-attachments/assets/21b4ac18-97ca-48c2-a4d0-9c48e27533c6" />

Step two: Create a virtual network(Basic)
<img width="1365" height="575" alt="Screenshot 2026-02-16 171411" src="https://github.com/user-attachments/assets/96c2254b-284c-403d-828f-2eccfb1f31d1" />

Step 2: Create a virtual network(Security)
- Enable Azure Bastion
- Enable DDoS Protection
<img width="1365" height="444" alt="Screenshot 2026-02-16 171637" src="https://github.com/user-attachments/assets/26369993-587a-4c6b-9dc0-7b31095e25ea" />
<img width="1365" height="332" alt="Screenshot 2026-02-16 171659" src="https://github.com/user-attachments/assets/773057c4-4019-431c-9f6b-ac55cdf2ff83" />

Step 2: Create a virtual network(IP Address)
- Configure IP Address
<img width="1365" height="577" alt="Screenshot 2026-02-16 172614" src="https://github.com/user-attachments/assets/67c2638d-0161-4a36-9bff-3736a567446a" />

- Add Subnet for frontend
<img width="1126" height="514" alt="Screenshot 2026-02-16 172748" src="https://github.com/user-attachments/assets/8190dc69-4e85-4b26-9eb5-9fbcaf90f589" />

- Add Subnet for backend
<img width="1134" height="555" alt="Screenshot 2026-02-23 172659" src="https://github.com/user-attachments/assets/2590285c-8963-4b50-8cba-a69ee14577fe" />

- Review configuration
<img width="1363" height="575" alt="Screenshot 2026-02-16 172951" src="https://github.com/user-attachments/assets/2db02415-fac0-47a2-a50d-6aaf59ecf4af" />

- Deploy virtual network
<img width="1365" height="644" alt="Screenshot 2026-02-16 174011" src="https://github.com/user-attachments/assets/a0f560bf-bfbc-4ba6-8132-6bc4c767fcd4" />


Step 3(Basic): Create a Virtual Machine Scale Set for Frontend and Backend applications
<img width="1354" height="491" alt="Screenshot 2026-02-23 184025" src="https://github.com/user-attachments/assets/50ef0aba-6876-471f-8485-9a8a381dc44c" />
<img width="1326" height="544" alt="Screenshot 2026-02-23 184135" src="https://github.com/user-attachments/assets/2bd2c110-a74e-47e5-9b13-4ea7a68b69d2" />
<img width="1325" height="456" alt="Screenshot 2026-02-23 184240" src="https://github.com/user-attachments/assets/3d5b9e83-6440-41b9-abb3-e4016659478f" />


Step 3(Networking): Create a Virtual Machine Scale Set
<img width="1317" height="439" alt="Screenshot 2026-02-23 184913" src="https://github.com/user-attachments/assets/12fb82a6-49e2-4f96-afbe-fb174b9c7808" />
- Select Network Interface Card (NIC)
<img width="1313" height="495" alt="Screenshot 2026-02-23 200430" src="https://github.com/user-attachments/assets/020af30f-1cfb-4c2d-b7c4-196deeb535f1" />
- Create Load Balancer
<img width="1327" height="576" alt="Screenshot 2026-02-23 200840" src="https://github.com/user-attachments/assets/c5394dab-7067-4163-aff5-3bedfad6e72f" />


Step 3(Management): Create a Virtual Machine Scale Set
- Enable Boot diagnostics
<img width="1318" height="559" alt="Screenshot 2026-02-23 201027" src="https://github.com/user-attachments/assets/eb9afc7a-6030-41fe-a367-e3c8c6668ae1" />

- Configure Application Health Monitor
<img width="1340" height="569" alt="Screenshot 2026-03-02 161516" src="https://github.com/user-attachments/assets/ad6fd624-79a5-4e8e-9943-77eff56d3d10" />

Step 3(Review): Create a Virtual Machine Scale Set
- Review Configuration and create
<img width="1318" height="556" alt="Screenshot 2026-02-23 201311" src="https://github.com/user-attachments/assets/671e5034-e15c-4716-ad8f-89a909ac2957" />
Virtual Machine Scale Sets deployed
<img width="1032" height="425" alt="Screenshot 2026-02-23 201858" src="https://github.com/user-attachments/assets/b7d4ec1c-22b7-4e44-8527-2bc9db664092" />

Step 4: Configure Network Security Group(NSG)
- Open the newly deployed Virtual Machine Scale Set
<img width="1320" height="604" alt="Screenshot 2026-03-02 163939" src="https://github.com/user-attachments/assets/c58b598e-c42b-421b-ab4c-491ccd85ebb6" />

- From the side menu, navigate to "Networking" submenu
- Then click the "Network Settings" option
<img width="1319" height="613" alt="Screenshot 2026-03-02 164308" src="https://github.com/user-attachments/assets/0077562a-916d-4278-846f-db3e956b3257" />

- Configure the Network Security Group(NSG) Inbound rule
<img width="1330" height="607" alt="Screenshot 2026-03-02 164717" src="https://github.com/user-attachments/assets/cc55a733-6e03-4cfd-bc7d-595993147fbf" />

- Configure the Network Security Group(NSG) Outbound rule
<img width="1330" height="612" alt="Screenshot 2026-03-02 164912" src="https://github.com/user-attachments/assets/dcbbbdec-ea17-4e4a-af44-98d4ac082478" />

Step 5: Enable Just-in-Time (JIT) VM access
- Launch Microsoft Defender for Cloud service
<img width="1319" height="627" alt="Screenshot 2026-03-06 161218" src="https://github.com/user-attachments/assets/ecd1ed64-1329-4676-8992-904caaae79b3" />

- Navigate to "Environment Settings" in the "Management" submenu
<img width="1317" height="603" alt="Screenshot 2026-03-06 160853" src="https://github.com/user-attachments/assets/f9b3dcb7-4e9f-4319-b0d3-d88c42d1411e" />

- Select Subscription and turn on server protection
<img width="1324" height="620" alt="Screenshot 2026-03-06 161353" src="https://github.com/user-attachments/assets/c4b7c073-23a1-41d5-ab0b-3b5677e50f9c" />

- Navigate to the Virtual Machine Scale Sets
- Click on "Configuration" submenu in the "Settings"
- Enable Just-In-Time VM Access
 <img width="1324" height="610" alt="Screenshot 2026-03-06 161846" src="https://github.com/user-attachments/assets/c7125b11-f877-43d9-89f2-3a4e953de5e9" />

 - Go back to Microsoft Defender for Cloud
<img width="1343" height="620" alt="Screenshot 2026-03-06 162406" src="https://github.com/user-attachments/assets/a98f6de5-8e7c-46e2-bc13-43cd24bc4999" />

- Configure JIT VM Access
<img width="1332" height="626" alt="Screenshot 2026-03-06 162706" src="https://github.com/user-attachments/assets/684c1a31-7119-4742-8810-8e76c4c734f6" />

- Navigate to VMSS to request connection with JIT VM Access
<img width="1318" height="624" alt="Screenshot 2026-03-06 163142" src="https://github.com/user-attachments/assets/7a4232c1-528f-435d-a742-2f750e8b966c" />

- Navigate to the Network Security Group, to check if JIT Access NSG rule has been created
<img width="1322" height="612" alt="Screenshot 2026-03-06 163600" src="https://github.com/user-attachments/assets/9f67edb0-4e1c-435b-82cc-9a71808d1041" />

Step 6: Backup & Disaster Recovery
- Open the Recovery Services Vault service
- Create a Recovery Services Vault(Basics)
<img width="1325" height="560" alt="Screenshot 2026-03-06 193321" src="https://github.com/user-attachments/assets/7d63b791-aa9f-459a-b977-40192947ed68" />
- Create a Recovery Services Vault(Redundancy)
<img width="1272" height="565" alt="Screenshot 2026-03-06 193528" src="https://github.com/user-attachments/assets/6a0ec78a-30bb-46d9-9bf9-1bba28cf2df7" />
- Create a Recovery Services Vault(Encryption)
<img width="1324" height="576" alt="Screenshot 2026-03-06 193631" src="https://github.com/user-attachments/assets/4c1ca8c0-3551-49b5-9493-ce8213c2f3dc" />
- Create a Recovery Services Vault(Vault Properties)
<img width="1306" height="559" alt="Screenshot 2026-03-06 193819" src="https://github.com/user-attachments/assets/af6c470d-8410-4c4c-96e5-3b76caaa1232" />
- Create a Recovery Services Vault(Networking)
<img width="1301" height="570" alt="Screenshot 2026-03-06 193910" src="https://github.com/user-attachments/assets/0c155569-fe7b-463c-9b95-7e62a10b4779" />
- Create a Recovery Services Vault(Review and create)
<img width="1317" height="561" alt="Screenshot 2026-03-06 194017" src="https://github.com/user-attachments/assets/bb1dcb31-26a6-4c50-9149-3a5813c37bcb" />
- Recovery Services Vault created
<img width="1031" height="619" alt="Screenshot 2026-03-06 194529" src="https://github.com/user-attachments/assets/4987ff0b-ed5c-4a20-9a72-e6aa8302618b" />
- Go to newly created Recovery Services Vault resource
<img width="1321" height="631" alt="Screenshot 2026-03-06 194744" src="https://github.com/user-attachments/assets/8d2cfcce-35c7-45e0-852c-d491b48d6172" />
- Click Backup to configure
<img width="1327" height="598" alt="Screenshot 2026-03-06 200038" src="https://github.com/user-attachments/assets/77dcb30f-65ca-4220-832f-380ab7aba6fc" />
- Configure Backup Policy
<img width="1315" height="560" alt="Screenshot 2026-03-06 200301" src="https://github.com/user-attachments/assets/cd66d4c3-6c4c-4f96-9ea4-b364c2f42d5c" />
- Configure Backup frequency and retention
 <img width="1317" height="565" alt="Screenshot 2026-03-06 202300" src="https://github.com/user-attachments/assets/ad95e7c3-64a0-4f63-944d-6469bdd143f3" />
- Click Add to choose the Virtual Machine to bakup
<img width="1335" height="559" alt="Screenshot 2026-03-06 200633" src="https://github.com/user-attachments/assets/7ceadae3-6eba-463e-bd85-6b1a5f4d7ad1" />
- Backup complete
<img width="1030" height="638" alt="Screenshot 2026-03-06 201337" src="https://github.com/user-attachments/assets/f67c77c4-f1b0-47b8-9cb9-8d3120800132" />
- To confirm the Virtual Machine has been backed up
- Go to resource, on the menu expand "Protected Items" then click "Backup Items"
<img width="1341" height="614" alt="Screenshot 2026-03-06 201801" src="https://github.com/user-attachments/assets/c8933b7a-5260-4f53-b82b-c32e47ef3391" />
- Click Azure Virtual Machine
<img width="1334" height="572" alt="Screenshot 2026-03-06 201855" src="https://github.com/user-attachments/assets/68f26654-6555-4faa-a58b-fb9c1220d0ca" />
- Open context menu(...), select Backup Now
<img width="1324" height="604" alt="Screenshot 2026-03-06 203512" src="https://github.com/user-attachments/assets/26677a63-1663-454c-816d-06a8d73045f0" />
- Select backup date
<img width="1244" height="567" alt="Screenshot 2026-03-06 203709" src="https://github.com/user-attachments/assets/e007eee5-3e74-4236-a10b-ed9fc1bf6457" />

Step 7: Set up Azure Site Recovery for failover
- Go to the Resource Group
- Open the Virtual Machine Scale Set
<img width="1340" height="617" alt="Screenshot 2026-03-06 205813" src="https://github.com/user-attachments/assets/06954850-bb35-4c9c-9fd2-a7d711ab7a21" />
- Click "Backup + disaster recovery", then click "Disaster recovery"
<img width="1325" height="614" alt="Screenshot 2026-03-06 210348" src="https://github.com/user-attachments/assets/66887900-b325-4c40-8fcc-095728adf066" />
- Configure Disaster Recovery(Basics)
<img width="1321" height="540" alt="Screenshot 2026-03-06 210806" src="https://github.com/user-attachments/assets/d24fff0e-f5b8-4f98-9318-a3067b206175" />
- Configure Disaster Recovery(Advanced)
<img width="1323" height="611" alt="Screenshot 2026-03-06 210948" src="https://github.com/user-attachments/assets/9706f994-e2de-43d7-a69f-631d0692c115" />
- Configure Disaster Recovery(Review + Start replication)
<img width="1325" height="507" alt="Screenshot 2026-03-06 211459" src="https://github.com/user-attachments/assets/e638deae-1157-4408-adc9-c861b0241d15" />
<img width="1322" height="557" alt="Screenshot 2026-03-06 211534" src="https://github.com/user-attachments/assets/a58a951f-bbc0-4d75-a49a-ca0b9eb98d93" />




