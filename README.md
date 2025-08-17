Packet Tracer Simulation

"Secure Hospital Network with VLANs and Port Security"
  
  Objective: To create a simulation of a secure network architecture for a hospital in Cisco Packet Tracer. 
            Setting up key HIPAA technical safeguards was the goal and using VLANs to isolate patient data from
            the public guest network shows this. Design includes:
              * Router-based DHCP server for automation
              * Port Security to harden physical access points
              * Controller-based wireless network for managed guest access
  
  Network Topology:
<img width="693" height="384" alt="Packet tracer hospital network" src="https://github.com/user-attachments/assets/0eaa8197-bae6-4880-b6bc-665ca5357773" />

  Features Implemented:
    * VLAN Segmentation (VLAN 10 and 20) for HIPAA compliance
    * Router-on-a-Stick (ROaS) for Inter-VLAN routing
    * DHCP Server on Router for automated IP management
    * Port Security with Sticky MACs to prevent unauthorized device access
    * Controller-based Wireless (WLC and LAP) for managed guest network

  Key Configuration Example:
    interface FastEthernet0/11
      description Connection to Staff Workstation
      switchport mode access
      switchport access vlan 20
      switchport port-security
      swithcport port-security mac-address stick

  How to Use: Download the .pkt file, then open it with Cisco Packet Tracer.
