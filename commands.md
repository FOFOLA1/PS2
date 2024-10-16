# User exec mode (Switch>)
* enable - [Privileged exec mode](#Privileged exec mode)
* show version - Display software version and system information
* exit - Exit to previous mode
* help - Display available commands

# Privileged exec mode ``(Switch#)``
* configure <terminal/line>
* configure terminal: Enter Global Configuration mode
* show running-config: Display current configuration
* show ip interface brief: Display brief interface status
* reload: Reload the router
* exit: Exit to User Exec mode
* show ip route: Display routing table
* show interfaces: Display interface status and configuration
* show version: Display software version and system information
* enable password password: Set enable password
* enable secret password: Set enable secret password


# Global Configuration mode (Switch(config))
* hostname name: Set hostname
* interface [type number]: Enter Interface Configuration mode
* ip address [address] [subnet mask]: Set IP address on interface
* no shutdown: Enable interface
* exit: Exit to Global Configuration mode
* line vty 0 4: Enter Line Configuration mode
* login local: Enable local login
* password password: Set password for VTY lines
* exit: Exit to Global Configuration mode
* router ospf [process-id]: Enter OSPF configuration mode
* exit: Exit to Global Configuration mode

# Interface Configuration Mode (Router(config-if)#)
* ip address [address] [subnet mask]: Set IP address on interface
* no shutdown: Enable interface
* exit: Exit to Global Configuration mode

# Line Configuration Mode (Router(config-line)#)
* login local: Enable local login
* password password: Set password for VTY lines
* exit: Exit to Global Configuration mode
