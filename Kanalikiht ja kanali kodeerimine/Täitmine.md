
## Bititäitmine
- Kaadrid algust ja lõppu tähistatakse spetsiifilise lipuga
	- tihtipeale on väärtuseks `0x7E (01111110)`
- Juhul kui kaadri sees edastatavates admetes leidub sama bitijärjestus siis loeb vastuvõtja selle ekslikult kaadri lõpuks
- Lahenduseks on **bitiäitmine** (*bit stuffing*)
	- Iga viie järjestikuse "`1`" järel lisatakse "`0`" (*farssbitt*)
	- Vastuvõtjas eemaldatakse viiele järjestikusele ühele järgnev  "`0`" 
	- ![[Kanalikiht ja kanali kodeerimine/Pasted image 2.png]]

## Baiditäitmine
- Kui andmed edastatakse baidi kaupa on mõistlikum kasutada **baiditäitmise** (*byte stuffing*) nimelist tehnikat (*Control Octet Transparency*)
- [[Kaader|HDLC]] protokollis kasutatakse selleks spetsiaalset sümbolit `0x7D` (*Control escape octet*), mis asetatakse iga kaadri sees oleva `0x7E` või `0x7D` okteti ette. Lisaks inverteeritakse vastava okteti viies bitt.
	
![[Kanalikiht ja kanali kodeerimine/Pasted image 3.png]]








