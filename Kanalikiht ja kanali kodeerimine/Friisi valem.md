# Friisi valem
![[Pasted image 13 1.png]]
- Kõige lihtsam raadiokanali mudel
- On põhimõtteliseks aluseks kõikidele teistele, keerukamatele ja täpsematele mudelitele
- Praktikas kasutatava ainult teatud erijuhtudel
	- Kosmoseside
	- Side lähestikku asuvate lennuvahendite, või lennuvahendi ja maa vahel
- Saatja ja vastuvõtja asuvad tühjuses
	- Vaakum
	- Õhk madalatel sagedustel
- Läheduses ei ole takistusi, ega peegeldusi põhjustavaid objekte
- Eeldame, et puudvad igasugused täiendavad kaod
- **Ekvivalente isotroopne kiiruguvõimsus** (*Equivalent Isotropically Radiated Power*) [W]

$$EIRP = P_s \cdot G_s$$
- Võimsuse pindtihedus ehk Poyntingi vektor
	- $$\Pi = \frac{EIRP}{4 \pi d^2} =
	\frac{P_sG_s}{4 \pi d^2}$$
	- ![[Pasted image 14 1.png]]

- [[Raadiokanal#Antenn|Antenni]] võimenduse $G$ seos efektiivse pindalaga 

$$A_{eff} = \frac{\lambda^2}{4\pi} G$$

- Vastuvõtja sisendisse jõudva signaali võimsus on võimsuse pindtiheduse ja vastuvõtuantenni efektiivse pindala korrutis:

$$P_{Vv} = P_SG_SG_{Vv} \left( \frac{\lambda}{4\pi d}\right)^2$$
- **Vaba ruumi kadu** (*Free Space Loss*)

$$FSL = \left( \frac{4\pi d}{\lambda}\right)^2$$

### Tähised
- $P_{Vv}$ - vastuvõetud signaali võimsus [W]
- $P_S$ - saatevõimsus [W]
- $G_S$ - saateantenni võimendus
- $G_{Vv}$ - vastuvõtuantenni võimendus
- $\lambda$ - signaali lainepikkus [m]
- $d$ - saatja ja vastuvõtja vaheline kaugus [m]
- $L$ - muud kaod
- Võimendused ja kaod on **ühikuta suurused**, väljendatakse kordades

## Lingi bilanss
- Lingi bilanss on Friisi valem väljendatuna logritmilstes mõõtühikutes
- Võimsused [dBm], antennide võimendused [dBi] ja kaod [dB]

$$P_{Vv} = P_S + G_S + G_{Vv} - FSL - L$$
- Praktikas on vaba ruumi kao leidmiseks mugav kasutada järgmist kohandatud valemit

$$FSL = 20 \cdot log_{10}(d) + 20 \cdot log_{10}(f) + 32.45$$
- Saate- ja vastuvõetud signaali võimsused [dBm]
	- Mõnikord kasutatakse ka [dBW]
- Saate- ja vastuvõtuantenni võimendused [dBi]
	- Harva kasutatakse ka [dBd]
- Ekvivalentne isotroopne kiirgusvõimsus $EIRP = P_S + G_S$
- Vaba ruumi kadu [dB]

$$FSL = 20log \left( \frac{4\pi d}{\lambda} \right)$$

- Muud kaod sammuti [dB]

