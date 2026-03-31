R1(config)# router ospf 1 
area 0 authentication message-digest
 
router ospf 2 
R2(config-router)# area 0 authentication message-digest 

 router ospf 3
area 0 authentication message-digest 

R1(config)# interface s0/0/0 
R1(config-if)# ip ospf message-digest-key 1 md5 MD5pa55

R2(config)# interface s0/0/0 
R2(config-if)# ip ospf message-digest-key 1 md5 MD5pa55
R2(config-if)# interface s0/0/1 
R2(config-if)# ip ospf message-digest-key 1 md5 MD5pa55 

R3(config)# interface s0/0/1 
R3(config-if)# ip ospf message-digest-key 1 md5 MD5pa55 

ex
ex
show ip ospf interface
