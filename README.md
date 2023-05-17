# guru-SOHO

This is my interpretation based on the Small-Office Home-Office design described below. 

https://gurutechnetworks.otombenard.com/assetsProject/project2

Project #2 Case Study and Requirements
XYZ company is a fast-growing company in Eastern Australia with more than 2 million customers globally. The company deals with selling and buying of food items, which are basically operated from the headquarters. The company is intending to open a branch near the local village Bonalbo. Thus, the company requires young IT graduates to design the network for the branch. The network is intended to operate separately from the HQ network. Being a small network, the company has the following requirements during implementation;
One router and one switch to be used (all CISCO products).
3 departments (Admin/IT, Finance/HR and Customer service/Reception).
Each department is required to be in different VIANS.
Each department is required to have a wireless network for the users.
Host devices in the network are required to obtain IPv4 address automatically.
Devices in all the departments are required to communicate with each other.
Assume the ISP gave out a base network of 192.168.1.0, you as the young network engineer who has been hired, design and implement a network considering the above requirements.

---------------------------------------------------

In this design, I used the follow combinations of DHCP pools, VLANs and subnets for the corresponding departments.

IT/Admin                  | VLAN 10 | 192.168.1.0/26    |
Finance/HR                | VLAN 20 | 192.168.1.64/26   |
CustomerService/Reception | VLAN 30 | 192.168.1.128/26  |
