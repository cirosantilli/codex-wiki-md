<h1 id="10c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let Alice's two bits be $(x,z)$ and Bob's bit be $b$. Alice applies

$$
X_A^xZ_A^z,
$$

while Bob applies

$$
X_B^b.
$$

They then send their qubits to Charlie. Acting on

$$
|\chi_1^+\rangle
=\frac{|000\rangle+|111\rangle}{\sqrt2},
$$

these operations produce, up to an irrelevant global phase,

$$
\frac{|x,b,0\rangle+(-1)^z
|1\mathbin\oplus x,1\mathbin\oplus b,1\rangle}{\sqrt2}.
$$

The complete encoding table is

$$
\begin{array}{c|c|c}
(x,z)&b&\text{state measured by Charlie}\\ \hline
(0,0)&0&|\chi_1^+\rangle\\
(0,1)&0&|\chi_1^-\rangle\\
(0,0)&1&|\chi_2^+\rangle\\
(0,1)&1&|\chi_2^-\rangle\\
(1,0)&0&|\chi_4^+\rangle\\
(1,1)&0&|\chi_4^-\rangle\\
(1,0)&1&|\chi_3^+\rangle\\
(1,1)&1&|\chi_3^-\rangle
\end{array}
$$

where a possible overall minus sign in the two $x=z=1$ cases has no observable effect.

Charlie performs a projective measurement in the eight-state GHZ basis. The sign $+$ or $-$ reveals $z$. The basis index reveals $(x,b)$ according to

$$
1\leftrightarrow(0,0),
\quad
2\leftrightarrow(0,1),
\quad
3\leftrightarrow(1,1),
\quad
4\leftrightarrow(1,0).
$$

He therefore reconstructs Alice's two bits and Bob's one bit with certainty, which is the [three-party dense coding with a GHZ state](../../../../../../three-party-dense-coding-with-a-ghz-state.md) protocol.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10C](../../10c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
