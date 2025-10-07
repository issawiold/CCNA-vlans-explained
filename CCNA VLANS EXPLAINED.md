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
-To an end point-
if#sw mod access
if#sw acc vlan 10
-To a switch layer1-
if#sw mod trunk
-If only one vlan below the switch-
if#sw trunk native vlan 10
-If more than one vlan below the switch -
if#sw trunk allow vlan 10,20
-For multilayer switch-
>en
#conf t
fig#int vlan 10
if#ip add (ip address) (subnet mask)
-to end opertion-
if#end
#copy run star
#reload

