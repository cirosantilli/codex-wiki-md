<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $a\ne b$, the operator $Q_{ab}=i\gamma_a\gamma_b$ is Hermitian and

$$
Q_{ab}^2=-\gamma_a\gamma_b\gamma_a\gamma_b=1.
$$

Therefore

$$
(\Pi_\pm^{(ab)})^2
=\frac14(1\pm2Q_{ab}+Q_{ab}^2)
=\Pi_\pm^{(ab)},
\qquad
\Pi_+^{(ab)}\Pi_-^{(ab)}=0.
$$

For $f=(\gamma_a+i\gamma_b)/2$, one has $Q_{ab}=2f^\dagger f-1$, so these projectors distinguish the two occupations, equivalently the two values of pair [fermion parity](../../../../../../fermion-parity.md). This proves that

$$
\boxed{\Pi_\pm^{(ab)}=\frac12(1\pm i\gamma_a\gamma_b)}
$$

describe a fermion-parity measurement.

Let $P=\Pi_+^{(N0)}$ and suppose $P|\psi\rangle=|\psi\rangle$. The bilinears $i\gamma_a\gamma_0$ and $i\gamma_b\gamma_0$ each anticommute with $i\gamma_N\gamma_0$, whereas their product commutes with it. Expanding the projectors and sandwiching by $P$ therefore gives

$$
\begin{aligned}
P\Pi_{s_a}^{(a0)}\Pi_{s_b}^{(b0)}P
&=\frac14P(1+i s_a\gamma_a\gamma_0)
(1+i s_b\gamma_b\gamma_0)P\\
&=\frac14(1+s_as_b\gamma_a\gamma_b)P\\
&=\frac1{2\sqrt2}
R_{ab}^{s_as_b}P.
\end{aligned}
$$

After normalizing the post-measurement state, the sequence consequently implements

$$
\boxed{R_{ab}^{s_as_b}}
$$

on the encoded ground space. This is [Measurement-only Majorana braiding](../../../../../../measurement-only-majorana-braiding.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
