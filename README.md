# Azure-Bastion-Service

# What is Bastion Service?
- Provides seamless RDP/SSH to Virtual Machines from the Azure Portal via TLS
- When users need to RDP onto a machine, users would use the public IP.
- Instead of exposing the public IP, use Azure Bastion Service. It is more secure.
- It is a fully managed service, therefore, bastion service will create its own compute machines that will establish the connectivity within a subnet on the Virtual Network


# Use Case
- Create a vm with no public IP
- Create a subnet named AzureBastionSubnet for the Bastion Service and add a public IP
- Connect to the vm using Bastion Service


# Create a subnet for the Azure Bastion Service
- Users can either create a subnet within the Virtual Network or
- Create the AzureBastion Subnet via Bastion serivice
- Bastion service should have a public IP
<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/171086678-98811683-45ce-4407-ae5a-f71deb1b95f9.png" height="90%" width="90%" alt="front door"/>

<p/>


<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/171086721-f146ba82-4acc-43c2-8fb5-d08c987aa250.png" height="90%" width="90%" alt="front door"/>

<p/>

# Deply Bastion Service
- When deploying Bastion Service, it can create the AzureBastionSubnet
- Once created, users will be prompted to enter admin credentials

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/171086791-468e5117-6501-425d-bf97-ea614b73eaf0.png" height="90%" width="90%" alt="front door"/>

<p/>

# Connect successfully to the virtual machine via the Azure Portal
- Enter admin credentials
<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/171087826-fa54ecb4-1400-44bb-b46c-d61fe8558c7d.png" height="90%" width="90%" alt="front door"/>

<p/>

# Successfully connected via Bastion Service
- Note this VM does not have a public IP and is not internet-facing
- Bastion Service allows secure login from the Azure Portal

<p align="center">
  
<img src="https://user-images.githubusercontent.com/104326475/171087992-203624ba-14d1-4cdc-a8d3-198901226c03.png" height="90%" width="90%" alt="front door"/>

<p/>
