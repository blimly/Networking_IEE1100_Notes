# Genereeriv polünoom
- [[Kontrollkood|Kontrollkoodi]]  väärtus sõltub edastatavatest andmetest ja kasutatavast genereerivast polünoomist $g(x)$
- Konkreetse vetuvastuse kvaliteet sõltub samuti genereerivast polünoomist, osad neist on paremad kui teised
- Genereeriva polünoomi pikkus on ühevõrra suurem [[Kontrollkood|kontrollkoodi]] omast ja tema esimene (kõrgeim) bitt on **alati 1**
- Genereeriv polünoom esitatakse kas polünoomi kuijul või kuueteistkümnendsüsteemis arvuna
	- Kuna esimene bitt on alati üks, siis seda kuueteistkümnendkujul eraldi välja ei kirjutata

## [[Tsükliline liiasuse kontroll|CRC]]-4
- Kasutatakse neljapbitise [[Kontrollkood|kontrollkoodi]] arvutamiseks 
	- Genereeriv polünoom: $x^4 + x + 1$
	- Hex: `0x3`
	- Bin: `10011`

## [[Tsükliline liiasuse kontroll|CRC]]-16-CCITT
- Kasutatakse kuueteistkümnebitise [[Kontrollkood|kontrollkoodi]]  leidmiseks
	- Genereeriv polünoom: $x^{17} + x^{16} + x^6 + 1$
	- Hex: `0x1021`
	- Bin: `1 00010000 00100001