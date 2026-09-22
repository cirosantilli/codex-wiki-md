<h1 id="34b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In position space,

$$
\begin{aligned}
\Psi_k(x)
&=\sum_{n=0}^2e^{ikna}\psi(x-na)\\
&=e^{ikx}\sum_{n=0}^2\psi(x-na)e^{-ik(x-na)}.
\end{aligned}
$$

Hence

$$
\Psi_k(x)=e^{ikx}u_k(x),
\qquad
u_k(x)=\sum_{n=0}^2\psi(x-na)e^{-ik(x-na)},
$$

up to the common normalization factor $1/\sqrt3$.

Under $x\mapsto x+a$, reindexing $m=n-1$ gives the same three terms modulo three sites. The term shifted by three sites is unchanged because $\psi_{m+3}=\psi_m$ and $e^{3ika}=1$. Therefore

$$
\boxed{u_k(x+a)=u_k(x)}.
$$

The one-dimensional [Bloch theorem](../../../../../../bloch-s-theorem.md) states that an eigenfunction in a potential of period $a$ can be chosen in the form

$$
\Psi_k(x)=e^{ikx}u_k(x),
\qquad u_k(x+a)=u_k(x).
$$

It applies because the three-atom ring is invariant under translation by one lattice spacing and obeys periodic boundary conditions.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [34B](../../34b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
