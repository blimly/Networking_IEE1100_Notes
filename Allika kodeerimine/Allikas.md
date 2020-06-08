
# Allikas
Sidesüsteemi üleksntava info tekkekoht
- looduslikud / tehislikud
- analoogsed / digitaalsed

### Näited
- Kõnesignaali allikas on inimese kõnetrakt (häälepaelad, kõri, suu), elektriliseks analoogsignaaliks muundab tekitatud heli mikrofon.
- Kujutissignaali allikas on kaamera, mis muudab valgustundlikule sensorvõrele langeva valguse elektriliseks signaaliks. 
- Allikas võib olla näiteks fail mistahes andmetega mida soovitakse side-süsteemi vahendusel edastada, näiteks tekst, kujutis, heli, programmi kood jne.

## Allika mudel
Sidesüsteemi ehitamiseks või olemasoleva süsteemi sobilikuse hindamiseks on vaja teada milliste allikate signaali on vaja üle kanda ja milline on nende allikate käitumine. 

Allika käitumiset ja selle parameetreid kirjeldatakse **allika mudeliga**

Allika mudeleid on väga palju mis erinevad üksteisest nii detailsuse kui ka keerukuse poolest. Mida detailsem mudel, seda paremini kirjeldab ta reaalset allikat ning seda täpsemad on hinnangud sidesüsteemi nõuetele. Kuid detailsemat mudelit on keerukam kirjeldada ja analüüsida. 

## Mäluta diskreetne allikas
- väljunis võib olla ainult lõplik hulk $N$ sümbolit $a_j$
- kõiki võimalike sümboleid nimetatakse **allika tähestikuks** $A=\{a_j\}$
- lihtsaim diskreetne allikas on **binaarne allikas**, mille väljunis on igal ajahetkel kas $0$ või $1$
- binaarse allika tähestik: $A=\{0;1\}$

- Mäluta allika puhul ei sõltu iga järgneva allika sümboli $a_j$ esinemise tõenäosus $p(a_j)$ talle eelnenud sümbolite hulgast või väärtustest (allika sümbolid on üksteisest sõltumatud)
- Kõikide sümbolite esinemise tõenäosused võivad olla võrdsed (nt. kull/kiri või täringu silmade arv)
- Aga enamasti on nad erinevad

## Allika entroopia
- Kui allika sümbolite esinemise tõenäosused on erinevad, siis saab seda
allikat iseloomustada Shannoni entroopiaga ehk antud informatsiooniallika poolt toodetava informatsiooni (üllatuse) keskmise hulgaga:

$$H(A) = \sum_{j=1}^N p(a_j)I(a_j) = -\sum_{j=1}^N p(a_j)log_2 p(a_j)$$

- kui kasutatava logaritmi aluseks on 2 siis on entroopia mõõtühikuteks bitt.

![[Allika kodeerimine/Pasted image 1.png]]
*(binaarse allika entroopia)*
