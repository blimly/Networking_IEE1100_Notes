# Global Positioning System
- GPS satelliidid edastavad signaale kahel sagedusel
	- ==L1== 1.57542 GHz
	- ==L2== 1.2276 GHz
- Signaalide eristamine [[CDMA]] meetodil
- Moduleerimiseks kasutatakse Goldi koode
- Avaliku C/A koodi edastatakse kiirusega 1.023 miljonit sümbolit sekundis
- Täpset koodi $P$ edastatakse kiirusega 10.23 miljonit sümbolit sekundis
- Täpset koodi on võimalik krüteerida $P(Y)$

## Näide: GPS II
- Kanal ==L1== on moduleeritud C/A ja $P$ koodiga. Kanal ==L2== ainult $P$ koodiga
- Informatsiooni ülekandekiirus 50 bit/s
- Kasutatakse Goldi koode pikkusega 1023 elementi 1ms jooksul
- Võimalike Golid koode pikkusega 1023 on 1025, kasutatakse ainult 32 neist

## GPS signaali moduleerimine
![[Kärgvõrgud ja mobiilside/Pasted image 21.png]]