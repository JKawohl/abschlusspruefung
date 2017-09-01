Tips

Netzwerkadresse = erste IP adresse in den Subnetz

zb 10.0.0.0 255.255.255.0 

Netzwerkadresse wäre hier die 10.0.0.0, 

die erste verfügbare IP die 10.0.0.1,

die letze IP 10.0.0.254,

und die Broadcastadresse die 10.0.0.255



Die Netzwerkadresse und die Broadcastadresse können nicht von einem Host belegt werden!

Wenn man sich im letzten Oktett befindet 255.255.255.0 dann ist es einfach die IP adresse und

Subnetmaske rauszufinden, denn diese sind meist identisch, bzw die Differenz von 256.

Wenn man zum Beispiel 120 Adressen braucht, ist der Nächste Subnetzbereich 128, und 256 - 128 ist 128.

Daher ist die Netzadresse in diesem Fall 10.0.0.128 und die Broadcastadresse die 10.0.0.255.

Die Subnetzmaske wäre 255.255.255.128

Subnetze werden immer in Potenzen von 2 gebildet. Es hilft bei einer Subnetz Aufgabe sind die Potenzen aufzuschreiben.

Die Subnetze    2 4 8 16 32 64 128 256
Die IP-Adressen 0 2 6 14 30 62 126 254

Ich hoffe das hilf
