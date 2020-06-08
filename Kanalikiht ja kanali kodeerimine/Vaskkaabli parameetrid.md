# Vaskkaabli parameetrid
## Impedants
- Signaali energia kadudeta ülekandmiseks saatjast sidekanalisse ja sellest omakorda vastuvõtjasse peavad saatja väljundtakistus, kaabli lainetakistus ja vastuvõtja sisendtakisuts olema omavahel võrdsed
- Sellist ühtset takistust nimetatakse süsteemi **karakteristlikuks impedantsiks**
- Kui takistuste võrdsuse timgimus ei ole täidetud, siis tekivad üleminuekukohtadelt peegeldused mis häirivad või suisa takistavad sidesüsteemi tööd :(
- Peegelduste vältimiseks kasutatakse kaabli otste "lõpetamiseks" spetsiaalseid takisteid ehk **terminaatoreid**
- ![[Kanalikiht ja kanali kodeerimine/Pasted image 1 1.png]] der Terminator
## Laine levimise kiirus
- Vaakumis levivad elektromagnetlained valuse kiirusega $c= 299792458 m/s \approx 3 \cdot 10^8 m/s$
- Mistahes muus keskonnas liiguvad mainitud lained aeglasemalt. Valguse kiiruse vaakumis $c$ suhed valguse kiiruse $v$ mingis keskonas (nt. vees/klaasis) nimetatakse antud keskonna **murdumisnäitajaks** (*refractive index*)
	- $$n = \frac{c}{v}$$
- Vaskkaablis levib signaal enamasti umbes $2/3$ valguse kiirusest $c$. Signaali kaablis levimise kiiruse $v$ suhet valguse kiirusesse $c$ nimetatakse kaabli **kiirusteguriks** (*velocity factor*)
	- $$VF = \frac{v}{c}$$ 
## Sumbumus
- Mingi osa kaablis ülekantavast energisast läheb alati "kaduma" ehk muutub teisteks energialiikideks
- Seetõttu on kaabli väljundis signaali võimsus $P_v$ alati väiksem kui tema sisendis $P_s$. Nende kahe võimsuse suhet nimetatakse kaabli sumbuvuseks
	- $$L = \frac{P_s}{P_v}$$
- Kaabli sumbumus sõltub kaabli ehitusest (mõõtmed, kuju ja materjalid) ning signaali sagedusest $f$
- Tavaliselt väljendatakse sumbuvust [[Detsibell|detsibellides]] pikkusühiku kohta $[dB/m]$
	- $$L = 10 \cdot log \left( \frac{P_s}{P_v} \right)$$

## Ribalaius
- Sagedust $f_c$ mille juures on sidekanali ülekanne vähenenud pooleni algsest (-3dB) nimetatakse **lõikesageduseks**
- Kanali ülemise ja alumise lõikesageduse vahet nimetatakse kanali **ribalaiuseks** $B$
- Vaskkaabli sageduskarakteristik on üldjuhul nullist alates kahanev, seega on ribalaius $B$ ja lõikesagedus $f_c$ omavahel arvuliselt võrdsed
- Mida suurem on kaabli ribalaius, seda suuremat andmesidekiirust üle selle teosada saab. Vajadusel saab sagedustihedus [[Modulatsioon#Moduleerimise eesmärgid|FDMA]] kasutades jaotada kaabli ribalaiuse mitme kasutaja vahel.

## Läbikoste
- Kui ühes kaablis on koosm mitu juhtmepaari (keerdpaari), siis mingi väike osa ühes kaablis levivast signaalist kandub üle teise ja vastupidi. Sellist nähtust nimetatakse **läbikosteks** (*crosstalk*)
- Kui häirepinget $U_n$ mõõdetakse samast kaabli otsast kui testsignaali $U_s$ siis läbikoste **NEXT** (*Near-End Crosstalk*) väärtus on:

$$NEXT = -20 \cdot log\left(\frac{U_n}{U_s}\right)$$
![[Pasted image 3 1.png]]