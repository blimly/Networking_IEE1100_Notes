# M-positsioonilised liinikoodid
- Digitaalne andmeedastus ei pea olema ilmtingimata binaarne
- $M$ - erinevat sümbolit $a_k$ kasutades saab ühe sümboliga edastada $I = log_2(M)$ bitti informatsiooni
- Tavaliselt valitakse $M$ väärtuseks mõni kahe täisarvulise aste (nt. 4, 8, 16). Sellisel juhul edastatakse ühe sümboliga täisarv bitte
	- Erinevad Etherneti standardid kasutavad andmete edastamisel näiteks $M=3;4;5 \text{ või } 16$ erinevat sümbolit
- Miteme sümboli kasutamine tähendab, et sama kestuse ja sama sagedusriba juures on võimalik edastada rohkem informatsiooni. Seega võidame [[Shannoni valem|spektraalefektiivsuses]] ($C/B$)
- Samas on vastuvõtjal raskem vastuvõetud sümboleid teineteisest eristada, vigadeta otsuste tegemiseks on vajalik suurem signaal-müra suhe. 
	- Hinda tuleb maksta vähenenud veakindluse ja sidekaugusega

## 4-PAM liinikood
- Edastavate sümbolite arv $M=4$

![[Pasted image 13 1.png]]
- Erinevatele sümboli väärtustele vastab erinev pingeimpulssi amplituud, seega kutsutakse sellist liinikoodi **Impulssapmlituudmoduleerituks** ehk **PAM** (*Pulse Amplitude Modulation*). Arv liinikoodi või modulatsiooniviisi ees tähistab kasutavate sümbolite arvu $M$
- Näide 
	- ![[Pasted image 14 1.png]]
	- Edastatavad sümbolid: $a_3, a_1, a_0, a_2, a_2$
	- Edastatavad bitid: `11 01 00 10 10`
	- Biti kestus $T_b$ on siin poole väiksem sümbolit omast $T_s$