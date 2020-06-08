# Hammingi kood
- Lineaarne binaarne [[Vigu parandavad koodid#Plokk-kood|plokk-kood]] minimaalse kaugusega $h_{min} = 3$
- Iga täisarvu $r \geq 2$ korral on ploki pikkus $n = 2^r - 1$, millest informatsiooni kannab $k = 2^r - r - 1$ bitti ja ülejäänud on paarsusbitid
- **Koodi kiiruseks** (*code rate*) nimetatakse informatsiooni edastavate bittide arvu $k$ suhet  kogu ploki pikkusesse $n$. $R= k/n$
- Hammingi koodi kiirus 

$$R = 1 - \frac{r}{2^r - 1}$$
- Suudab parandada ühekordseid bitivigu
- Näiteks Hamming (127, 120) kiirus on $R = 0.94$

## Hamming (7, 4)
- Olgu $r = 3$
- Koodsõna pikkus: $n = 2^3 - 1 = 7$ bitti
- Infot kannavad: $k = 2^3 - 3 - 1 = 4$ bitti
- Ülejäänud $7-4=3$ on konrollitud liiasust kanvad paarsusbitid
- Koodi kiirus $R = 4/7 \approx 0.57$ seega 57% edastatavatest bittidest sisaldavad andmeid
- Kuna praktikas on bitivigade tõenäosus palju väiksem kui $1/7$, siis kasutatakse pikema koodsõnaga Hammingi koode
- Paarsusbittide leidmine
	- ![[Modulatsioon/Pasted image 9.png]]
	- Paarsusbitid $p4, p2, p1$ leitakse andmebittide $d3$ ja $d5 - d7$ mooduliga kaks summeerimise teel
		- $p4 = d7 \oplus d6 \oplus d5$
		- $p4 = d7 \oplus d6 \oplus d3$
		- $p4 = d7 \oplus d5 \oplus d3$
- ==Sõnum **d**:== `1101`
	- $p4 = 1 \oplus 1 \oplus 0 = 0$
	- $p4 = 1 \oplus 1 \oplus 1 = 1$
	- $p4 = 1 \oplus 0 \oplus 1 = 0$
- **Koodsõna c**: 110==0==1==10==
---
- Koodsõna on seitsmebitine, siis võimalike koodsõnade arv on $2^7 = 128$
- Lubatud koodsõnu on aga ainult 16 (iga kaheksas)
- Koodis kaugus $h_{min} = 3$

## Vigase biti tuvastamine
- Vastuvõetud koodsõna põhjal arvutatakse välja **sündroom** $s$
	- $A = p4 \oplus d7 \oplus d6 \oplus d5$
	- $B = p4 \oplus d7 \oplus d6 \oplus d3$
	- $C = p4 \oplus d7 \oplus d5 \oplus d3$
- Kui sündroomi väärtus on 0, siis on sõnum vigadeta
- Vastasel juhul näitab sündroom vigase biti järjekorranumbrit
- Vea parandamiseks tuleb bit vastupidiseks muuta
![[Modulatsioon/Pasted image 10.png]]

## Maatriksid
### Genereeriv maatriks
![[Modulatsioon/Pasted image 12.png]]
- Genereeriva maatriksi ridade arv on võrdne sõnumi $d$ bittide arvuga $k$, veergude arv on aga võrdne koodsõna $c$ pikkusega $n$ ($k \times n$ maatriksis)
- Sõnumile $d$ vastav koodsõna $c$ leitakse korrutisena:

$$c=dG$$
### Paarsuskontrolli maatriks
![[Modulatsioon/Pasted image 13.png]]
- Kasutatakse sündroomi arvutamiseks ehk vigade tuvastamiseks 
- Paarsuskontrolli maatriksil on $n$ rida ja $n-k$ veergu
- Sündroom $s$ leitakse

$$s=cH$$


