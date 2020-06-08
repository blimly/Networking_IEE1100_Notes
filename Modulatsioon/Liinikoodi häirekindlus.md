# Liinikoodi häirekindlus
- [[Unipolaarne NRZ liinikood|Unipolaarse liinikoodi]] korral, kus ühele sümbolile vastab pingenivoo $+U$ ja teisele $0V$ on bitivea tõenäosus AWGN mudeli korral 
- $$P_b = 
Q \left( \frac{U}{2 \sigma} \right) = 
Q \left( \frac{1}{2} \sqrt{ \frac{S}{N}}\right)
$$
	- $\sigma$ on mürapinge efektiivväärtus (võrdne mürapinge jaotuse standardhälbega)

![[Traadita kohtvõrk ja hajaspektriside/Pasted image 33.png]]
Näites, kus signaal müra suhe oli $SNR=10dB$ on bitivea tõenäosus $P_b \approx 0.05688..$ ehk umbes $5.7\%$


- $Q$-funktsioon on defineeritud kui (normaaljaotuse "saba"):
	
$$Q(x) = \frac{1}{\sqrt{2 \pi}} \int_x^{\infty} e^{- \frac{u^2}{2}}du$$
![[Pasted image 38.png]]

## $E_b/\eta$
- Sidesüsteemi olilisimaid näitajaid on [[Signaal müra suhe|signaal müra suhe]] $S/N$
- Sellest sõltub omakorda bitivigade suhe $BER$
- Digitaalsete sidesüsteemide puhul kasutatakse signaal-müra suhte asemel sellega võrdelist suurust: biti energia $E_b [J]$ suhet valge müra võimsuse spektraaltihedusse $\eta [W/Hz]$

$$\frac{E_b}{\eta}$$

- Suurus on seotud signaal-müra suhtega spektraalefektiivsuse $\rho [bitt/s/Hz]$ kaudu

$$\frac{S}{N} = 
\frac{E_b}{\eta} \cdot \rho = 
\frac{E_b}{\eta} \frac{R}{B}$$

## Modulatsiooniviiside häirekindlus
- bitivea tõenäosus binaarse [[Faasmodulatsioon|faasimanipulatsiooni]] BPSM korral
	- Koherentsel demoduleerimisel (algfaas teada):

$$P_b = Q \left( \sqrt{\frac{2E_b}{\eta}} \right)$$
- Mittekoherentsel demoduleerimisel

$$P_b = \frac{1}{2}e^{-\frac{E_b}{\eta}}$$

#### Modulatsiooniviiside võrdlus häirekindluse järgi
![[Traadita kohtvõrk ja hajaspektriside/Pasted image 34.png]]