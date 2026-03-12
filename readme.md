1. From stock firmware: LAN is port 4, WAN is port 3. There are 18 interfaces in stock firmware. I have no idea why they need so many

2. Stock bootlog also says that eth1 is WAN. But eth1 is always UP even if the cable isn't plugged in.

3. Why is port 5 turned on? Is it really necessary?

4. For MT7621 devices there are 4 cases apparently:
4.1. both lan and wan are defined inside switch0, wan has phy-handle.
4.2. wan is defined in gmac1 and lan is defined in switch0, wan has phy-handle.
4.3. lan is defined in gmac1 and wan is defined in switch0, lan has phy-handle.
4.4. both lan and wan are defined inside switch0, neither of them have phy-handle.

I need help determining correct .dts from stock .dts.
