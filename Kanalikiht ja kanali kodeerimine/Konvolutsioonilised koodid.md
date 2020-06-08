# Konvolutsioonilised koodid
- Moodustavad lisaks plokk-koodidele teise suure koodide klassi
- Pikkus pole fikseeritud
- Kodeerimine reaalajas 
- Ei ole vaja oodata, kuni teatud arv (plokk) sümboleid koodrisse sabub
- Väljund sõltub eelmistest sümbolitest - **mäluga kood**
 ![[Traadita kohtvõrk ja hajaspektriside/Pasted image 14.png]]

- Paarsusbittide väärtused: 

- $$p_i[n] = \left( \sum_{j=0}^{K-1}g_i[n]d[n-j] \right) mod(2)$$
	- $K$ on koodri pikkus (*constraint*)
	- $g_j$ on [[Genereeriv polünoom|genereeriv polünoom]]	]]
		- $g_0 = (1,1,1), \qquad g_1 = (1,1,0)$
		- $g_0 = x^2+x+1, \quad g_1 = x^2 + x$
- Koodi kiirus $R = 1/m$, kus $m$ on summaatorite arv
![[Modulatsioon/Pasted image 15.png]]
