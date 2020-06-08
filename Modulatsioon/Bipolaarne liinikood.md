# Bipolaarne liinikood
- Kui andmetele vastava signaalipinge väärtus võib olla nii positiivne kui negatiivne, siis nimetatakse liinikoodi **bipolaarseks**
- Enamasti vastab ühele biti väärtusele positiivne ($+U$) ja teisele sama suur negatiivne pingenivoo ($-U$)
	- Näiteks RS-232 liidese korral vastab biti väärtusele `1` **negatiivne** pinge vahemikus -3V kuni -15V ja biti väärtusle `0` **positiivne** nivoo vahemikus +3V kuni +15V

$$u(t) = 
  \begin{cases} 
   +U & \text{, kui } a_k = 0 \\
   -U & \text{, kui } a_k = 1
  \end{cases}
$$
- Selline vastavus on **bipolaarne NRZ liinikood**
- Bitijadale `01101` vastab liinikood:

![[Kanalikiht ja kanali kodeerimine/Pasted image 1 1.png]]

---
![[Pasted image 2 1.png]]