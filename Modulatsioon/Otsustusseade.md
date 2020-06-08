# Otsustusseade
![[Traadita kohtvõrk ja hajaspektriside/Pasted image 31.png]]
- Vastuvõetud müradega signaali $y(t)$ põhjal tuleb vastuvõtjas kindlaks teha, et millist sümbolit $a_i$ parasjagu edstati
- Sõlme, mis neid otsuseid teeb, nimetatakse **otsustusseadmeks**
- Kuna vastuvõetud signaal $y(t)$ on juhuslik, siis ei ole võimalik ühe konkreetse sümboli korral ette teada kas selle väärtus määratakse korrektselt kindlaks või tehakse viga
- Samas on võimalik statistiliselt analüüsida vea tegemisetõenäosust $P_s$ või katseliselt mõõta tekkinud vigade hulka ülekantud sümbolite hulga kohta
- Binaarsel edastusel ($M=2$) on vastavalt tegemist bitivea tõenäosusega $P_b$ ja bitivigde suhtega $BER$

## Mürade mõju bitivigade tekkele
![[Traadita kohtvõrk ja hajaspektriside/Pasted image 32.png]]
- Jaotustihedus $f(y)$ näitab kui suur on tõenäosus, et signaal $y(t)$ omab minit konkreetset väärtust
- Näiteks tõenäosus, et vastuvõetud pinge väärtus $y=2V$ on $0.1$
	- $f(2) = 0.1$
- Tinglik jaotustihedus $f(y|0)$ näitab tõenäosust, et signaal omab mingit konkreetset väärtust $y(t)$ eeldusel, et parasjagu edastatakse biti väärtust `0`
- $f(y|0)$ on vastuvõetud signaali jaotustihedus eeldusel, et edastatava biti väärtus on `1`

---
- [[Liinikoodi häirekindlus]]