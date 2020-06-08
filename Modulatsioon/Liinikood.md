
# Liinikood
- Sidekanalis ülekantavad andmed, ehk muutujate väärtused, on oma olemuselt abstraktsed arvud
- Andmete ülekandmiseks üle füüsilise kanali (kaabel, raadiolink) tuleb abstraktsetele sümbolitele $a_k$ vastavusse panna reaalsed signaalid
- Kuna andmeside toimub elektromagnetnähtustele tuginedes siis on tegemist elektrilisete signaalidega
- Vastavust digitaalsete sümbolite $a_k$ ja neid kirjeldavate pingete vahel nimetatakse **liinikoodiks**
- Arvutites esitatakse andmeid kahendsüsteemis seega koosneb võimalike sümbolite $a_k$ hulk kahest elemendist $\{0, 1\}$
	- Tavaliselt vastab biti väärtusele `0` madal pingenivoo, enamasti 0 volti.
	- Biti väärtusele `1` kõrge, enamasit positiivne pingenivoo $+U$

$$u(t) = 
  \begin{cases} 
   0 & \text{, kui } a_k = 0 \\
   +U &\text{, kui } a_k = 1
  \end{cases}
$$
- Konkreetsed pingenivoode väärtused sõltuvad kasutatavast tehnoloogiast
	- Näiteks TTL loogika korral loetakes madalaks pingeid alla 0.8V ja kõrgeks pinget alates 2V kuni toitepingeni (tavaliselt +5V)
- Signaali väärtus püsib konstantsena ühel kahest nivoost kogu **biti kestuse** $T_b$ vältel: $nT_b \leq t < (n+1)T_b$ kus $n$ on biti järjekorranumber 
- Kahendarv `10010` liinikoodina:
	- ![[Kanalikiht ja kanali kodeerimine/Pasted image 23.png]]


## Diferentsiaalne kood 
- Sidekanalis võib juhtuda, et siganaali polaarsus muutub vastupidisek. Näiteks kui keerdpaarkaablis kiud kogemata valet pidi ühendada.
- Sellisel juhul peab vastuvõtja NRZ(L) liinikoodi kasutamise korral ekslikult kõiki edastatud ühtesid nullideks ja vastupidi

## Liinikoodi vastuvõtt
- Vastuvõtjas mõõdetakse signaalipinge $u(t)$ väärtust korra biti kestuse $T_b$ jooksul
- Seda üritatakse teha võimalikult sümboli keskel
- ![[Pasted image 7 1.png]]
- Mõõdetud väärtust võrrledakse lävega $U_l$. Sõltuvalt sellest kas pinge on lävest suurem või väiksem on tegemist vastavalt ühe või teise biti väärtusega
- Lävipnge väärtuseks võetakse tavaliselt pool signaalipinge maksimaalse ja minimaalse väärtuse vaheline keskpunkt

$$U_l = \frac{+U-(-U)}{2}$$

## Liinikoodide võrdlemine
- Liinikoodi spektri kuju (ribalaius $B$)
- Tundlikus häirete ja mürade suhtes - veakindlus
- Vigade tuvastamise võimalused
- Sünkroniseerimise lihtsus
- Rakendamise hind ja keerukus

## Liinikoodide näiteid 
![[Pasted image 11 1.png]]

---
- [[Unipolaarne NRZ liinikood]]
- [[Bipolaarne liinikood]]
- [[Liinikoodi spekter]]
- [[RZ ja NRZ liinikoodid]]
- [[M-positsioonilised liinikoodid]]
- [[Otsustusseade]]
- [[Liinikoodi häirekindlus]]