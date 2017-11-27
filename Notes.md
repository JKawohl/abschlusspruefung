Notes:

#DHCP: Dynamic Host Configuration Protocoll
#DDR : Double Data Rate
#LTO: Linear Tape Open
#S.M.A.R.T. tools:
Self-Monitoring, Analysis and Reporting Technology:
#ECC RAM
ECC- und Paritätsprüfung    
Ein error-correcting code (ECC) ist eine Kodierung zur Fehlerkorrektur, die im Gegensatz zur Paritätsprüfung in der Lage ist, einen 1-Bit-Fehler zu korrigieren und einen 2-Bit-Fehler zu erkennen. Das ECC-Verfahren benötigt auf 32 Bit 6 Check-Bits und auf 64 Bit 7 Check-Bits[8].

Das ECC-Verfahren wird häufig in Speicherbausteinen für Serversysteme eingesetzt, die eine besonders hohe Datenintegrität benötigen.

#Firewall
##Paketfilter
Einfach aber wirkungsvoll: der 'Paketfilter'
Ein Paketfilter entscheidet anhand verschiedener Kriterien , ob ein Paket ausgeliefert, zurückgewiesen oder still verworfen wird. Kriterien hierfür sind: Quell- oder Ziel-Adresse eines Paketes, Quell- oder Ziel-Port eines Paketes und der Protokoll-Typ. So sollte eine Firewall, die ihr lokales Netz (Intranet) schützt, eine Regel beinhalten, die die Ports 137 bis 139 für ein- und ausgehenden Verkehr blockiert. Denn über diese Ports kommunizieren Windows-Freigaben, d.h. ihre freigegebenen Ordner im Netz. Wer möchte schon die im heimischen Netz freigegebenen privaten Ressourcen im Intenet zur Verfügung stellen?
Diese definierten Kriterien zusammen bilden ein Regelwerk, vorstellbar als lange 'Checkliste', anhand dessen eine Firewall die Entscheidung trifft, ob ein Paket abgewiesen oder weitergeleitet wird.

##Stateful Inspection
Eine Erweiterung der einfachen Paketfilter besteht darin, über die einfachen Kriterien der Quell- und/oder Zieladresse sowie Ports hinaus, den Zustand jedes Paketes zu untersuchen und für bestimmte Verbindungen eine Statustabelle zu führen.
So kann die Firewall nachvollziehen, ob ein bestimmtes Paket den Start einer neuen, den Teil einer bereits existierenden Verbindung oder ein ungültiges Paket darstellt. Damit kann die Anzahl der zu überprüfenden Regeln für ein bestimmtes Paket, und damit die zu einer Überprüfung notwendige Zeit sowie die Komplexität des Regelwerkes gesenkt werden. Hierbei wird zu Beginn der Überprüfung abgefragt, ob dieses Paket Teil einer bestehenden Verbindung ist. So kann ein Paket einer bereits bestehenden Verbindung durchgelassen werden, ohne sämtliche (nachfolgenden) Regeln überprüfen zu müssen.

##Deep Packet Inspection durch Application Level Firewall
Tiefer eingreifende Firewalls verfolgen zudem den Ansatz, neben Absender und/oder Empfänger eines Paketes zusätzlich den übermittelten Inhalt zu untersuchen. Im Unterschied zu 'Paketfilter' und 'Stateful Inspection' wird hier der Netzwerkverkehr nicht nach Überprüfung weitergeleitet oder verworfen, stattdessen übernehmen so genannte Proxys, bzw. 'Stellvertreter' den Part der eigentlichen Kommunikation als Vermittler. Nicht Ihr Rechner selbst kommuniziert dann mit Servern im Internet, sondern der Proxy übernimmt diese Aufgabe. Auf diesem Weg kann Schadsoftware, also beispielsweise Viren oder Trojaner aus der Netzwerkkommunikation herausgefiltert werden, noch bevor diese Ihren Rechner erreichen.
Diese weitergehende Untersuchung des Datenverkehrs stellt allerdings zusätzliche Anforderungen an die Ressourcen des Computers, auf dem diese Firewall-Technologie zum Einsatz kommt.

#Verschlüsselung
##Symmetrische Verschlüsselung

Bei der symmetrischen Verschlüsselung wird ein und derselbe Schlüssel verwendet, um Botschaften zu verschlüsseln und auch wieder zu entschlüsseln. Der Schlüssel muss also sowohl dem Sender als auch dem Empfänger bekannt sein und zu diesem Zweck vorher ausgetauscht werden. Das ist gleichzeitig auch der Nachteil dieser Verschlüsselungsart, da durch den Austausch das Risiko besteht, dass der Schlüssel beim Übermitteln unbefugten Personen bekannt werden könnte. Idealerweise müsste die Übergabe des Schlüssels auch verschlüsselt werden, was innerhalb der symmetrischen Verschlüsselung zu einem Paradoxon führt.

Bei unserem Beispiel treffen wir wieder auf Alice, Bob und Eve: Möchte Bob eine verschlüsselte Liebesbotschaft an Alice schicken, muss er ihr vorher den geheimen Schlüssel übergeben. Die eifersüchtige Eve könnte die verschlüsselte Nachricht und den Schlüssel beim Übermitteln abfangen. Noch dramatischer wird es, wenn wir uns vorstellen, dass Alice in einem Land lebt, wo die Behörden gerne Zugriff auf alle Daten hätten und es keinen „sicheren Hafen“ für Geheimnisse mehr gäbe. Das Abfangen von verschlüsselten Nachrichten und versendeten Schlüsseln ist ein Kinderspiel für solche Behörden.

##Asymmetrische Verschlüsselung
Doch wie funktioniert die asymmetrische Verschlüsselung? Bei der Verschlüsselung kommen die von Mathematikern oft verehrten Primzahlen zum Einsatz. Für alle Leser, bei denen der Matheunterricht schon etwas länger her ist, kurz zur Auffrischung: Eine Primzahl ist eine Zahl, die nur durch sich selbst und durch 1 geteilt werden kann. Zum Beispiel ist 7 eine Primzahl, weil sie nur durch 1 und durch 7 (ohne Rest) geteilt werden kann. Hingegen ist die 8 keine Primzahl, weil sie zusätzlich zu 1 und 8 auch durch 2 und durch 4 geteilt werden kann.

Wenn Alice ein Schlüsselpaar erzeugen möchte, benötigt sie zwei Primzahlen. Nehmen wir für die erste Primzahl p = 349 und für die zweite Primzahl q = 577. Die Multiplikation dieser beiden Zahlen ergibt N= 349 x 577 = 201 373. N = 201 373 ist nun Alices öffentlicher Schlüssel, den sie der Welt mitteilen kann. Da nur ihr die Werte p und q bekannt sind, kann nur sie die Nachricht entschlüsseln. Eve müsste also die Werte p und q herausfinden, das heißt die Frage beantworten, welche Zahlen miteinander multipliziert den Wert 201 373 ergeben. Man nennt diesen Vorgang Faktorzerlegung oder Faktorisierung.

Primzahlen eignen sich für die Verschlüsselung deshalb, weil ihre Kombination (welche Primzahlen ergeben 201 373) schwieriger zu erraten ist als bei Nicht-Primzahlen (zusammengesetzte Zahlen). Bei den letzteren gibt es nämlich mehrere Kombinationsmöglichkeiten die zum Ergebnis führen könnten, bei den Primzahlen nur eine.
Bei den bisherigen Verfahren hatte man das Problem der Schlüsselübergabe. Man musste den Schlüssel stets geheimhalten, denn eine Veröffentlichung hätte es notwendig gemacht, einen neuen Schlüssel zu verwenden.

Das Public-Key Verfahren beruht deshalb auf zwei Schlüsseln. Einem öffentlichen (offen zugänglich) und einem privaten (geheim). Der eine Schlüssel wird vom anderen abgeleitet. Bei einem guten asymmetrischen Verfahren gibt es keine Möglichkeit aus einem Schlüssel den anderen zu berechnen.

Wenn man nun eine geheime Botschaft übermitteln will, verschlüsselt man sie mit dem Public Key des Empfängers. Das Entschlüsseln ist mit diesem nicht möglich. Der Empfänger kann die Botschaft nun mit seinem geheimen Private Key einfach entschlüsseln.

Die Schlüssel sind ein Produkt aus Primfaktoren. Der Code ist es zwar einfach durch mehrfache Divison bis zu den Primzahlfaktoren herauszufinden, aber dies ist bei langen Schlüsseln viel zu zeitaufwendig. Etwas schneller geht es mit Faktorisierungsalgorithmen. Der neueste dieser Art ist das so genannte Zahlenkörpersieb (Number Field Sieve, NFS), mit dem sich die Suchzeit um ein Zehnfaches verkürzt.

Momentan ist es möglich eine Zahl mit 130 Dezimalstellen (etwa 440 Bit) in ihre Primfaktoren zu zerlegen. Dies dauerte in einem Versuch, an dem 1600 Rechner, die über das Internet verbunden waren, beteiligt waren, ganze 8 Monate.

Ein Verfahren, mit dem es schneller geht, wird in nächster Zeit nicht erwartet.

Es gibt zwei Algorithmen, die zur Zeit sehr häufig benutzt werden: ElGamal und RSA.

#IPv6
Subnetz berechnung: Es ist immer empfohlen 64 bit als host identifier zu haben:
Also bei /60 hat man 128 - 60 = 68 
Minus 64 bit Hostidentifier = 4 Bit 
2^4 = 16


    