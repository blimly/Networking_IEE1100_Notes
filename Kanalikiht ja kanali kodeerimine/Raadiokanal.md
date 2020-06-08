# Raadiokanal 
![[Pasted image 11 1.png]]
## Antenn
- Seade mis muundab vaelduva elektrivoolu energia elektromagnetkiirguse omaks ja vastupidi
- Antenn soboitab omavahel raadioseadme ja -eetri
- **Antenni parameetrid:**
	- Võimendus $G [dBi]$
		- $$G = 10 \cdot log_{10} \left( \frac{P_{max}}{P_{Iso}} \right)$$
	- Impedants $Z_a$
	- Töösagedused $f_{min}..f_{max}$ (ribalaius $B$)
	- Suunadiagramm $D(\theta, \phi)$
		- ![[Pasted image 12 1.png]]

## Mitmekiireline levi
![[Pasted image 16 1.png]]
- Tavaliselt on saatja ja vastuvõtja vahel mitu erinevat võimaliku leviteekonda. Tagajärjeks ongi signaali saabumine vastuvõtjasse mitme koopiana ehk **mitmekiireline levi**
- Mitmekiireline levi põhjustab
	- Signaalitugevuse juhuslikku kõikumist ehk **feedinguid** (*fading*)
	- **Sümbolitevahelist interferentsi** ISI (*Inter- Symbol Interference*)
- Peamised vastumeetmed on
	- Pauside (*Guard Interval*) jätmine sümbolite vahele
	- **Ekvaliseri** (*equalizer*) kasutamine
	- Sümbolikiiruse vähendamine sümbolite arvu $M$ suurendamine teel (OFDM)
- Üldjuhul on signaali $N$ võimaliku leviteed
- ![[Pasted image 17 1.png]]
- Igaühe ülekanne $H_i$ on pöördvõrdeline levitee pikkusega
	- $L_i \sim d_i^{-n}$
	- astendaja $n$ on sõltuvalt levikeskkonnast vahemikus $1..4$
- Levitee viide $\tau_i$ on samuti võrdeline levitee pikkusega $d_i$
	- $$\tau_i=\frac{d_i}{v}$$
- Vastuvõtja sisendis olev realisatsioon on summa kanalis lisandunud müradest $n(t)$ ja mitut leviteed pidi saabunud signaalist $s(t)$

$$y(t) = \sum_{i=1}{N}H_i \cdot s(t- \tau_i) + n(t)$$
![[Pasted image 18 1.png]]

---
- [[Friisi valem]]
- [[Fresneli tsoon]]