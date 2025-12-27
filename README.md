# pfsense
LAB 1 – Networking & Interface Configuration

-Q1 : Identified the interfaces

         Go to interfaces and assignments and then identified all physical and virtual interfaces visible to pfSense.

Q2 : Configure one interface as LAN

         Assigned one interface as LAN , and set IP configuration , I have given ip address  as 192.168.1.1 and subnet as /24,Enable the LAN interface.

Q3 : Renamed Interfaces

        I changed the interfaces names into meaningful name like LAN-Core,WAN-Uplink, Lab-Network

Q4: Reboot Verification

        Q4 requirement is to reboot the pfsense ,i did this by navigated towards diagnostics and then reboot, it has taken 80 seconds to rebbot                

LAB 2 - Firewall Rule Logic & Policy Enforcement

Q1 : Allow traffic for one specific internal host

        Navigated to firewall -> rules ->  LAN , we have to create a pass rule for that, configuration is  Action : pass, Source : 192.168.1.10 Destination : Any ,
        This ensures only one internal host is allowed to access this network.

Q2 : Block all ICMP Traffic from LAN

   -> Created a block rule above all rules
   
   -> Configuration is Protocol : ICMP , Source : LAN net, Destination : Any
   
   -> The main result  is All ping (ICMP) requests from LAN are blocked

Q3 : Create Time-Based Rule(Working hours)

   -> First thing is to create a schedule
   
