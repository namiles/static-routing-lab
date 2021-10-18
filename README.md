# Configuring Static Routes
You can find the full device configurations for my Static Routing lab below.. This lab and more are available at https://www.nicksnetworklab.com.   

### R1
```
ip route 10.1.1.0 255.255.255.0 172.16.1.2 
ip route 2.2.2.2 255.255.255.255 172.16.1.2 
ip route 3.3.3.3 255.255.255.255 172.16.1.2 
[optional] ip route 0.0.0.0 0.0.0.0 172.16.1.2
```
### R2
```
ip route 1.1.1.1 255.255.255.255 172.16.1.1 
ip route 3.3.3.3 255.255.255.255 10.1.1.2 
```
### R3
```
ip route 1.1.1.1 255.255.255.255 10.1.1.1 
ip route 172.16.1.0 255.255.255.0 10.1.1.1 
ip route 2.2.2.2 255.255.255.255 10.1.1.1 
```
