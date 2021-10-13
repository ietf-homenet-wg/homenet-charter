# Charter for Working Group

This working group focuses on the evolving networking technology within and among relatively small "residential home" networks.
For example, an obvious trend in home networking is the proliferation of networking technology in an increasingly broad range and number of devices.
This evolution in scale and diversity sets some requirements on IETF protocols.
Some of the relevant trends include:

* Multiple segments: While less complex L3-toplogies involving as few subnets as possible are preferred in home networks for a variety of reasons including simpler management and service discovery, the introduction of more than one subnet into a home network is enough to add complexity that needs to be addressed, and multiple dedicated segments are necessary for some cases.
For instance, a common feature in modern home routers in the ability to support both guest and private network segments.
Also, link layer networking technology is poised to become more heterogeneous, as networks begin to employ both traditional Ethernet technology and link layers designed for low-powered sensor networks.
Finally, similar needs for segmentation may occur in other cases, such as separating building control or corporate extensions from the Internet access network for the home.
Different segments may be associated with subnets that have different routing and security policies.

* Service providers are deploying IPv6, and support for IPv6 is increasingly available in home gateway devices.
While IPv6 resembles IPv4 in many ways, it changes address allocation principles and allows direct IP addressability and routing to devices in the home from the Internet.
This is a promising area in IPv6 that has proved challenging in IPv4 with the proliferation of NAT.

* End-to-end communication is both an opportunity and a concern as it enables new applications but also exposes nodes in the internal networks to receipt of unwanted traffic from the Internet.
Firewalls that restrict incoming connections may be used to prevent exposure, however, this reduces the efficacy of end-to-end connectivity that IPv6 has the potential to restore.

Home networks need to provide the tools to handle these situations in a manner accessible to all users of home networks.
Manual configuration is rarely, if at all, possible, as the necessary skills and in some cases even suitable management interfaces are missing.

The purpose of this working group is to focus on this evolution, in particular as it addresses the introduction of IPv6, by developing an architecture addressing this full scope of requirements:

* prefix configuration for routers

* managing routing

* name resolution

* service discovery

It is expected that the working group will define a set of protocol specifications to accomplish the four requirements from above.
However, it is not in the scope of the working group to define entirely new routing protocols or address allocation protocols.
As noted, additional options or other small extensions may be necessary to use the existing protocols in these new configuration tasks.
The working group shall also not make any changes to IPv6 protocols or addressing architecture.
Prefix configuration, routing, and security related work shall not cause any changes that are not backwards compatible to existing IPv6 hosts.
There may be host visible changes in the work on naming and discovery protocols, however.
In its design, the working group shall also consider security aspects and the impact on manageability.
The main focus of the working group is home networks, but the group's results may also find applications in other small networks.
The group should assume that an IPv4 network may have to co-exist alongside the IPv6 network and should take this into account insofar as alignment with IPv6 is desirable.
But the group should also ensure that even IPv6-only are possible, and while IP-version agnostic work is of course desirable, IPv4-specific work is outside the scope of the group.

The working group will liaise with the relevant IETF working groups.
In particular, the group should work closely with the V6OPS working group, review any use or extension of DHCP with the DHC working group, and work with additional DNS requirements with the DNSEXT and DNSOP working groups.
If it turns out that additional options are needed for a routing protocol, they will be developed in the appropriate Routing Area working group, with the HOMENET working group providing the architecture and requirements for such enhancements.
The working group will also liason with external standards bodies where it is expected that there are normative dependencies between the specifications of the two bodies.
It is expected that in the architecture definition stage liaising with the Broadband Forum, DLNA, UPnP Forum, OASIS, ZigBee Alliance and other SDOs is necessary, as is understanding existing technology from these groups.
