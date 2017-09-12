# Prüfung 2

### 1. Subnetze

#### a) 3 Vorteile bei Subnetzen

1. Sicherheit durch Abgrenzung zb zw 2 Routern, ein Netzt mit nur 2 Adressen
2. Erhöhung der Performance - Kleines Netz - Besserer Broadcast
3. IP Einsparung  - Man nutzt nicht gesamten Bereich, sondern Teile
4. Übersichtlicher zb 1 Abteilung = 1 Subnetz
-----

### b) Unterschied zw Private Adressen u. Öffentliche Adressen

private werden vom router vergeben, sind nur im eigenem netz gültig, nicht nach außen routbar

öffentliche werden vom ISP vergeben, benötigt für internetkommunitkation

Private IP Bereiche:

192.168.x.x  bis 192.168.255

172.16.x.x bis 172.31.255

10.x.x.x bis 10.255

------

#### c) Planung vom Netz

Lösung

4 Subnetze a 62 möglichen Host, weil /24 kann man mit 4 sub, in 62 verteilen. siehe bild.
Netz: 192.168.33.0 / 24

Meine Rechnung


Produktion 50 ip + router = 51 = 64 näheste 2er Potenz = 2 hoch 6

Netzmaske 255.255.255.256-64=192 oder /32 - 6 = 26

Vertrieb 40 +1 = 41 wie Produktion weil nächste potenz ist 64

Leitung 5 PC + Router = 6 IPs, 8 ist die nächste potenz von 2 = 2 hoch 3

Netzmaske 255.255.255.256-8 = 248 oder /32 - 3 = 29

Core 4  PC , wie Leitung

--------

### d) 

arp = Address Resolution Protocol

Zum versenden von Packeten wird IP + MAC benötigt.

------
## 2. VOIP und VLAN

### a) Prinzip von VOIP

Sprache wird in digitale Signale, in Packete zerteilt, und via Internet verschickt, und am Zielsystem wieder zusammengesetzt und umgewandelt. VOIP server nötig

Server = verbindet auch bei dyn IP die Sender + Empfänger. Protokoll = RDP auf UDP aufsetzt.

Zb Skype / Hangouts / Lync

-----

### b) 

Vermittlung VOIP Gateway

Software Softphone

Gerät Analog-Telefon-Adapter

Telefon Voip Telefon

Telefonanlage IP PBX

-----

### c ) 

VOIP braucht nur die Packete zu senden - Einseitige kommunikation - einsparung vom Netzwerkverkehr + Geschwindigkeitsgewinn

Quality of Service = TCP - schlechte Qualität. Weil bei fehlern nochmal nachgefragt wird. Sprache - echtzeitanwendung.

UDP sendet nur, TCP sendet und empfängt. 


------ 

### d) VLANs

Richtige Aussagen

Lösung - IEEE 802.1Q

Broadcastdomäne

portweise Zuordnung im Switch konfiguriebar

Dynamische Zuordnung anhand von Macadressen

VLAN meherer Switches - Tags


------


#### e) Vlan berechnung

12 bits = 2 hoch 12 - 4096 Möglichkeiten 0 - 4095

Meist sind 0 und 9095 reserviert - dann nur 4094 möglichkeiten 


## 3 Firewall - 

### a) 

Schutz von Computern vor unerwünschten Zugriffen von Außen. Filterung von Eingangsverkehr mit Regeln


----------

### b) 

20 -> FTP , 21 > FTP kontrolle,  25 > SMTP 




---------

### c)

bestehende Verbindung - Stateful

Nutzdaten durchleichten - Application

nur IP - Packet

Proxy Firewall - Application

Einfachster - Packet



erklärung - Packet Filter

Paketfilter (auch Portfilter) stellen die einfachste Variante einer Firewall dar. Hierbei wird immer der Header der einzelnen Protokolle (IP-Header, ICMP-Header, TCP-Header, UDP-Header) überprüft und in Abhängigkeit der eingestellten Filter-Regeln verarbeitet

Application Layer

Das Application Level Firewall wird in den Datenstrom zwischen Client und Server geschaltet und "spielt" in Richtung Client den Server und stellt gegenüber dem Server den Client da. Für jeden TCP-Dienst wird daher ein eigenes Programm (der sog. Proxy) benötigt!


Stateful


 in der Lage, sich die aktuellen Status- und Kontextinformationen zu merken bzw. diese bei der Filterung zu berücksichtigen.



-------------

### d)

DMZ = Demiliterized Zone. Bereich zwischen 2 Firewalls. zb Webserver in der DMZ aber Firmennetz hinter 2ten Firewall.

Bereich zwischen dem Benutzernetz und dem Internet. Wird oft verwendet um Angriffe vor ab abzufangen. 



------------

### e)

workstation switch firewall email firewall router internet

------------------------

## 4 DHCP

### a) 

DHCP

Dynamic Host Configuration Protocol

Automatische Vergabe von IP adressen an Rechner im Netz, und anderen Informationen - wie ZB Router, DNS Server, Mail Server, Nameserver usw.

IP Adress Konflinkte werden vermieden

Endgeräte automatisch konfiguriert




-----

### b)


Richtige Aussagen

Default Gateway
Subnetzmaske
DNS
öff IP des WAN zugangsrouters
Gültigeisdauer



--------------

### c)
Discover cl to server
Offer server to client
Request cl to server
ACK server to client



------------------

### d) 

IP Adressen Reservierung

oder RADIUS Server

------------------

### e ) 


DHCP Relay Agent nicht eingerichted. DHCP Anfragen sind nicht rootbar, da über broadcast.




------------------
## 5. Datensicherung und Cloud

### a) 

Datensicherung über :

- Medien > optisch, magnetisch, elektonisch, cloud
- RAID > raid 0, raid 1, raid 5, raid 6, mischformen
- Backup > voll , diff, inkr
- Lagerort > im pc, safe, anderer ort
- Empfehlungen > mind 2 versch medien, min 2 lagerorte, regelmäßige backups, mischung zw voll und diff, einsatz von raid




---------------
### b) 

Raid0 - kleinster gemeinsamer nenner

entweder 4*750 = 3000

oder 5 * 500 = 2500

Raid1 - KGN durch 2 ( NUR GLEICHE FESTPLATTEN)

dh 4*750 = 3000 / 2 = 1500

Raid5 - KGN && -1 dh 5-1 *500
 
 oder 4-1 * 500

Raid10 - kombi aus 1 und 0, mind 4 platten und KGN

4*750 / 2


--------------------

### c) 

Infrastructure as a Service = Hardware zur miete für Dienste, zb amazon s3

Platform as a Service = Nutzung von Platform zur nutzung und entwicklung

Software as a Service = OFFICE 365 in der cloud


--------------

### d)

3 vorteile von cloud computing

Zugriff von überall

Skalierbar

Keine physischen Maschienen nötig

Platz und Strom, kosten ( lizensen ) ersparnis

Zentrales Backup

3 nachteile von cloud computing

daten nicht in eigener hand > Datenschutz

Abhängigkeit von Cloud anbietern

diebstah gefahr, hacker gefahr

benötigt internetzugang

