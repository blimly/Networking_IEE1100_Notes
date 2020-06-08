# Vaheldamine
(*Interleaving*)
- Vigu parandavad koodid suudavad edukalt parandada suhteliselt suurt hulka vigu, eeldusel, et vead on vastuvõetud andmetes ühtlaselt jaotunud
- Praktikas kipuvad vead esinema suuremate gruppide ehk pursetena (*error burst*)
- Vaheldi (*Interleaver*) on seade mis vähendab veapursete mõju ja parandab seega vigu parandavate koodide kasutamise tõhusust. 
- Eemärk saavutatakse muutes enne saatmist eandmete järjekorda selliselt, et järjestiku eksisteerivad andmed ei paikneks edastamisel lähestiku
- Selle teostamiseks on mitmeid erinevaid viise.

## Block interleaver
- Olgu edastatavaks sõnumiks järgnev tekst
	- ==SeeOnVaheldamiseNäide==
- Peale veapurset on vastuvõetud andmetest kadunud neli järjestikust sümbolit
	- ==SeeO____eldamiseNäide==
- Edastatavad andmed kirjutatakse ridahaaval $n \times m$ tabelisse
![[Modulatsioon/Pasted image 16.png]]
- Andmed edastatakse sideliinis veergude kaupa
- ![[Modulatsioon/Pasted image 17.png]]
- Kõrvutised sümbolid ei paikne edastamisel koos
- Edastamisel tekib viide, mis on tingitud tabeli kirjutamisest enne edastamise algust ja lugemisest peale vastuvõtu lõppu
- Kui nüüd kustub edastatud jadas veapurske tõttu neli järjestikust sümbolit on tulemus järgmine 
- ![[Modulatsioon/Pasted image 18.png]]
- Vastuvõtjas on täidetud tabel kujul 
- ![[Modulatsioon/Pasted image 19.png]]
- Pärast sümbolite õige järjekorra taastamist on veapurse jaotunud ühtlasemalt sõnumi peale laiali
- ![[Modulatsioon/Pasted image 20.png]]