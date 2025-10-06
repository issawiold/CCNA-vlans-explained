# vlans-explained
vlans explained
>en
#conf t
fig#vlan 10 (any number you want 1-1001)
vlan#exit
fig#vlan 20
vlan#name (name it what you want)
vlan#exit
fig#int f#/#
To an end point
if#sw mod access
if#sw acc vlan 10
To a switch or router
if#sw mod trunk
If only one vlan below the switch router
if#sw trunk native vlan 10
If more than one vlan below the switch router
if#sw trunk allow vlan 10,20
if#end
#copy run star
#reload

