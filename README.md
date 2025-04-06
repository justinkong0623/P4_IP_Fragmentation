# P4_IP_Fragmentation
**Setup on Window Computer**  

1.Create a new project in Programmer Studio.  

![image](https://github.com/user-attachments/assets/e18c0ad8-f06e-4eed-975b-cedd32c9895b)

2.Add IP_Fragmentation.p4, configuration.p4cfg, and sleep.c to the project.  

3.Change the debug mode from Simulation to Hardware.  

![image](https://github.com/user-attachments/assets/96f87a17-64b8-4a73-b8ed-b129cfb0c994)


4.Set the IP address for the SmartNIC.  

![image](https://github.com/user-attachments/assets/6a2af2e4-a551-43d0-9191-e6bb8fef5419)  

5.Modify the build settings as shown below.  

![image](https://github.com/user-attachments/assets/6ea68c9c-a7e3-4a78-bfcf-6bef058837f2)

6.Rebuild the project (Alt + F7).

**Setup on Linux Computer 1 (with SmartNIC)**  

sudo systemctl start nfp-sdk6-rte  

sudo systemctl start nfp-hwdbg-srv  

sudo make setup  


**Setup on Linux Computer 2 (without SmartNIC)**  

sudo make setup


**Setup on Window Computer**  

Start Debugging (F12)  

