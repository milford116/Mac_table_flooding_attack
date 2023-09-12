# Mac_table_flooding_attack
Mac Table Flooding :
In computer networking, a media access control attack or MAC flooding is a technique employed to compromise the security of network switches. The attack works by forcing legitimate MAC table contents out of the switch and forcing a unicast flooding behavior potentially sending sensitive information to portions of the network where it is not normally intended to go.

Attack Strategy:
Switches maintain a MAC table that maps individual MAC addresses on the network to the physical ports on the switch. This allows the switch to direct data out of the physical port where the recipient is located, as opposed to indiscriminately broadcasting the data out of all ports as an Ethernet hub does. The advantage of this method is that data is bridged exclusively to the network segment containing the computer that the data is specifically destined for.
In a typical MAC flooding attack, a switch is fed many Ethernet frames, each containing different source MAC addresses, by the attacker. The intention is to consume the limited memory set aside in the switch to store the MAC address table.
The effect of this attack may vary across implementations, however the desired effect (by the attacker) is to force legitimate MAC addresses out of the MAC address table, causing significant quantities of incoming frames to be flooded out on all ports. It is from this flooding behavior that the MAC flooding attack gets its name.
After launching a successful MAC flooding attack, a malicious user can use a packet analyzer to capture sensitive data being transmitted between other computers, which would not be accessible were the switch operating normally. The attacker may also follow up with an ARP spoofing attack 
which will allow them to retain access to privileged data after switches recover from the initial MAC flooding attack.
