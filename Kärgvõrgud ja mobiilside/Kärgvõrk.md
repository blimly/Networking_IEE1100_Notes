# Mobiilside kärgvõrk
- Praktikas kaetakse territoorium tugijaamade võrgustikuga
- Ühe tugijaama leviulatus jääb, sõltuvalt mobiilside põlvkonnast ja kasutajate paiknemise tihedusest, vahemiku mõnesajast meetrist kuni mõnekümne kilomeetrini
- Ideaalsel juhul on ühe tugijaama leviala ringikujuline, reaalsel maastikul on leviala kuju ebakorrapärane
- [[Mobiilsidevõrk|Mobiilsidevõrgu]] mudelis eeldatakse enamasti, et kõikide tugijaamade levialad on korrapärase kuusnurga (meekärje) kujulised. Sellest ka nimetus **kärgvõrk** (*Cellular Network*)
	- Naaberkärgede vaheline kaugus: $d=\sqrt{3}R$
	- ![[Pasted image 4.png]]

## Sageduste taaskasutus 
- Ideaalsel juhul kasutataks kõikides kärgedes side pidamiseks unikaalseid sagedusi
- Praktikas on kasutatavate sageduste arv piiratud
	- Sagedusriba on iseenesest piiratud ressurss
	- Viimast peab veel jagama erinevate teenusepakkujate vahel
	- Seadmete ribalaius on reaalselt piiratud
- Seetõttu tuleb olemasolevad kanaleid korduvalt kasutada (*frequency reuse*). Interferentsi vähendamiseks üritatakse samu sagedusi kasutatavad tugijaamad paigutada teineteistest võimalikult kaugele
- ![[Pasted image 5.png]]
- Sageduste taaskasutustegur: $N = I^2 + J^2 + IJ$
- Kus $I$ ja $J$ on naturaalarvud
- Võimalikud $N$ väärtused: `1, 3, 4, 7, 9, 12, 13, 16, 19, 21,...`
- Minimaalne kaugus $D$ kahe, sama sagedusi kasutava kärje vahel: $D=\sqrt{3N}R$

## Kärgede jaotamine
![[Pasted image 6.png]]
- Maktrokärg: 1-30 km
- Väike makrokärg: kuni 3 km
- Mikrokärg: kuni 1 km
- Pikokärg: kuni 500 m


