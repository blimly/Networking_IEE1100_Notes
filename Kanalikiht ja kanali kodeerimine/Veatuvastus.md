# Veatuvastus
- Üldjuhul pole ülekandel tekkiv vigade hulk aksepteeritav, seega peab korralik sidesüsteem omama võimekust vigade mõju vähendamiseks. Selleks on kaks võimalust 

### ARQ
(*Automatic Repeat reQuest*) 
Vigade otsimine ja tuvastamine. Kui viga leitakse, siis palub vastuvõtja saatjal andmed uuesti edastada
![[Modulatsioon/Pasted image 4.png]]

#### HARQ
(*Hybrid Automatic Repeat reQuest*)
![[Modulatsioon/Pasted image 22.png]]

### FEC
(*Forward Error Correction*) 
Kui andmete uuesti saatmine pole võimalik, siis kasutatakse algoritme mis võimaldavad kontrollitud liiasuse lisamisega saatja poolel tekkinud vigade paramdamist vastuvõtjas
![[Modulatsioon/Pasted image 21.png]]

## Kontrollsumma
- Kõige lihtsam meetod vigade tuvastamiseks aga ebatõhus
- Arvutatakse edastavate andmete liitmise teel
- Väiksemate andmehulkade korral liidetakse andmed kokku bitthaaval mooduliga kaks
- Suuremate kaadrite korral tehakse liitmist tavaliselt ühe või mitme baidi kaupa, kasutatava moodul sõltub liidetavate baitide arvust
- Paarsuskontroll on sobilik kasutamiseks üksikute sümbolite edastamisel, nagu näiteks üle RS-232 või RS-485 liidese
- Suuremate kaadrite edastamisel kastutatakse vajadusel pikemat kontrollsummat. 
- Ühebaidist kontrollkoodi leidmiseks on vaja liita mooduliga $n =2^8 = 256$
	- Olgu edastav kaader: `1011 0010  0101 1101  1000 1000`
	- Kümnendkujul oleks: `178  93  136`
	- Kontrollsumma: $(178 + 93 + 136) mod(256) = 151$
	- Tulemus:  `178  93  136  151`

## Paarsuskontroll
- Lihtsaim ja levinuim kontrollsumma kasutamise viis
- Lisatakse $n$ bitti andmeid sisaldavale sõnumile üks **paarsusbitt** $p$. Paarsusbiti väärtus valitakse selline, et ühtede hulk edastuse (andmed + paarsusbitt) oleks alati paarisarv (*even parity*)
	- Näiteks ASCII sümbolile `F` vastab koodõna `1000110`
	- Andud koodsõnas on kolm ühte, ehk ühtede arv on paaritu
	- Seega peab lisatava paarsusbiti väärtus olema `1`, et saaksime kokku paarisarvu ühtesid: `10001101`
- Kui vastuvõtja tuvastab vastuvõtul paaritu arv ühtesid, siis on ilmselgelt ülekandel viga tekkinud.
- Paarsusbiti väärtuse saab leida kui liidame kõik edastava sümboli bitid omavahel mooduliga kaks kokku

[[Tsükliline liiasuse kontroll]]
