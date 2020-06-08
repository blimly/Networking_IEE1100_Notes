
# Nyquisti kriteerium
**Nyquist-Shannon-Kotelnikovi teoreem**
- Kui signaali $s(t)$ ribalaius on $B$ hertsi, siis on see signaal **täielikult määratud** diskreetse väljavõttega ajavahemike $\Delta t = 1/2B$ sekundi tagant
- Praktikas tuleb mõõta tihedamalt, ehk vajalik diskreetimissamm peab vastama nõuetele  $\Delta t \leq 1/2B$
- Teisisõnu, diskreetimissagedus peab olema vähemalt kaks korda suurem kui on diskreeditava signaali ribalaius
	
$$f_s \geq 2B$$
- Kui signaali diskreetimissammu valikul peetakse kinni Nyquisti kriteeriumist, siis diskreetimisega informatsioonikadu **ei kaasne** (moonutus $D = 0$)
- Paljud reaalsed signaalid on **[[Liinikoodi spekter|põhiriba signaalid]]** (*baseband*), ehk nende madalaim saedus $f_{min}$ on kas võrdne nulliga või väga lähedal nullile
- Selliste signaalide ribalaius $B$ on seega arvuliselt võrdne maksimaalse sagedusega signaalikomponendi omaga $f_{max}$
- Seetõttu kirjutatakse enamasit Nyquisti kriteerium kujul

$$f_s \geq 2f_{max}$$