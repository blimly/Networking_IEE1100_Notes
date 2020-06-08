
# Kvantimine
- Diskreetimise tulemusena saadud signaalil $s(n \cdot \Delta t)$ on nüüd lõplik arv väärtuseid, kuid väärtuste endi võimalik hulk on ikka lõputu.
- Signaali väärtus igal ajahetkel $n \cdot \Delta t$ mõõdetakse mingi lõpliku täpsusega $\pm q/2$, saadud arvuline tulemus salvestatakse $n_b$ bitist koosneva kahendarvuna


Joonlaual on tavaliselt $q = 1mm$
Kui joone pikkus on näiteks $\pi = 3.14159.. cm$, siis joonlauaga saame mõõtetulemuseks $31 mm$ täpsusega $\pm 0.5 mm$
Tulemus 31 on kaheksabitise ($n_b = 8$) kahendarvuna $0001 1111$

- Sidetehnikas on tavaliselt digitaliseeritavaks signaaliks pinge $u(t)$
- Kvantimissammu väärtus $q$ on määratud digitaliseeritava analoogpinge $u(t)$ muutumispiirkonnaga ($U_{min}$ kuni $U_{max}$) ning tulemuse kirjeldamiseks kasutatavate bittide arvuga $n_b$ alljärgnevat

$$q = \frac{U_{max} - U_{min}}{2^{n_b}}$$

## Kvantimismüra
- Kvantimisega kaasneb alati **pöördumatu informatsioonikadu** mida iseloomustab **kvantimismüra** võimsusega 

$$N = \frac{q^2}{12}$$

![[Kanalikiht ja kanali kodeerimine/Pasted image 2.png]]

- Kvantimismüra on seda suurem mida vähem bitte samasse vahemikku jääva signaali väärtuse kirjeldamiseks kasutatakse

Ümardamisviga on seda suurem mida juurem on "joonlaua" jaotise suurus $q$

- Suur täpsus tähenda ka suurt ülekantavate bittide hulka, samas kui andmemahu vähendamisega suureneb ümardamisviga ja sellega ka signaali moonutuste määr $D$
- Signaal-kvantimismüra sute ligikaudne avaldis

$$SNR \approx 6 \cdot n_b + 4.7 dB$$