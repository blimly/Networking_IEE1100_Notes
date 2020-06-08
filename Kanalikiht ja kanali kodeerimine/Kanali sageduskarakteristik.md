
# Kanali sageduskarakteristik
- Sidekanalis toimub harmoonilise signaaliga kaks muutust
	- Sumbumuse tõttu väheneb signaali amplituud
	- Lõpliku levikiiruse tõttu teikib ajaline viide $\tau$ kanali sisen- ja väljundsignaali vahel, mida väljendatakse enamasti **faasinihkena** $\Delta \phi$
- Kumbki muutus on üldjuhul sagedusest $f$ sõltuv
	- Amplituudi muutuse sõltuvust sagedusest nimetatakse süsteemi **amplituudsageduskarakteristikuks** $|H(f)|$ ehk sageduskarakteristiku mooduliks
	- Faasi muutust vastavalt **faasikarakteristikuks** $\phi_H(f)$
- Kokkuvõtlikult on tegemist sidekanali (süsteemi) sageduskarakteristikuga 

$$H(f) = |H(f)| \angle \phi_H(f) = |H(f)|e^{\phi_H(f)}$$

![[Pasted image 2 1.png]]

## Näide
- Sisendpinge: $u_s(t) = cos(20 \pi t)$
- Väljundpinge: $u_v(t) = 0.5cos(20\pi t - \frac{\pi}{4})$
- Signaali sagedus $f = 10Hz$
- Ülekanne $|H(10)| = 0.5 = -3dB$
- Faasinihe $\phi_H(f) = -\pi/4 = 45^{\circ}$

$$H(10) = 0.5e^{-\frac{\pi}{4}}$$