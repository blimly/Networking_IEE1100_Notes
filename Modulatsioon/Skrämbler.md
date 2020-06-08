# Skrämbler (*Scrambler*)
- Füüsilise kihi seade mille ülesandeks on bittide väärtuste (pseudo) juhuslik ümbersuunamine
- Kasutamise põhjused:
	- Vältimaks pikki, ainult ühest sümbolist, koosnevaid jadasi
		- `...1111111111111111111...`
	- Lihtsustamaks vastuvõtjas kella sünkroniseerimist (*Clock Recovery*)
	- Tagab ülekantava signaali spektri kuju sõltumatuse edastatavast informatsioonist
	- Kui, reegel, mille järgi bittide järjekorda muudetakse ei ole teada, siis põhimõtteliselt tagab ka andmete trualisust ülekandel (krüpteerimine)

## Aditiivne skrämbler
- Nimetatakse ka sünkroonseks skrämbleriks (*additive or synchronous scrambler*)
- Edastatavale signaalile liidetakse (mooduliga kaks) **pseudojuhuslik** binaarne jada
- Liidetav binaarne jada võib olla mällu salvestatud, kuid tavaliselt tekitatakse see tagasisidestatud nihkeregistriga (LFSR). Tekitav pseudojuhuslik jada on täielikult määratud nihkeregistri algsisu ja genereeriva polünoomiga (tagasiside võtmise kohtadega)
- Tagamaks algsete andmete korrektset taastamist peab deskrämbler töötama sünkroonselt, selleks lisatakse edastavatele andmetele sünkrosõnad
- **Additiivse skrämbleri näide**
	- Olgu edastatav bitijada järgmine 
		- `11111111 01111010`
	- Skrämbleri poolt liidetav pseudojuhuslik binaarne jada
		- `10101101 00010110`
	- Nende summa mooduliga kaks
		- `01010010 01101100`
	- Tulemuseks on palju rohkemate muudatustega bitijada
- **Deskrämbleri näide**
	- Vastuvõtjas tuleb esialgsete andmete taastamiseks liita vastuvõetud bitijadale sünkroonselt sama pseuojuhuslik jada
		- ![[Pasted image 35.png]]
	- Kui vastuvõtjas ei ole pseudojuhuslik jada saatja omaga sünkroonis on tulemuseks väljaloetamatu signaal
		- ![[Pasted image 36.png]]

## Multiplikatiivne skrämbler 
- Nimetatakse ka isesünkrooniseeruvaks skrämbleriks (*multiplicative or self-synchronizing scrambler*)
- Korrutab sisendsignaali iseenda ülekandefunktsiooniga (z-ruumis)
- Ei vaja sünkroniseerimist
- On määratud samuti polünoomiga. 
- Algseis pole kriitiline
- Kui deskräbleri sisendis on ühekordne viga, siis väljundis on vigade arv korrutatud tagasisideühenduste omaga 

![[Pasted image 37.png]]

- Olgu skrämbleri algseis saatjas `0x07E7E`
- Edastatava kaadri algus enne skrämleerimist oli:
	- `0x01 0xA6 0x6E 0xE9 0xB9 0xA6...`
- Vastuvõtjas polnud skrämbleri algseis teada ja seetõttu oli deskrämleri algseis vaikimisi `0x00000` 
- Deskrämbleeritud kaadri algus peale deskrblerit oli
	- `0xD9 0x79 0x6E 0xE9 0xB9 0xA6...`