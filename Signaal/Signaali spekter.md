# Signaali spekter 

![[Pasted image 1 1.png]]

- Enamasti koosneb signaal $s(t)$ mitmest erineva sagedusega komponendist.
- Signaali **spekter** $S(f)$ on nende komponentide jaotus sageduse järgi.
- Signaali spektris oleva kõrgeima ja madalaima sageduse erinevust nimetatakse **ribalaiuseks**

$$B = f_{max}-f_{min}$$

![[Allika kodeerimine/Pasted image 2.png]]

## Fourieri rida - perioodilise signaali spekter
- Suvalist perioodilist signaali $s(t)$ perioodiga $T$ saab esitada spektrikomponentide kaudu

$$s(t) = \frac{A_0}{2} + \Sigma_{n=1}^{\infty} A_n sin(\frac{2 \pi n t}{T} + \phi_n)$$

-  $A_0$ - alaliskomponent ehk keskväärtus
- $A_n$ - n-inda spektrikomponendi amplituud
- $\phi_n$ - n-inda spektrikomponendi faas
- Perioodilise signaali spekter on diskreetne

### Fourier'i teisendus
*(Mitteperioodilise signaali s(t) korral)*

$$S(f) = \int_{-\infty}^{\infty} 
s(t) e^{-j 2 \pi f t} dt$$

$$s(t) = \frac{1}{2\pi} \int_{-\infty}^{\infty} 
S(f) e^{j 2 \pi f t}df$$