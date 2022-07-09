# DNS-CONFIGURATION
-------------------
R1
---
int g0/0
Rip address 192.168.1.1 255.255.255.0
no shutdown 
ip dhcp pool internal
default-router 192.168.1.1
network 192.168.1.0 255.255.255.0
dns-server 192.168.1.10
end

DHCP Excluded-address
----------------------
R1
----
ip dhcp excluded-address 192.168.1.1 192.168.1.10
end
![DNS Lab](https://user-images.githubusercontent.com/106605770/178120685-ce4cb0f7-f19a-48bd-8867-42276dcae42c.PNG)
