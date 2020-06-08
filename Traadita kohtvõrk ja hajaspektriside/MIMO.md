# Multiple Input Multiple Output
- Andmeedastuse kiiruse või töökindluse suurendamiseks 
- Mitme andtenni kasutamine nii saatjas, kui vastuvõtjas
- Signaalitöötlus lähtuvalt kanali olekuinfost 
	- **CSI** (*Channel State Information*)
- Suunadiagrammi formuleerimine
- Ruumiline multipleksimine (*Spatial multiplexing*) 
	- Mitu aeglast kanalit
- Ruumiline kodeerimine (*Diversity Coding*)
- **SDMA** (*Space Division Multiple Access*)
- MIMO süsteemis on vähemalt kaks saate- ja kaks vastuvõtuantenni
	- Massivne MIMO 5G mobiilside võrkudes kasutab kuni 128 antenni
- Saateantennide arv $N$ peab olema väiksem või võrdne, kui vastuvõtuantennide oma $M$
	- $$N \leq M$$
- Kokku on MIMO süsteemis $N \cdot M$ erinevat leviteed, igaühte neist saab kirjeldada impulsskajaga $h_{mn}$
- Informatsiooni kõigi nende impulsskajde kohta nimetatakse kanali olekuinformatsiooniks **CSI**. Tavaliselt esitatakse kanali olekuinformatsioon ülekandemaatriksi $\mathbf{H}$ kujul

# 2x2 MIMO
![[Kärgvõrgud ja mobiilside/Pasted image 31.png]]
- Lihtsaimal juhul $N=M=2$
- Signaalid vastuvõtja sisendites
	- $$\begin{cases} 
	y_1 = h_{11}x_1+ h_{12}x_2 \\
	y_2 = h_{21}x_1+ h_{22}x_2
	\end{cases}$$
	- Maatriksi kujul: $\vec{y} = \mathbf{H}\vec{x}$ kus:
		- $\vec{y} = \begin{bmatrix} y_1 \\ y_2 \end{bmatrix}$
		- $\vec{x} = \begin{bmatrix} x_1 \\ x_2 \end{bmatrix}$
		- $\mathbf{H} = \begin{bmatrix} h_{11} & h_{12} \\ h_{21} & h_{22} \end{bmatrix}$
- Kui CSI on teada, saab vastuvõtjas saadetud signaalid teineteisest eristada
	- $\vec{x}=\mathbf{H}^{-1}\vec{y}$
	- Kus $\mathbf{H}^{-1}$ on ülekandemaatriksi pöördmaatrix. 2x2 matriksi korral:
		- $$\mathbf{H}^{-1} = \frac{1}{h_{11}h_{22}-h_{12}h_{21}} \begin{bmatrix} h_{22} & -h_{12} \\ -h_{21} & h_{11} \end{bmatrix}$$
- Olekumaatriksit saab hinnata edastades teadaoleva kujuga pilootsignaali
