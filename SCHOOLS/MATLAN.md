## Determinan Matriks
October 11th 2024

```JSON
// ORDO 2x2
A = 
[ 1  2 ]
[ 3  4 ]

D = | 1  2 | = (1x4) - (2x3) = 4 - 6 = -2 //
	| 3  4 |

	^
  perkalian silang 1,1 dengan 2,2 dan 1,2 dengan 2,1

---

2x - y  = 8
 x + 3y = -10

D = | 2 -1 |
	| 1  3 |
  = 6 -(-1)
  = 7

Dx = | 8   -1 |
	 | -10  3 |
   = 24 - 10
   = 14
   
Dy = | 2  8  |
	 | 1 -10 |
   = -20 - 8
   = -28

x = Dx / D = 14 / 7  = 2
y = Dy / D = -28 / 7 = -4
   
```

### Sifat determinan matrix

```JSON
|A||B| = |AB|
```

## Matriks identitas

```JSON
Matriks I = [ 1 0 ]
			[ 0 1 ]
```

## Inverse Matrix

Inverse matrix di notasi kan dengan petik `-1`. 
Contoh `A = [...]`, inverse nya adalah `A^-1 = [...]`

#### Rumus
```JSON
A^-1 =  1  [       ]
	   --- [ Adj.A ]
	   |A| [       ]
```

> PAPAN TULIS
![[WhatsApp Image 2024-10-11 at 09.29.26_8cb3665e.jpg]]

---

# Matriks Invers

## 1. Definisi
Matriks invers dari matriks $A$ adalah matriks lain, dilambangkan sebagai $A^{-1}$, sehingga ketika dikalikan dengan $A$, menghasilkan matriks identitas $I$:
$$
A A^{-1} = A^{-1} A = I
$$

## 2. Matriks Identitas
Matriks identitas $I$ adalah matriks persegi dengan satu di diagonal dan nol di tempat lainnya. Contoh matriks identitas ukuran 2 adalah:
$$
I = \begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
$$

## 3. Syarat untuk Inversibilitas
Tidak semua matriks memiliki invers. Matriks $A$ dapat dibalik (atau non-singular) jika:
- $A$ adalah matriks persegi (jumlah baris sama dengan jumlah kolom).
- Determinan dari $A$ tidak nol: $\text{det}(A) \neq 0$.

## 4. Mencari Invers
Untuk menemukan invers dari matriks $2 \times 2$:
$$
A = \begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
$$
Inversnya diberikan oleh:
$$
A^{-1} = \frac{1}{ad - bc} \begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}
$$
dengan syarat bahwa $ad - bc \neq 0$.

## 5. Contoh
Mari kita cari invers dari matriks:
$$
A = \begin{pmatrix}
4 & 7 \\
2 & 6
\end{pmatrix}
$$

1. **Hitung determinan**:
   $$
   \text{det}(A) = (4)(6) - (7)(2) = 24 - 14 = 10
   $$
   Karena $\text{det}(A) \neq 0$, matriks ini dapat dibalik.

2. **Gunakan rumus invers**:
   $$
   A^{-1} = \frac{1}{10} \begin{pmatrix}
   6 & -7 \\
   -2 & 4
   \end{pmatrix} = \begin{pmatrix}
   0.6 & -0.7 \\
   -0.2 & 0.4
   \end{pmatrix}
   $$

## 6. Invers dari Matriks yang Lebih Besar
Untuk matriks yang lebih besar, mencari invers dapat dilakukan dengan:
- **Pengurangan Baris**: Menggabungkan matriks dengan matriks identitas dan melakukan pengurangan baris untuk menemukan invers.
- **Metode Kofaktor**: Menemukan matriks *adjugate* dan membagi dengan determinan.

## 7. Properti Invers
- $(A^{-1})^{-1} = A$
- $(AB)^{-1} = B^{-1} A^{-1}$
- $(A^T)^{-1} = (A^{-1})^T$

---
