# Commands for Router and Switch

## User exec mode ``Switch>``
* ``enable`` - přejde do [Privileged exec mode](#privileged-exec-mode-switch)
* ``show version`` - Zobrazí verzi
* ``exit`` - Vrátí zpět do předchozího modu
* ``help`` - Zobrazí možné commandy

## Privileged exec mode ``Switch#``
* ``configure terminal`` -  přejde na [Global Configuration mode](#global-configuration-mode-switchconfig)
* ``show running-config``: Zobrazí aktuální config (není uložen v paměti, po restartu se smaže)
* ``show startup-config``: Zobrazí config, který se použije po zapnutí routeru
* ``copy running-config startup-config``: Nakopíruje běžící config do paměti routeru (tj. použije se po zapnurí switche/routeru)
* ``copy startup-config running-config``: Proběhne merge obou configů, nikoli kopie (lepší použít ``reload`` pokud to není nutné)
* ``line console [number]``: přejde do [Line Configuration mode](#line-configuration-mode-switchconfig-line) k nastavení připojení pomcí console portu (popřípadě VTY)
* ``show ip interface brief``: Zobrazí jednoduchý status ip rozhraní
* ``reload``: Restart
* ``exit``: Vrátí do [user exec mode](#user-exec-mode-switch)
* ``show ip route``: Zobrazí routovací tabulku
* ``show interfaces``: Zobrazí status a config rozhraní
* ``show version``: Zobrazí verzi
* ``enable password [password]``: Helo pro vstup do exec modu (většinou "cisco")
* ``enable secret [password]``: Nastavení hesla pro vstup do tohoto modu (většinou je "class")


## Global Configuration mode ``Switch(config)``
* ``hostname <name>`` - Nastaví hostname (Tedy to, co vidím na začátku každýho řádku, default je Switch nebo Router)
* ``banner motd "text"``: Nastavení úvodní zprávy při vstupu do global configu
* ``interface [number]`` - Vstup do [Interface Configuration mode](#interface-configuration-mode-switchconfig-if) k nastavení například jednotlivých portů (první je označen 0)
* ``ip address [address] [subnet mask]`` - Nastaví IP a masku
* ``service password-encryprion``: nastaví kódování hesla, aby nebyly lehce čitelné v configu (stále se dají lehce encryptovat)
* ``no shutdown`` - Zapne rozhraní
* ``line vty 0 4`` - Vstup do [Line Configuration mode](#line-configuration-mode-switchconfig-line)
* ``password <password>`` - Nastavení hesla pro VTY linky
* ``exit`` - Vrácení do global config mode

# Interface Configuration Mode ``Switch(config-if)#``
* ``ip address [address] [subnet mask]`` - Přidělí IP adresu danému rozhraní
* ``no shutdown`` - Zapne rozhraní
* ``exit`` - Navrácení do global config modu


# Line Configuration Mode ``Switch(config-line)#``
* ``password <password>`` - Nastavení hesla pro linku
* ``exit`` - Navrácení do glogal configu
