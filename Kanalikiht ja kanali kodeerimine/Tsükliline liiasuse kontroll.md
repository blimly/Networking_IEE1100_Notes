# Tsükliline liiasuse kontroll - CRC
- **CRC** (*Cyclic Redundancy Control*)
- Tõhusam kui kontrollsumma
- Selle järgi leitakse vigu tuvastav [[Kontrollkood|kontrollkood]] andmete spetsiaalse arvu **genereeriva polünoomiga $g(x)$** läbijagamise teel
- Meetod käsitleb ka edastatavaid andmeid polünoomina
- Kontrollkoodi pikkus on tavaliselt 4, 8, 16 või 32 bitti
	- enamasti 8 või 16
### Kahendarvu esitamine [[Genereeriv polünoom|polünoomina]]
- Võimaldab pikki kahendarve lühemalt kirja panna
- Kirjapilt kujutab kogu arvu asemel ainult ühtede asukohti
	- Kahendarvu `10100101` on polünoomina $x^7 + x^5 + x^2 + 1$