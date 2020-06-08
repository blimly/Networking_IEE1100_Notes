# Pseudojuhuslik binaarne jada
- Ühtede ja nullide järjestus mis statistiliselt analüüsides käitub sarnaselt juhuslikule (binaarsele) jadale
- Samas on sellise jada genereerimisprotsess **rangelt deterministlik**
	- Teades vajalike parameetreid on võimalik alati genereerida täpselt identne järjestus
- **Leiab rakendust** 
	- [[Sagedushüplemine|sagedushüplemise]] ja spektri otsese hajutamise juures
	- koodtihenduse teostamisel ([[CDMA]])
	- [[Skrämbler#Aditiivne skrämbler|aditiivsetes skrämblerites]]
	- radar- ja sonartehnikas 
	- ning paljudes muudes valdkondades

## Genereerimine
![[Traadita kohtvõrk ja hajaspektriside/Pasted image 7.png]]
- Tekitatakse tagasisidestatud nihkeregistriga
- Tagasiside võtmisega sobivatest kohtadest on võimalik genereerida maksimaalse pikkusega **m-jada**
- Kui tagasissidestatud nihkeregistri pikkus on $n_b$ bitti, siis m-jada pikkus on 

$$N=2^{n_b}-1$$

### Võimalikud tagasisidekohad m-jada jaoks
![[Traadita kohtvõrk ja hajaspektriside/Pasted image 9.png]]

- **Näide:**
	- $n = 3$
	- $N = 7$
	- Genereeriv polünoom: $g(x) = 1 + x^1 + x^3$
	- ![[Traadita kohtvõrk ja hajaspektriside/Pasted image 10.png]]
	- **M-jada ajaline kuju**
		- ![[Traadita kohtvõrk ja hajaspektriside/Pasted image 11.png]]
	- **M-jada spekter**
		- ![[Traadita kohtvõrk ja hajaspektriside/Pasted image 12.png]]
	- **M-jada autokorrelatsioonifunktsioon**
		- ![[Traadita kohtvõrk ja hajaspektriside/Pasted image 13.png]]