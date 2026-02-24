# Design-Deploy-and-Secure-Highly-Available-VM-Infrastructure

Name: Kolawole Olaribigbe

Step one: Create a resource group
<img width="1365" height="581" alt="Screenshot 2026-02-16 165917" src="https://github.com/user-attachments/assets/21b4ac18-97ca-48c2-a4d0-9c48e27533c6" />

Step two: Create a virtual network(Basic)
<img width="1365" height="575" alt="Screenshot 2026-02-16 171411" src="https://github.com/user-attachments/assets/96c2254b-284c-403d-828f-2eccfb1f31d1" />

Step two: Create a virtual network(Security)
- Enable Azure Bastion
- Enable DDoS Protection
<img width="1365" height="444" alt="Screenshot 2026-02-16 171637" src="https://github.com/user-attachments/assets/26369993-587a-4c6b-9dc0-7b31095e25ea" />
<img width="1365" height="332" alt="Screenshot 2026-02-16 171659" src="https://github.com/user-attachments/assets/773057c4-4019-431c-9f6b-ac55cdf2ff83" />

Step two: Create a virtual network(IP Address)
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


Step three(Basic): Create a Virtual Machine Scale Set for Frontend and Backend applications
<img width="1354" height="491" alt="Screenshot 2026-02-23 184025" src="https://github.com/user-attachments/assets/50ef0aba-6876-471f-8485-9a8a381dc44c" />
<img width="1326" height="544" alt="Screenshot 2026-02-23 184135" src="https://github.com/user-attachments/assets/2bd2c110-a74e-47e5-9b13-4ea7a68b69d2" />
<img width="1325" height="456" alt="Screenshot 2026-02-23 184240" src="https://github.com/user-attachments/assets/3d5b9e83-6440-41b9-abb3-e4016659478f" />


Step three(Networking): Create a Virtual Machine Scale Set
<img width="1317" height="439" alt="Screenshot 2026-02-23 184913" src="https://github.com/user-attachments/assets/12fb82a6-49e2-4f96-afbe-fb174b9c7808" />
- Select Network Interface Card (NIC)
<img width="1313" height="495" alt="Screenshot 2026-02-23 200430" src="https://github.com/user-attachments/assets/020af30f-1cfb-4c2d-b7c4-196deeb535f1" />
- Create Load Balancer
<img width="1327" height="576" alt="Screenshot 2026-02-23 200840" src="https://github.com/user-attachments/assets/c5394dab-7067-4163-aff5-3bedfad6e72f" />


Step three(Management): Create a Virtual Machine Scale Set
- Enable Boot diagnostics
<img width="1318" height="559" alt="Screenshot 2026-02-23 201027" src="https://github.com/user-attachments/assets/eb9afc7a-6030-41fe-a367-e3c8c6668ae1" />


Step three(Review): Create a Virtual Machine Scale Set
- Review Configuration and create
<img width="1318" height="556" alt="Screenshot 2026-02-23 201311" src="https://github.com/user-attachments/assets/671e5034-e15c-4716-ad8f-89a909ac2957" />
First Virtual Machine Scale Set deployed
<img width="1032" height="425" alt="Screenshot 2026-02-23 201858" src="https://github.com/user-attachments/assets/b7d4ec1c-22b7-4e44-8527-2bc9db664092" />


