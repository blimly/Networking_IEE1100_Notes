# Signaalide võrdlemine ja tuvastamine
- Sidetehnikas tekib tihti vajadus teadaoleva kujuga signaali $s(t)$ tuvastamiseks vastuvõetud realisatsiooni $y(t)$ seest
	- Otsustusseade peab näiteks suutma leida vastuvõetud realisatsioonist $y(t)$ nii ühtedele kui nullidele vastavaid signaalikujusid
- Teine praktkas lahendamist vajab probleem on mitme signaali summa seast ühe konkreetse signaali $s_i(t)$ eristamine
	- Leiab kasutamist **kooditiheduse** [[CDMA]] (*Code Division Multiple Access*) ressursijaotusmehhanismi käigus
	- CDMA-d kasutatakse näiteks 3G mobiilsides, [[GPS]] navigatsioonisüsteemis jne.
- Mõlema probleemi lahendamiseks kasutatakse **korrelatsiooni**


## Korrelatsioon
- **Ristkorrelatsioon** - signaalide $x(t)$ ja $y(t)$ vaheline sarnasus

$$R_{xy}(\tau) = \int_{-\infty}^{\infty} x^*(t)y(t+\tau) dt$$

- **Autokorrelatsioon** - signaali enesesarnasus

$$R_{x}(\tau) = \int_{-\infty}^{\infty} x^*(t)x(t+\tau) dt$$

- **Diskreetesl juhul** - enamasti on signaalid digitaalsel kujul: $s(n \cdot \Delta t) \equiv s[n]$

$$R_{xy}[n] = \sum_{m=-\infty}^{\infty} x^*[m]y[m+n]$$