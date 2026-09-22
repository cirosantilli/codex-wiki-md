<h1 id="4g/solution">Solution</h1>

↑ **Parent:** [4G](../4g.md)

A binary [linear-feedback shift register](../../../../../linear-feedback-shift-register.md) stores $L$ bits, shifts them at each clock step, and inserts a fixed linear combination over $\mathbb F_2$ of the stored bits. Its output obeys a recurrence $s_n+c_1s_{n-1}+\cdots+c_Ls_{n-L}=0$. Write its connection [polynomial](../../../../../polynomial-split.md) as $C(D)=1+c_1D+\cdots+c_LD^L$; the corresponding monic [feedback polynomial](../../../../../feedback-polynomial.md) is $z^LC(z^{-1})$.

The [Berlekamp-Massey algorithm](../../../../../berlekamp-massey-algorithm.md) maintains the shortest recurrence fitting the observed prefix. Initialize $C=B=1$, length $L=0$, displacement $m=1$, and previous nonzero discrepancy $b=1$. At symbol $n$, calculate $d=s_n+\sum_{j=1}^Lc_js_{n-j}$. If $d=0$, increase $m$. If $d\ne0$, save $T=C$ and replace $C$ by $C-(d/b)D^mB$. If $2L\leq n$, replace $L$ by $n+1-L$, $B$ by $T$, $b$ by $d$, and $m$ by $1$; otherwise only increase $m$. In the binary field subtraction equals addition. The shifted previous discrepancy [polynomial](../../../../../polynomial-split.md) cancels the current discrepancy while preserving earlier equations. A failed recurrence of length $L$ at position $n$ requires a corrected length at least $n+1-L$ when this exceeds $L$, explaining the length update. Thus the algorithm recovers the shortest compatible register; a known bound $L$ and at least $2L$ output symbols suffice to identify its minimal recurrence.

For the printed twelve-bit prefix, the nonzero discrepancies occur at positions $n=0,1,2,5,6,7$ (indexing from zero). The successive updated pairs $(L,C)$ are

$$
(1,1+D),\quad(1,1),\quad(2,1+D^2),\quad(4,1+D^2+D^3),\quad(4,1+D+D^2),\quad(4,1+D+D^4).
$$

All remaining discrepancies vanish. Therefore

$$
\boxed{s_n=s_{n-1}+s_{n-4}\quad(n\geq4),\qquad
z^4+z^3+1\text{ is the shortest compatible feedback polynomial}.}
$$

The first four observed bits are the fill. Length four is necessary: a length-three recurrence would need to hold already at $n=3$ and no such recurrence fits the prefix. Indeed the equations at $n=3,4,5$ force $c_2=1$, $c_1+c_3=0$, $c_1+c_3=1$, a contradiction. Finite observations cannot rule out longer nonminimal registers.

## ↑ Ancestors (10)

1. [4G](../4g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
