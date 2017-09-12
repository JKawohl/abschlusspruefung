# Übungen zu Subnetting

1. Wie lauten die Netzwerk und Broadcastadresse für folgende IPs?

153.123.221.235/22

10.0.129.224/20

172.20.240.0/20

10.12.14.16/28

2. 

In einer Schule soll das Netz 200.100.50.0 mittels Subnetting so aufgeteilt werden, dass jeder Klassenraum
ein eigenes Subnet bekommt.
Wieviel Adressen stehen im Netz 200.100.50.0 ohne Subnetting frei zur Verfügung?

Wieviele Klassenräume können ein eigenes Netz bekommen, wenn in einem Raum 12 Schüler und ein
Lehrer PC sowie ein Drucker installiert sind?

Wie lauten die Net-IP, Netmask und Broadcast-IP der Subnetze? (Tabelle)

Es reichen die ersten 4


Netz    Netzadresse   Netztmaske        Broadcastadresse
0       200.100.50.0  255.255.255.240   200.100.50.15
1
2
3



Nachträglich sollen die Rechner mit dem Internet verbunden werden.
Welches Problem tritt auf?





Wie kann dieses Problem gelöst werden?








3. 

Fünf Labore der Informatik sollen sich das Class C Netz 141.69.203.0 so aufteilen, dass jedes Labor ein
eigenes Netz bildet. In einem Labor befinden sich maximal 22 Rechner, dazu ein Drucker. Der Router soll
die kleinste frei verfügbare Host ID bekommen.
Welche Netzmaske ist erforderlich?





Wie lauten die Net-IP, Broadcast-IP und Gateway Adressen jedes Teilnetzes? (Tabelle)

Es reichen die ersten 4

Netz   Netzadresse    Broadcastadresse    Gateway Adresse
0     141.69.203.0    141.69.203.31       141.69.203.1
1
2
3
4



4.

Sie sind Deutschland-Admin einer gröÿeren Firma mit Niederlassungen in Berlin, Düsseldorf, Hannover,
München, Stuttgart. In jeder Niederlassung gibt es die Abteilungen Einkauf (E), Forschung (F), Lager (L),
Produktion (P), und Verkauf (V). Jede Abteilung bekommt ein eigenes Netz. Die maximale Abteilungs-
gröÿe beträgt 50 Hosts. Jede Filiale ist über WAN mit der Deutschlandzentrale verbunden. Es wird eine
einheitliche Netzmaske in allen Netzen verwendet.

Wie lautet die Netzmaske?


Wieviel Netze brauchen Sie?


Wieviel IP-Adressen brauchen Sie?


Welche privaten IP-Netze könnte die Firma füer das Subnetting verwenden?
