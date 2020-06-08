# Ülekandemeedium
- Informatsiooni edastavad signaalid $s(t)$ kantakse saatjast vastuvõtjasse **ülekandemeediumi** vahendusel
- **Suunatud meediumites** (*guided medium*) on **vaskkaabel** ja **fiiberoptiline kaabel**. Mõlema kaudu levib signaal ainult kaabli suunas. Kaablis on signaali kaod väikesed, madala võimsusega signaalid võivad levida sadade ja tuhandate kilomeetrite kaugusele
- **Suunamata meediumi** (*unguided medium*) all peetakse silmas raadiokanalit ja vähesel määral kasutatavat optilist sidet vabs ruumis. Sellise sidekanali korral ei ole vaja saatja ja vastuvõtja vahele kaabeldust vedada, terminalid saavad ruumis vabalt paikneda ja ringi liikuda

## Keerdpaar
- Lihtsaim, odavam ja seega laialt levinud ülekandemeedium
- Ehituselt koosneb kahest, ümber ühise telje spiraalselt keeratud, vaskjuhtmes. Sellest ka nimetus **keerdpaar** (*twisted pair*)
- Tavaliselt on ühes kaablis koos mitu keerdpaari. Tavalise Etherneti juhtme korral neli keerdpaari
- Keerdpaarkaableid jaotatakse vastavalt kvaliteedile ja kasutusvaldkonnale erinevateesse kategooriatesse (CAT3 kuni CAT7)
- Tavaliselt on keerdpaarkaabel ilma varjesuseta (UTP -*Unshielded Twisted Pair*). Suuremat häirekindlust tagavad varjestatud kaablid (STP - *Shielded Twisted Pair*)

## Keerdpaari impedants
- Keerdpaari **impedants** ehk **lainetakistus** sõltub peamiselt kasutatavate juhtmete läbimõõdust ja nende vahekaugusest 

$$Z_0 = \frac{276}{\sqrt{\varepsilon_r}} 
log \frac{d}{r}
$$
- Impedantsi mõõtühikuks on oom $[\Omega]$
- Ethernetikaablite impedants on $100 \pm 15 \Omega$

## Koaksiaalkaabel
![[Kanalikiht ja kanali kodeerimine/Pasted image 23.png]]
- Teiseks levinud vaskkaabli tüübiks on **koaksiaalkaabel** (*Coaxial cable*)
- Ehituselt on tegemist kahe, erineva läbimõõduga, silindrilise juhtmega, millest üks asub teise sees
- Koaksiaalkaabel töötab kõrgematel sagedustel ja on suurema ribalaiusega kui keerdpaar, kuid samas on ta kallim ja suuremate mõõtmetega
- Karakteristlik impedant on tüüpiliselt $50\Omega$, televisioonitehnikas on $75\Omega$, ning on kaabli mõõtudest leitav järgmiselt 

$$Z_0 = \frac{138}{\sqrt{\varepsilon_r}} 
log \frac{d_1}{d_2}
$$

---
- [[Kanali sageduskarakteristik]]
- [[Vaskkaabli parameetrid]]
- [[Raadiokanal]]