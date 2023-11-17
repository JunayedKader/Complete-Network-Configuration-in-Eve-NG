# Complete-Network-Configuration-in-Eve-NG
Unlock the full potential of my network infrastructure with this comprehensive Eve NG project. Experience a seamless blend of VLANs, DTP, VTP, Etherchannel, OSPF, NAT, VPN, and STP configurations, meticulously crafted for optimal performance and security.

1. VPCs and IP Addresses:

  VPC1: 10.1.1.1
  VPC2: 10.1.1.2
  VPC3: 20.1.1.1
  VPC4: 20.1.1.2
  VPC5: 30.1.1.1
  VPC6: 30.1.1.1

2. Access Switch VLAN Configuration:

  Access Switch 1: VLAN 10
  Access Switch 2: VLAN 20
  Access Switch 3: VLAN 30
  Access Switch 4: VLAN 40

3. SVI (Switched Virtual Interface) IPs in SW1:

  VLAN 10: 10.1.1.254
  VLAN 20: 20.1.1.254
  VLAN 30: 30.1.1.254
  VLAN 40: 40.1.1.254

4. HSRP (Hot Standby Router Protocol) Configuration:

  VLAN 10: Virtual IP 10.1.1.100
  VLAN 20: Virtual IP 20.1.1.100
  VLAN 30: Virtual IP 30.1.1.100
  VLAN 40: Virtual IP 40.1.1.100

5. Trunking Configuration on SW1:

  Via Gi0/1-4 interfaces with Access Switches 1-4 (Gi0/0)

Trunking Configuration on SW2:

  Via Gi0/1-4 interfaces with Access Switches 1-4 (Gi0/1)

6. Additional Configurations:

  Dynamic Trunking Protocol (DTP) configured between switches.
  VLAN Trunking Protocol (VTP) with the domain server name "ccna" for sharing VLAN information.

7. Multilayer Switch Interconnection (SW1 and SW2):

  Interfaces: Gi1/1, Gi1/2, Gi1/3, Gi2/0
  Configured as an EthernetChannel.

8. IP Configuration for Interfaces:

  SW1 Gi0/0: 12.1.1.1
  Router R1 Gi0/1: 12.1.1.2
  SW2 Gi0/0: 13.1.1.1
  Router R1  Gi0/2: 13.1.1.2


Routers R1 and R2 are equipped with the OSPF routing protocol to facilitate the exchange of routing information. Additionally, I have implemented Port Address Translation (PAT) on both R1 and R2 to enable communication with diverse networks.

Mirroring this setup, the right side of the network has been meticulously configured to maintain symmetry and coherence.

Furthermore, a Virtual Private Network (VPN) tunnel has been established between R1 and R2, bolstering the network's security by ensuring confidential and secure access.


Topology:

![image](https://github.com/JunayedKader/Complete-Network-Configuration-in-Eve-NG/assets/57216984/ad89121f-99e7-4470-8021-4f5503e29b9e)
