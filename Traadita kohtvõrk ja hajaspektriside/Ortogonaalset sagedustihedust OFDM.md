# OFDM
- Mitmekiirelise levi tõttu tekkiv sümbolitevaheline interferents ISI piirab maksimaalset edastuskiirust $R$
- Üheks ISI vähendamise viisiks on sümbolikiiruse vähendamine. Sama bitikiiruse hoidmiseks on seega vaja tõsta kasutatavate sümbolite arvu $M$
- **Ortogonaalse sagedustihenduse** OFDM (*Orthogonal Frequency Division Multiplex*) korral jaotatakse andmevoog $N$, omavahel ortogonaalse, sageduskanali vahel
- Igas alamkanalis on bitikiirus nüüd $N$ korda väiksem
- Igas alamkanalis kasutatakse $M$ positsioonilist modulatsiooni, seega on sümbolikiirus summaarselt vähenendu $N \cdot M$ korda

![[Kärgvõrgud ja mobiilside/Pasted image 23.png]]
- Kui jaotame andmevoo $N$ kanali vahel, siis igaühes neist on edastuskiirus $R_N$ nüüd $N$ korda väiksem ja vastavalt on sama palju kordi väiksem ühe kanali ribalaius

$$B_{0N} = B_0/N$$
- Kanalid on omavahel ortogonaalsed, kui nenede kandesagedused $f_{cN}$ erinevad omavahel edastuskiiruse $R_N$ võrra

## OFDM spekter
![[Kärgvõrgud ja mobiilside/Pasted image 24.png]]

![[Kärgvõrgud ja mobiilside/Pasted image 25.png]]

![[Kärgvõrgud ja mobiilside/Pasted image 26.png]]

![[Kärgvõrgud ja mobiilside/Pasted image 27.png]]

## Digitaalslt moduleeritud signaali spekter
![[Kärgvõrgud ja mobiilside/Pasted image 22.png]]
- Digitaalselt moduleeritud signaali amplituudspekter on $sinc(x)$ [[Pingeimpulssi spekter|funktsiooni]] kujuline 
- Ribalaius $B_0$ on võrdne kahekordse sümbolikiirusega $R$

$$B_0 = 2R$$

---
- [[IEEE 802.11#IEEE 802 11a g|IEEE 802.11a OFDM]]