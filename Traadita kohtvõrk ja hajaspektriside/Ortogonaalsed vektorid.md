# Ortogonaalsed vektorid
![[Kärgvõrgud ja mobiilside/Pasted image 4.png]]
- Kaks vektorit $\vec{a}$ ja $\vec{b}$ on **ortogonaalsed**, kui nende skalaarkorrutis on võrdne nulliga: $\vec{a} \cdot \vec{b} = 0$
- Ortogonaalsed vektorid on alati omavahel risti

## Funktsioonide skalaarkorrutis
- Funktsioonide $x(t)$ ja $y(t)$ skalaarkorrutis on defineeritud kui 

$$\langle x, y \rangle = \int_a^b x(t)y(t)dt$$

- Öeldakse, et signaalid on omavahel ortogonaalsed kui neid kirjeldavate funktsioonide skalaarkorrutis on null:
	- $$\langle x,y \rangle = 0$$
- Ortogonaalsete signaalide korral onristkorrelatsiooni väärtus nullkohal samuti null
	- $$R_{xy}(0) = 0$$
- Ortogonaalseid signaale saab edastada kanalis samal sagedusel samaaegselt ilma, et nad üksteist märkimisväärselt mõjutaksid. Selline omadus võimaldab teostada mitmeid erinevaid ressursijaotusmeetodeid (näiteks [[CDMA]])

## Ortogonaalsed signaalid
- Omavahel ortogonaalsed signaalid on näiteks siinus- ja koosinussignaalid

$$\int_0^{nT}
sin \left( \frac{2 \pi t}{T} \right)
cos \left( \frac{2 \pi t}{T} \right) dt = 0
$$

- Omadus leiab rakendust näiteks [[Faasmodulatsioon|PSK]] ja [[Modulatsioon|QAM]] modulatsiooni teostamisel
- [[Sagedusmodulatsioon#Sunde FSK|Sunde FSK]] teostus tugineb teatud sageduserinevusega harmooniliste signaalide ortogonaalsusele
- [[Raadiokanal#Mitmekiireline levi|OFDM]] modulatsioon kasutab sümbolikiiruse vähendamiseks samuti suurt hulka ortogonaalseid kandesignaale

## Ortogonaalse koodi näide
![[Kärgvõrgud ja mobiilside/Pasted image 5.png]]
- Olgu meil kaks (hajutavat) koodi $x(t)$ ja $y(t)$, mõlemad pikkusega kaks
- Saab näidata, et need koodid on omavahel ortogonaalsed
	- $$R_{xy}(0) = 0$$
- Seega saab põhimõtteliselt neid kasutada kahe kasutaja eristamiseks [[CDMA]] kasutavas sidesüsteemis

![[Kärgvõrgud ja mobiilside/Pasted image 6.png]]