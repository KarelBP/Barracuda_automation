# Barracuda automation
Prototype of automation for Barracuda CloudGen Firewalls via Control Center, driven from ServiceNow. The XML files are update sets. Developed using CGF & CC 10.5, but it's quite possible it works with older versions too.

## Files

### Catalog Items
Barracuda rename IP networks.xml => Identify networks in IP networks (cmdb_ci_ip_network) and populate their names from Global Firewall Objects in Barracuda CC.

Barracuda rename networks in discovery ranges.xml => Identify networks in discovery ranges (discovery_range) and populate their names from Global Firewall Objects in Barracuda CC.

### Flows
Barracuda get named IPv4 networks.xml => Get names of IPv4 networks from Global Firewall Objects/Policies in Barracuda CC

Barracuda look up network name.xml => Look up names of networks from the cmdb_ci_ip_network table which don't have their names set

Barracuda rename discovered IP networks.xml => Flow to trigger renaming of records in IP networks table (cmdb_ci_ip_network).

Barracuda rename network ranges.xml => Flow to trigger renaming of records in Discovery Range Sets table (discovery_range).

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
