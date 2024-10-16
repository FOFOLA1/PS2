# Commands for Router and Switch

## User exec mode (Switch>)
* ``enable`` - [Privileged exec mode](#Privileged-exec-mode-``Switch#``)
* ``show version`` - Display software version and system information
* ``exit`` - Exit to previous mode
* ``help`` - Display available commands

## Privileged exec mode ``Switch#``
* ``configure terminal`` -  [Global Configuration mode](#Global-configuration-mode-``Switch(config)``)
* ``show running-config``: Display current configuration
* ``show ip interface brief``: Display brief interface status
* ``reload``: Reload the router
* ``exit``: Exit to User Exec mode
* ``show ip route``: Display routing table
* ``show interfaces``: Display interface status and configuration
* ``show version``: Display software version and system information
* ``enable password password``: Set enable password
* ``enable secret password``: Set enable secret password


## Global Configuration mode ``Switch(config)``
* ``hostname <name>`` - Set hostname
* ``interface [type number]`` - Enter [Interface Configuration mode](#Interface-Configuration-Mode-``Switch(config-if)#``)
* ``ip address [address] [subnet mask]`` - Set IP address on interface
* ``no shutdown`` - Enable interface
* ``line vty 0 4`` - Enter [Line Configuration mode](#Line-Configuration-Mode-``Switch(config-line)#``)
* ``password <password>`` - Set password for VTY lines
* ``exit`` - Exit to Global Configuration mode

# Interface Configuration Mode ``Switch(config-if)#``
* ``ip address [address] [subnet mask]`` - Set IP address on interface
* ``no shutdown`` - Enable interface
* ``exit`` - Exit to Global Configuration mode

# Line Configuration Mode ``Switch(config-line)#``
* ``password <password>`` - Set password for VTY lines
* ``exit`` - Exit to Global Configuration mode
