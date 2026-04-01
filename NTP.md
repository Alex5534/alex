R1(config)# ntp server 192.168.1.5 
R2
R3

R1(config)# ntp server 192.168.1.5 
R2
R3


R1(config)# ntp authenticate 

R1(config)# ntp trusted-key 1 

R1(config)# ntp authentication-key 1 md5 NTPpa55 

R1(config)# service timestamps log datetime msec 
R2
R3
