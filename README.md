# Barracuda automation
Automation building blocks for Barracuda Control Center, driven from ServiceNow. The XML files are update sets.

## Files

### Catalog Items
Barracuda rename IP networks.xml => (description)

Barracuda rename networks in discovery ranges.xml => (description)

### Flows
Barracuda get named IPv4 networks.xml => Get names of IPv4 networks from Global Firewall Objects/Policies in Barracuda CC

Barracuda look up network name.xml => Look up names of networks from the cmdb_ci_ip_network table which don't have their names set

### Actions
Barracuda create singleIPv4Address.xml => Create a singleIPv4Address object in Global Firewall Objects/Policies in Barracuda CC

Barracuda create singleIPv4Network.xml => Create a singleIPv4Network object in Global Firewall Objects/Policies in Barracuda CC

Barracuda create listIPv4Address.xml => Create a listIPv4Address object in Global Firewall Objects/Policies in Barracuda CC. An initial member (reference to an existing object) must be provided

Barracuda create listIPv4Network.xml => Create a listIPv4Network object in Global Firewall Objects/Policies in Barracuda CC. An initial member (reference to an existing object) must be provided

Barracuda delete object.xml => Delete an object from Global Firewall Objects/Policies in Barracuda CC

Barracuda add object to group.xml => Add an object reference into a group in Global Firewall Objects/Policies in Barracuda CC

Barracuda remove object from group.xml => Remove an object reference from a group in Global Firewall Objects/Policies in Barracuda CC

Barracuda create access rule.xml => Create a simple access rule (pass) via Barracuda CC

Barracuda delete access rule.xml => Delete an access rule via Barracuda CC
