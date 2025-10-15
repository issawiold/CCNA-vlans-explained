# CCNA VLANs Explained

VLANs are used to segment networks, improving performance and security.

\>en  
\#conf t  
fig#vlan 10 (any number you want 1-1001)  
vlan#exit  
fig#vlan 20  
vlan#name (name it what you want)  
vlan#exit  

Assigning VLANs to Ports:

- **To an endpoint:**  
  fig#int f#/# (port to end-point)  
  if#switchport mode access  
  if#switchport access vlan 10  
  if#exit  

- **To a switch (Layer 1):**  
  fig#int f#/# (port to another switch/router)  
  if#switchport mode trunk  
  if#switchport trunk encapsulation dot1q  
  if#switchport trunk allowed vlan 10,20  
  if#exit  

Configuring a Layer 3 Interface on a Multilayer Switch:

\>en  
\#conf t  
fig#int vlan 10  
if#ip address (ip address) (subnet mask)  
if#no shutdown  
if#exit  
#copy run start  
#reload  

Troubleshooting Commands:

\#show vlan brief  
\#show interfaces trunk  
\#show running-config | section vlan  

