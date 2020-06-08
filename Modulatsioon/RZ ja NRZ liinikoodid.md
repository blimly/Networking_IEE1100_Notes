# RZ ja NRZ liinikoodid
## NRZ liinikood
- NRZ liinikood on lihtsa teostusega, [[Bipolaarne liinikood|bipolaarsel]] kujul alaliskomponendivaba ja suhteliselt kitsa ribalaiusega
- Probleemid tekivad olukorras, kui edastatakse järjest suuremal hulgal ainult ühtesid või null. Sellisel juhul püsib pinge konstantselt samal nivool ja vastuvõtjal tekib raskuseid järjestikuste sümbolite omavahel eristamisega.
- Probleem tekib pealmiselt sellepärast, et saatja ja vastuvõtja kellad käivad praktikas veidi erinevate kiirustega ehk pole omavahel **sünkroniseeritud**
- Seetõttu tekib varem või hiljem olukord, kui saatja edastab alles n-indat bitt, aga vastuvõtja võtab enda arvates vastu järgmist bitti

### NRZI liinikood
- Taolisest puudusest on vaba **NRZI** (*Non Return to Zero Inverted*) liinikood. NRZI liinikoodi korral ei näita edastava sümboli $a_k$ väärtust mitte signaali nivoo vaid hoopis selle muutumine
- Kui signaali väärtus jääb järgmise biti kestuse ajal samaks, siis edastatakse ühete sümbolit väärtust ja kui muutub, siis teist.

### NRZM liinikood
- Juhul kui nivoo muutus, kas madalalt kõrgele või kõrgelt madalale, vastab sümboli väärtusele $a_k = 1$ on tegemist **NRZM** (*Non Return to Zero Mark*) variandiga NRZI liinikoodist. Sümboli $a_k = 0$ edastamisel jääb sellisel juhul signaali nivoo smaks. 
- Kuna andmed on kodeeritud nivoo muutustena või nende puudumisena, siis esimene nivoo iseenesest informatsiooni ei kanna
- NRZM liinikood mis kujutab bitijada: `10111`
	- ![[Pasted image 6 1.png]]

### NRZS liinikood
- Vastupidisel juhul, kui nullile vastab muutus ja ühele signaali konstantseks jäämine, on tegemist **NRZS** (*NRZ-Space*) liinikoodiga

Mõlemad NRZM ja NRZS on immuunsed polaarsuse muutumisele ülekandel

## RZ liinikood
- Sünkroniseerimisprobleemide lahendamiseks tuleb kasutada liinikoode, kus iga üksik sümbol pikast ühetaoliste jadast oleks selgelt eristatav
- Üheks võimaluseks on **RZ** (*Return to Zero*) liinikoodid
- Unipolaarse RZ liinikoodi korral vastab biti väärtusele `1` poole sümboli kestusega kõrge impulss. Poole peal läheb pingenivoo tagasi null, selat ka koodi nimetus. Nullile vastab sellisel juhul konstantne nullnivoo
- Unipolaarne NRZ koodi korral on pikas ühtede jadas iga sümbol eraldi tuvastatav, kuid pika nullide jada korral oleme ikka sama probleemi ees, mis enne

### Unipolaarne RZ liinikood
- Bitijadale `11101` vastav signaalipinge ajaline kuju
	- ![[Pasted image 8 1.png]]
- RZ liinikood lihtsustab vastuvõtja sünkroniseerimist saatja kellaga
- Poole kitsam impulssi kestus tähendab, et signaali ribalaius $B$ on sama edastuskiiruse $R$ korral kaks korda suurem
- Poole lühema impulssi tõttu on biti `1` energia poole väiksem

$$E_b = \frac{U^2T_b}{2}$$

### Bipolaarne RZ liinikood
![[Pasted image 9 1.png]]
- Iga sümbol on teistest eristatav. Öeldakse, et liinikood on **isesünkroniseeruv**
- Kahe sümboli edastamiseks kasutatakse kolme erinevat pingenivood ($+U, 0, -U$)
- Miinuseks võrreldes NRZ liinikoodiga on ka siin suurem ribalaius $B$ ja väiksem biti energia $E_b$
- Nagu kõigi bipolaarsete liinikoodide korral puudub ka siin alaliskomponent $U_0$