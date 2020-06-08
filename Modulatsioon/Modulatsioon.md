
# Modulatsioon
![[Pasted image 15 1.png]]

- Liinikood on sobiv andmete edastamiseks seadme siseselt või kahe, omavahel otse juhtmetega kokku ühendatud seadmete vahel.
- Põhiribasignaalid ei sobi kasutamiseks fiiberoptilistes kaablites ega raadiokanalis. Samuti ei toeta paljud sidevõrgud nende ülekannet
- Protsess nimega **modulatsioon** võimaldab edastatavatele sümbolitele vastavad signaalid viia sidekanali jaoks sobivale kujule
- **Modulatsioon** - informatsiooni edastamiseks kasutatava füüsikalise nähtuse (elektrivool, elektromagnetväli jne.) mingi parameetri muutmine vastavalt ülekantava signaali muutustele
- Modulatsioon raadio- ja sidetehnikas on kõrgsagedusliku elektrivõnkumise (kandesignaali $s_c(t)$) või impulsijada minig parameetri muutmine tunduvalt madalama sagedusega moduleeriva signaali $m(t)$ rütmis
- Modulatsiooniga kaasneb signaali $m(t)$ esialgse kuju oluline muutus ja tema spektri üleminek teisele (kande) sagedusele
### Kandesignaal
- Kandesignaal $s_c(t)$ on tavaliselt harmooniline signaal kujul

$$s_c(t) = A \cdot cos(2 \pi f_c t + \phi)$$
- Modulatsiooni käigus saab mõjutada ühe või mitut kandesignaali parameetrit
	- Amplituudi $A$
	- Sagdust $f$
	- Algfaasi $\phi$

![[Pasted image 17 1.png]]


## Modulaator
![[Pasted image 16 1.png]]
- Seadet mis modulatsiooni teostab nimetatakse **moudulaatoriks** ja signaalide esialgse kuju taastamiseks vastuvõtjas kasutatakse **demodulaatorit**
- Enamsati tostab mõlemat operatsiooni **modem**

## Moduleerimise eesmärgid
- Võimaldab edastada signaali $m(t)$ kanalis mille sagedusomadused on piiratud
- Võimaldab vähendada edastatava signaali $m(t)$ kuju või mõne tema olulise parameetri moonutuse edastusel
- Võimaldab mitme signaali samaaegset edastamist ühes kanalis: **sagedustihendus** FDMA (*Frequency Division Multiple Access*)

## Sagedustihendus (FDMA)
![[Traadita kohtvõrk ja hajaspektriside/Pasted image 21.png]]
- Kanali sagedusriba efektiivne kasutamine
- Mitme signaali samaaegne edastamine ühes kanalis
![[Traadita kohtvõrk ja hajaspektriside/Pasted image 22.png]]

## Modulatsiooniviisid
- Vastavalt mõjutatavale kandesignaali parameetrile eristatakse 
	- [[Amplituudmodulatsioon]] AM, ASK
	- [[Sagedusmodulatsioon]] FM, FSK
	- [[Faasmodulatsioon]] PM, PSK
	- Kvadratuurne amplituudmodulatsioon QAM.
		- Muudetakse samaaegselt kandesignaali kui ka algfaasi
- Kui moduleeriv signaal $m(t)$ on pidev, on tegmist **analoogmodulatsiooniga**, kui tal on aga lõplik arv $M$ väärtuseid, siis räägime **[[Digitaalmodulatsioon|digitaalmodulatsioonist]]** ehk **manipulatsioonist**

---
- [[Konstellatsioonidiagramm]]