# Commands for Router and Switch

## User exec mode (Switch>)
* ``enable`` - přejde do [Privileged exec mode](#privileged-exec-mode-switch)
* ``show version`` - Zobrazí verzi
* ``exit`` - Vrátí zpět do předchozího modu
* ``help`` - Zobrazí možné commandy

## Privileged exec mode ``Switch#``
* ``configure terminal`` -  přejde na [Global Configuration mode](#global-configuration-mode-switchconfig)
* ``show running-config``: Zobrazí aktuální config (není uložen v paměti, po restartu se smaže)
* ``line console [number]``: přejde do [Line Configuration mode](#line-configuration-mode-switchconfig-line) k nastavení připojení pomcí console portu (VTY)
* ``show ip interface brief``: Zobrazí jednoduchý status ip rozhraní
* ``reload``: Restart
* ``exit``: Vrátí do [user exec mode](#user-exec-mode-switch)
* ``show ip route``: Zobrazí routovací tabulku
* ``show interfaces``: Zobrazí status a config rozhraní
* ``show version``: Zobrazí verzi
* ``enable password [password]``: Helo pro vstup do exec modu (většinou "cisco")
* ``enable secret [password]``: Nastavení hesla pro vstup do tohoto modu (většinou je "class")


## Global Configuration mode ``Switch(config)``
* ``hostname <name>`` - Set hostname
* ``interface [type number]`` - Enter [Interface Configuration mode](#interface-configuration-mode-switchconfig-if)
* ``ip address [address] [subnet mask]`` - Set IP address on interface
* ``no shutdown`` - Enable interface
* ``line vty 0 4`` - Enter 
* ``password <password>`` - Set password for VTY lines
* ``exit`` - Exit to Global Configuration mode

# Interface Configuration Mode ``Switch(config-if)#``
* ``ip address [address] [subnet mask]`` - Set IP address on interface
* ``no shutdown`` - Enable interface
* ``exit`` - Exit to Global Configuration mode


# Line Configuration Mode ``Switch(config-line)#``
* ``password <password>`` - Set password for VTY lines
* ``exit`` - Exit to Global Configuration mode
