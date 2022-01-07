# Using others workstation

## Docker relationship map

![workstation](./MacOS_vs_workstation.png)

## Code for going to workstation
Description: 
IP address for Workstation: 172.19.240.104
IP address for DGX: 172.19.240.34
```bash
ssh [user_name]@[IP address]
```

## Code for port mapping of MacOS & workstation
Description: type in local host number for the container
```bash
ssh [user_name]@[IP address] -L localhost:100XX:localhost:100XX -L localhost:100xx:localhost:100xx
```

```{note}
You should see 
![connected_workstation](./connected_workstation.png) 
```