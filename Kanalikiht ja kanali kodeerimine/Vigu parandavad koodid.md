# Vigu parandavad koodid
- **[[Veatuvastus#FEC|FEC]]** (*Forward Error Correction*)
- Saavutatakse kontrollitud liiasuse lisamisega
- [[Hammingi koodid]]
	- Kolmkordselt kordav kood - Hamming (3, 1)
	- Hamming (7, 4)
- [[Reed-Solomoni koodid]]
	- CD, DVB, WiMAX, QR
- BCH Koodid
- [[Konvolutsioonilised koodid]]
- Võrekoodid
	- Viterbi algoritm
- Turbokoodid
	- 3G/4G mobiil, kosmoseside
- LDPC koodid (Gallageri koodid)

## Plokk-kood
- Fikseeritud pikkusega $n$ koodsõnad $c_i$
- Edastatavale informatsioonile $d_i$ pikkusega $k$ lisatakse kontrollitud liiasus pikkusega $n-k$
- Kood on **süstemaatiline**, kui koodsõna sisaldab informatsiooni $d_i$ muutmata, eraldataval kujul
- Kood on **lineaarne**, kui mistahes kahe koodsõna $c_i$ ja $c_j$ liitmisel saadakse samuti koodsõna

---
- Plokk koodis on võimalik $n-k$ paarsusbitiga tagada koodi minimaalne kaugus $n-k$
- Selline kood on v]imeline parandama vigu kordsusega kuni

$$t = \Bigg \lfloor \frac{n-k}{2} \Bigg \rfloor$$

## Mõisted
- **Hammingi kaal** - Koodsõna $c$ hammingi kaaluks $w\{c\}$ on mittenulliste koordinaatide arv
- **Hammingi kaugus** - Kahe koodsõna $c_i$ ja $c_j$ vaheliseks kauguseks nimetatakse nende kooridnaatide arvu, mills nad üksteisest erinevad $h = d\{c_i, c_j\}=w\{c_i \oplus c_j\}$
- **Minimaalne kaugus** - koodi $C$ minimaalseks kauguseks $h_{min}$ nimetatakse kahe erineva koodsõna **vähimat** kaugust $h_{min} = d\{c_i, c_j\} \quad i \neq j$