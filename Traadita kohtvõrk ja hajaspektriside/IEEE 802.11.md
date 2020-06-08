# IEEE 802.11
- IEEE 802.11-1997 (*Legacy Mode*)
- Töösagedus 2.4 GHz ISM riba (*Industrial, Scientific and Medical band*)
- Edastuskiirus 1 või 2 Mbitt/s
- Veaparandus konvolutsioonilise koodiga $k/n$
	- $k$ andmebitti iga edastava $n$ biti kohta
- Meediapöördus: CSMA/CA
	- IEEE 802.11 RTS/CTS
- Edastuseks kasutab kas 
	- Infrapunakiirgust IR
	- [[Sagedushüplemine|Sagedushüplemist]] (FH-SS)
	- [[Sageduse hajutamine|Sageduse (otsest) hajutamist]] (DS-SS)

## Sagedused ja võimsuspiirangud
- 2400 - 2483.5 MHz:	 EIRP $\leq$ 100 mW
- 5150 - 5350 MHz: 		EIRP $\leq$ 200 mW (ainult siseruumides)
- 5470 - 5725 MHz: EIRP $\leq$ 1 W
- **EIRP** - Ekvivalentne isotroopne kiirgusvõimus (*Effective Isotropic Radiated Power*)

$$EIRP = P_S \cdot G_S [W]$$

$$EIRP = P_S + G_S [dBm]$$

## 2.4 GHz kanalijaotus
![[Kärgvõrgud ja mobiilside/Pasted image.png]]

## Wi-Fi signaali [[Vaskkaabli parameetrid#Laine levimise kiirus|sumbuvus]]

- Vaba ruumi kadu

$$FSL = \left( \frac{4\pi d}{\lambda} \right)^2$$

- Vaba ruumi kadu (logaritmilistes ühikutes)

$$FSL = 20log(d) + 20log(f) - 147.55 [dB]$$
- Reaalsetes keskkondades on kauguse $d$ logaritmi kordaja  vahemikus 12 (koridorid) kuni 45 (ohtra mööbli, vaheseinade ja inimestega ruumid)

## IEEE 802.11b
- Edastuskiirus kuni 11 Mbit/s
	- 5.9 Mbit/s (TCP)
	- 7.1 Mbit/s (UDP)
- Töösagedus 2.4 GHz
- Hajutamine [[Barkeri koodid|Barkeri koodiga]] (CCK modulatsioon)
	- + Suurem edastuskiirus
	- - Vähenenud töökaugus ja häirekindlus

## IEEE 802.11a/g
- Andmeedastus 1.5 kuni 54 Mbit/s
- 2.4 GHz (g) ja 5 GHz (a) sagedusalad
- Modulatsiooniviisid: BPSK, QPSK, 16-QAM ja 64-QAM
- Kasutab [[Ortogonaalset sagedustihedust OFDM]] (*Orthogonal frequency-division multiplexin*)
	- 802.11a Kasutab 52 kandjat
		- 48 andmeside- ja 4 pilootkanalit
	- Teostatakse 64 punktilise diskreetse [[Signaali spekter#Fourier'i teisendus|Fourier'i teisenduse]] abil
		- $$X_k = \sum_{n=0}^{N-1}x_ne^{-\frac{j2\pi kn}{N}}$$
		- $$x_n=\frac{1}{N}\sum_{n=0}^{N-1}X_k e^{\frac{j2\pi kn}{N}}$$
	- Kanali samm 312.5 kHz
	- Sümboli kestus 3.2 $\mu s$
	- Sümbolite vahel 0.8 $\mu s$ paus (*Guard Interval*)
- **Spektrimask**
	- ![[Kärgvõrgud ja mobiilside/Pasted image 28.png]]
- ![[Kärgvõrgud ja mobiilside/Pasted image 29.png]]

## IEEE 802.11n
- Standard aastast 2009, seadmed tootmises juba 2007 aastast
- Töötab nii 2.4 kui 5 GHz sagedusalas
- Kanali ribalaius kas 20 või 40 MHz
- Sümbolite vaheline paus 0.4 $\mu s$ (*Guard Interval*)
- Andmeedastuskiirus 54-600 Mbit/s
- Kasutab andmeedastuskiiruse suurendamiseks mitut anteni ([[MIMO]])
- **Spekter**
	- ![[Kärgvõrgud ja mobiilside/Pasted image 30.png]]

## IEEE 802.11...
- **802.11ac**
	- Kanali ribalaius kuni 160MHz
	- Ühe kanali edastuskiirus 500Mbit/s
	- Kuni kaheksa MIMO kanali toetus
	- Kuni 256-QAM modulatsioon
- **802.11ad - WiGig**
	- Kuni 7Gbit/s 
	- 60GHz
- **802.11af - White-Fi**
	- 54-790MHz
	- TV sagedused, kognitiivne raadio

## IEEE 802.15.1 (Bluetooth)
- 1994 Ericson
- 2.4 GHz ISM-bänd
- [[Sagedushüplemine|Sagedushüpplus]] 79 kanali vahel
	- $B$ = 1MHz 
	- 800 hüpet sekundis
- Modulatsiooniviisid
	- Basic Rate (1 MBit/s): GFKS
	- Enhandced Data Rate (2 ja 3 Mbit/s): $\pi/4$-DQPSK, 8-DPSK
- Asendamaks ühendusjuhtmeid (RS-232)
- Väga väike töökaugus: 1-100m
- Väikesed kasutatavad võimsused -3 kuni 20dBm
- 1-25 Mbit/s