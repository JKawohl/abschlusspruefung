Drei Kategorien:
#VFD (Voltage and Frequency Dependent bzw. Offline UPS/USV)


Eine USV dieser Kategorie (Kategorie 3 in der Norm EN 62040-3) leitet den Strom im Normalbetrieb direkt vom Eingang an den Ausgang weiter. Außerdem wird vom Eingang ein Gleichrichter versorgt, der die Akkumulatoren lädt. Sollte die Netzversorgung abbrechen, wird der Ausgang auf einen Wechselrichter umgeschaltet, der aus den Akkumulatoren gespeist wird. Die Umschaltung erfolgt je nach Modell mit einer Verzögerung von bis zu 10 Millisekunden (ms). Darüber hinaus werden nach EN 62040-3 Spannungsschwankungen unter 16 ms sowie Spannungsspitzen zwischen 4 und 16 ms kompensiert. Für einige sehr empfindliche Geräte kann dies bereits zu lange sein. Im Normalbetrieb ist die Höhe und die Frequenz der Ausgangsspannung direkt abhängig von der Eingangsspannung. Diese Art von USVen werden oft mit dem Begriff „Offline“, „Stand by“ oder „passiv“ beschrieben.

##Drei Kernfeatures:
- Umschaltung erfolgt mit "langer" Verzögerung
- Höhe und Frequenz der Ausgangsspannung direkt abhängig von der Eingangsspannung!
- Geringer Schutzt vor Spannungsspitzen 


#VI (Voltage Independent bzw. Netzinteraktive UPS/USV)

In einer USV dieser Kategorie wird ein bidirektionaler Wechselrichter als zentrales Bauteil eingesetzt. Er erzeugt je nach Bedarf aus der Wechselspannung am Eingang die Gleichspannung zum Laden der Akkumulatoren oder aus der Gleichspannung der Akkumulatoren die Wechselspannung am Ausgang. Weil der Umrichter außerdem fortlaufend die Höhe der Spannung am Ausgang begrenzt, ist diese weitgehend unabhängig von der Höhe der Spannung am Eingang. Sofern eine Spannung am Eingang anliegt, bestimmt deren Frequenz aber die Frequenz der Spannung am Ausgang. Die Umschaltzeit bei Stromunterbrechung ist kürzer als bei VFD-USV und liegt bei etwa 2 bis 4 ms. Die Eingangsspannung ist synchron zur Ausgangsspannung.

VI-USVs schützen nicht nur vor den Folgen eines Stromausfalls, sondern auch vor Unterspannung und Überspannung (EN 62040-3 Kategorie 2). Sie werden auch mit den Begriffen „Line-Interactive“, „Single-Conversion“, „Delta-Conversion“ oder „aktiver Mitlaufbetrieb“ bezeichnet.

##Drei Kernfeatures:
- unabhängig von der Höhe der Spannung am Eingang.
- Kurze Umschaltzeit
- Schützt vor Unterspannung und Überspannung




#VFI (Voltage and Frequency Independent bzw. Online UPS/USV)
Bei einer USV dieser Kategorie ist der Eingang direkt auf einen Gleichrichter geführt, der die Akkumulatoren speist. Der Ausgang wird ausschließlich von einem Wechselrichter versorgt, der im Normalbetrieb, also bei vorhandener Netzspannung am USV-Eingang, die notwendige Energie über den Gleichrichter (GR) bezieht und bei Netzausfall über die Batterieanlage (Akkumulatoren) versorgt wird.

Die Wechselspannung am Ausgang wird in jedem Fall – unabhängig von der Qualität der Eingangsspannung – über einen nachgeschalteten Wechselrichter (WR) aus der Gleichspannung des sogenannten Zwischenkreises erzeugt. Zur Erhöhung der Versorgungssicherheit verfügt eine VFI-USV über eine so genannte Bypass-Schaltung, die parallel zur Gleichrichter/Wechselrichter-Kombi geschaltet ist. Bei Überlasten am USV-Ausgang oder Auftreten eines internen Fehlers im Gleichrichter/Wechselrichter-Zweig wird der angeschlossene Verbraucher „unterbrechungsfrei“ auf diesen Bypasszweig umgeschaltet und somit weiter versorgt. Da Gleichrichter und Wechselrichter ständig mit dem vollen Betriebsstrom belastet sind, müssen sie besonders hochwertig sein und machen diese Bauart zur teuersten. Außerdem treten sowohl bei der Gleich- als auch bei der Wechselrichtung Verluste auf, was den Wirkungsgrad verringert. In den Produktbeschreibungen von USV-Anlagen ist in der Regel der Wirkungsgrad bei voller Last angegeben. Da die meisten USV aber nicht voll ausgelastet eingesetzt werden, sind die in der Regel niedrigeren Wirkungsgrade bei Teillast für die korrekte Berechnung des Stromverbrauchs und Kosten entscheidend. Ein Wirkungsgrad von mehr als 95 % bei voller Last kann heute als Standard für eine VFI-USV bezeichnet werden.

Eine VFI-USV (EN 62040-3: Kategorie 1) schützt neben den Folgen eines Stromausfalls, Unterspannung und Überspannung auch vor Schwankungen der Frequenz und vor Oberschwingungen. Sie bieten ebenfalls sporadischen Schutz vor Blitzeinwirkungen und Spannungsverzerrungen (Burst). Sie werden auch mit den Begriffen „Online“, „Double-Conversion“, „Dauerbetrieb“ oder „Doppelwandler“ bezeichnet. USVen der Kategorie 1 werden bevorzugt in Anwendungsgebieten eingesetzt, die hohe Kriterien an die tolerierbaren Ausfallzeiten stellen, wie z.B. in der Stromversorgung eines Rechenzentrums.

Zu beachten ist, dass VFI-USV im Vergleich zu VFD- oder VI-USV den höchsten Eigenstrombedarf haben. Während z. B. eine 650 VA VFD-USV im Leerlauf (ohne angeschlossene Verbraucher) mit ca. 5 W auskommt, eine 850 VA VI-USV mit ca. 15 W, benötigt eine VFI-USV schon im Leerlauf erheblich mehr Strom (eine Faustregel besagt, dass sie ca. 10 % ihrer Nennleistung benötigt, sprich eine 850 VA VFI-USV benötigt im Leerlauf ca. 85 W an Eigenbedarf).

## Kernfeatures:
- Keine Ausfallzeit beim Umschalten
- Teuer
- Hoher Eigenstromverbrauch