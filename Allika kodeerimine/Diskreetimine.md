# Diskreetimine
- Analoogsignaali fikseerimine ainult mingil lõplikul hulgal ajahetkedel $t = n \cdot \Delta t$
	- $n$ - suvaline täisarv
	- $\Delta t$ - **diskreetimissamm** ehk ajavahemik mille tagant mõõtmist teostatakse
- Diskreetimise tulemusena saama signaali $s(n\cdot \Delta t)$ mis on väärtuse poolest ikka pidev, kuid argumendi poolest **diskreetne** (väärtus on määratud ainult konkreetsel ajahetkel $n \cdot \Delta t$)

![[Pasted image 1 2.png]]

## Diskreetimissagedus
- Kui sageli tuleb analoogsignaali väärtust mõõta ehk milline peab olema diskreetimissammu $\Delta t$ väärtus
- Enamasti on kasutusel analoog-digitaalmuundust kirjeldades diskreetimissammu $\Delta t$ asemel selle pöördväärtus ehk **diskreetimissagedus** (*sampling frequency*)

$$f_s = \frac{1}{ \Delta t }$$

- Kui suur peab olema signaali diskreetimissagedus $f_s$?
	- [[Nyquisti kriteerium]]