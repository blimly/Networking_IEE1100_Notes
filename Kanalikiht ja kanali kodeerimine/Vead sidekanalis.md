# Vead sidekanalis
- Digitaalse andmeedastuse korral peab vastuvõtja temasse jõudnud signaali ja mõra summa $y(t) = s(t) + n(t)$ põhjal otsustama, millist sümbolit parasjagu edastatakse
- Sidekanalis levides signaal nõrgeneb ja tihtipeale ka moonutub
- Moonutuste ja mürade tõttue teeb vastuvõtja mõnikord **eksliku otsuse** vastuvõetud sümboli väärtuse kohta
- Kui tegemist on binaarse edastusega ($M=2$), siis nimetatakse sellist ekslikut otsust **bitibveaks**

## Bitivead
- Digitaalse edastuse kvaliteedi n'itajana kasutatakse **bitivigade suhet**: BER (*Bit Error Rate*)
- BER näitab kui suur osa edastatud $n$ bitist võeti vastu vigaselt 

- $$BER = \frac{n_e}{n}$$
	- $n_e$ - vigaselt vastuvõetud bittide arv
- Bitivigade suhe on pöördvõrdeline [[Signaal müra suhe|signaal-müra suhtega]] vastuvõtja sisendis. Ehk mida tugevam on signaal võrreldes müradega, seda harvemini tehakse ekslike otsuseid