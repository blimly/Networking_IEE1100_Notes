# Informatsioon
- **Informatsioon** - teadmatuse vähenemise määr või üllatuse suurus
- **Teadmised** - õigustatud tõene uskumus (filosoofia)
- **Andmed** - muutujate **x** väärtused 
	- reaalsed konkreetsed arvud
	- **x** võib olla kelirõhu väärtus mikrofoni sisendis, pikslite heledused, mälupesade väärtuses jne

Informatsiooni hulka saab numbriliselt väljendada mingis sümbolis $a$ sisalduva (Shannoni) **informatsiooniga**

$$I(a_i)=log_c\left[\frac{1}{p(a_i)}\right] = -log_c p(a_i)$$

- Info mõõtühikud on sõltuvalt logaritmi alusest:
	- $c=2$ bitt, bait(8 bitti), nibble(4 bitti)
	- $c=e$ nat
	- $c=10$ hartley

## Info tekkekiirus
- Kui allika sümbol $a_j$ kestab aja $T_s$ vältel, siis väljastatakse uus sümbol iga $T_s$ sekundi tagant. Sellisel juhul saab öelda, et allika **sümbolikiirus on $r_s=1/T_s$ baudi ehk sümbolit sekundis**.
- Allika keskmine info tekkekiirus $R(A)$ on võrdne entroopia $H(A)$ ja sümboli kestuse $T_s$ suhtega:

$$R(A)=\frac{H(A)}{T_s}=r_s\cdot H(A)$$

- Reaalsete allikate informatsiooni tekkekiirus võib olla väga suur, seega on tihtipeale vaja informatsiooni hulka enne edastamist kuidagi kärpida.