# Networks Essentials

## Examen

Bedrijven van hoofdstuk 3.1 => Je moet ze ze herkennen, maar je moet ze niet heel specefiek kennen

## Network Components

Om te beginnen hebben we de Hosts, Cisco benoemd dit als "Alle apparaten die een nummer hebben gekregen waarmee ze
kunnen communiceren.' Zo een nummer noemen ze ook wel een IP-adress, IP staat voor Internet Protocol. Dit adres wordt
gebruikt om de host (bijvoorbeeld jouw computer) en het netwerk waarmee deze verbonden is, te identificeren.

Je hebt ook Clients, dit zijn eigenlijk de 'eindpunten', dat betekent dat het erna niet meer verder verstuurd worden.
Clients zijn een type van host. ze gebruiker software om informatie op te vragen en weer te geven. Als je een website
wilt bezoeken ga je eigenlijk aan de server vragen hoe de website er uit ziet en die server laat uw browser weten hoe
dat de HTML er uit ziet en dus ook hoe dat de webpagina die je ziet er uit moet zien.

Je hebt dus eigenlijk de client die via het internet info vraagt aan de server, oftewel: </br>
Client ↔ internet ↔ Server

> heb hiertussen even een les gemist

## OSI model (Module 3)

### Application Layer

HTTP-Protocol; IMAP-protocol, DHCP...
HTTP Protocol doet eigenlijk 3 verschillende lagen.

### Presentation Layer

Encryption of decryption!

### Session Layer

Zet de verbinding op tussen begin device en end device. => Die verbinding dient om te controleren of de data is
aangekomen of dat de data correct is. Elke communicatie is een nieuwe verbinding. Als je surft naar www.hbvl.be dan gaat
je computer 2 sessions openen. Eentje vanuit de router om te vragen voor de website en eentje vanuit de server om te
versturen.

### Transport Layer

Kapt de data op in kleine stukken, hierdoor kan hij meer informatie versturen in kleine karretjes. afhankelijk van UCP
of TCP is het rond de 9000 bytes.

Maakt gebruik van een poort => Die poort wordt gebruikt om bij uw computer te weten van welke processen ze komen, en
naar welke processen ze moeten gaan. Die wordt dus omgedraaid. (ge hebt een source-poort en een destination-poort, bij
het reageren worden de destination poort en de sourcec poort omgewisseld).

#### TCP (Connection oriented)

Wat wilt connection oriented zeggen? => Er wordt een connectie opgezet.
Error free => als er een error is, wordt het terug gestuurd en het juiste opgevraagd.
Same order delivery => Wordt in dezelfde volgorde gezet.
TCP heeft ook Flow control => Als de buffers vol zijn gaat die zeggen dat ge wat trager moet gaan, en als die terug leeg
zijn ga je meer kunnen versturen.

<br/>
Alles wat correcte data kan opleveren is TCP (TCP buffered).

#### UDP (ConnectionLess)

ConnectionLess => Geen session.
Geen Same Order delivery => Moet niet in de juiste volgorde staan.
Waarom gebruiken we UDP => Sneller => Ook is er geen connectie, wat betekent dat je sneller kunt gaan, vrt moet 1 stream
maken en die stream wordt doorgestuurd. Als je via TCP zou gaan zou een live-uitzending mega zwaar zijn op de server van
VRT. <br/>
Alles wat incorrecte data is UDP (UDP hapert)

### Network Layer

IP => Zorgt voor routing, en wilt weten waar het begin en het einde is. Die gaat van netwerkkaart naar netwerkkaart, ja
ik begrijp dit ook nog altijd niet per se.

Die router gaat beslissen of hij die naar links of naar rechts moet sturen. Die weet niet per se waar dat hij naar toe
moet gaan. Maar die weet wel dat die gewoon naar links of naar rechts moet, en weet welke kant de meeste uit zijn. In de
plaats van die exact naar die plaats te sturen, stuurt die gewoon naar een andere netwerkkaart.

### DataLink Layer

Physical Layer + DataLink Layer = taak van de netwerkKaart

#### LLC(Logical link control)

Driver van netwerkkaart.

Controleren of de data wel goed is

#### MAC-adressen

ookwel fysiek adres genoemd. Altijd uniek (in theorie).
Worden gebruikt om te communiceren tussen 2 netwerkkaarten.
Bij de packets die deze stuurt wordt een header gezet met de MAC adres van de

### Physical Layer

Zet 011010110101 (bits) Om naar elektrische pulsen en andersom.

### Encapsulation

Je hebt de basis data; en dan voeg je der een header aan toe, die bundel stuur je door, en daar voeg

### Segmentation

Het een voor een uit elkaar halen van de headers

### Unicast, Multicast, Bordcast

Unicast => één op één verbindingen (99% van het internetverkeer) <br/>
Multicast => Je stuurt naar iedereen van het gamen waar je zit,... <br/>
Broadcast => Je stuurt naar iedereen van het netwerk. Als je bijv wilt weten welk ip adress, dan stuur je een broadcast
voor de DHCP (discovery protocol) server. en die stuurt dan een unicast terug.

### Protocol Functions

TCP heeft ze allemaal

## Pysical layer

### Latency vs bandbreedte

Latancy is hoe lang het duurt, bandbreedte is hoe snel het gaat. Deze 2 hebben niet veel met elkaar te maken.