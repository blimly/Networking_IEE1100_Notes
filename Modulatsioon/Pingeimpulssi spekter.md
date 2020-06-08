# Pingeimpulssi spekter
- Sidetehnikas huvitab meid signaali ribalaius $B$
	- Kui lai on meie digitaalse signaali $u(t)$ spekter?
	- Kui suure ribalaiusega kanalit on vaja sellise signaali edastamiseks?
- Üksikule sümbolile $a_k$ vastav pingeimpulss
	- ![[Modulatsioon/Pasted image 3.png]]
- Mitteperioodilise signaali spektri $S(f)$ sai leida tema ajalisest kujust $s(t)$ [[Signaali spekter#Fourier'i teisendus|Fourieri tesenduse]] abil. Meie pingeimpulssi $u(t)$ spekter oleks seega:
![[Pasted image 14 1.png]]
$$U(f) = \int_{-\infty}^{\infty} u(t)e^{-j2 \pi f t} dt$$
- Tulemus on amplituudspekter $[V/Hz]$ kujul:

$$U(f) = UT_b sinc(T_bf)$$
- Funktsioon $sinc(x)$ on normeeritud $sin(x)/x$ funktsioon:

$$sinc(x) = \frac{sin(\pi x)}{\pi x}$$

![[Pasted image 4 1.png]]
*joonis on normeeritud kujul*
- Spekter on lõputult lai: $B = \infty$
- Nullkohad on edastuskiiruse $R = \frac{1}{T_b}$ täisarvkordsed
- Aplituudi ühikuks on $[V/Hz]$
- Maksimum on võrdne impulssi pindalaga $U\cdot T_b$ ja seega võrdeline biti energiaga: $E_b = U^2 T_b$