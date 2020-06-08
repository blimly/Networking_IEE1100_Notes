# Faasmanipulatsioon
- Üheks enamlevinumaks digitaalseks modulatsiooniviisiks andmeedastusel on faasmanipulatsioon **PSK** (*Phase Shift Keying*)

## BPSK
- Kõige lihtsamal binaarsel juhul **BPSK** (*Binary-PSK*), vastab bittide väärtustele kaks erinevat kanesignaali algfaasi väärtus $\phi$:

$$s_{BPSK}(t) =
  \begin{cases} 
   A \cdot cos(2 \pi f_c t) & \text{, kui } a_k = 1 \\
   A \cdot cos(2 \pi f_c t + \pi) &\text{, kui } a_k = 0
  \end{cases}
$$

- BPSK teostamiseks korrutatakse kandesignaal $s_c(t)$ lihtsalt läbi NRZ formaadis moduleeriva signaaliga $M(t)$

$$s_{BPSK} = s_c(t) \cdot m(t)$$

![[Traadita kohtvõrk ja hajaspektriside/Pasted image 26.png]]

$$s_{BPSK} = 
\begin{cases}
A \cdot cos(2 \pi f_c t) & \text{, kui } a_k = 1 \\
   -A \cdot cos(2 \pi f_c t) &\text{, kui } a_k = 0
\end{cases}
$$
![[Traadita kohtvõrk ja hajaspektriside/Pasted image 27.png]]
