# Kontrollkood
## Leidmine
- Ülekantavad 9 bitti: `010100101`
- Kontrollimiseks neljabitist kontrollkoodi [[Genereeriv polünoom#Tsükliline liiasuse kontroll CRC -4|CRC-4]]
- Gen polünoom: `10011`
- Kontrollkood on alguses: `0000`
- Gen. polünoomi kõrgeim bitt asetatakse kohakuti kõrgeima mittenullise andmebitiga. 
- Edasised jagamistehted on asendatud mooduliga kaks summeerimisega
![[Modulatsioon/Pasted image 6.png]]
- Edastatav kaader koosneb edastatavatest andmetest ja neile lisatud kontrollkoodist 
- ![[Modulatsioon/Pasted image 7.png]]

## Kontrollimine
- Vastuvõtjas teostatakse sama operatsioon ja võrreldakse leitud kontrollkoodi ülekantuga. Kui need on omavahel võrdsed siis eeldatakse, et ülekandel vigu ei tekinud
- Alternatiiviks on kogu vastuvõetud kaadri (andmed  ja kontrollkood) genereeriva polünoomiga läbi jagamine, kui jäägiks on null, iis ülekanne toimus vigadeta, vastupidisel juhul on sõnumis viga
![[Modulatsioon/Pasted image 8.png]]