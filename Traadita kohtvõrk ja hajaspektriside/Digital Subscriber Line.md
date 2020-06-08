# DSL - Digital Subscriber Line
![[Kärgvõrgud ja mobiilside/Pasted image 32.png]]
- Digitaalne kasutajaliides - andmeedastus üle telefoniliini
	- "Viimane miil"
- Võimaldab andmesidet samaaegselt telefoniteenuse kasutamisega (FDM)
- Kasutatakse majanduslikel kaalutlustel - paljude kasutajateni on olemas analoogtelefoni ajastust pärinev kaabledus
	- Odavam kui fiiberoptilise kaabli paigaldamin
- Edastuskiirus 256 kbit/s kuni 100 Mbit/s
	- Laboritingimustes saavutatud 1 kuni 10Gbit/s

## ADSL
- Asümmeetriline DSL
- 1.104 MHz laiune sagedusriba jaotatud 256 kanaliks laiusega 4.3125 kHz
	- [[Ortogonaalset sagedustihedust OFDM|OFDM]]
	- Allalink 224 kanalit
	- Üleslink 25 kanalit
- Sõltuvalt [[Signaal müra suhe|SNR]] väärtusest kannab iga üksik kanal 1-15 bitti informatsiooni
	- Modulatsiooniviisid BPSK kuni 32768-QAM
- Sümbolikiirus 4000 baudi
	- Allalink: 224x15x4000 = 13.4 Mbit/s
	- Üleslüli: 24x15x4000 = 1.5 Mbit/s
- **Kanalid**
	- ![[Kärgvõrgud ja mobiilside/Pasted image 33.png]]
- **Ülesehitus**
	- ![[Pasted image 34.png]]