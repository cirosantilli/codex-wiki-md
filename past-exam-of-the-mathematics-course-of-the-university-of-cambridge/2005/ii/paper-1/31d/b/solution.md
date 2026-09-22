<h1 id="31d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The jump coefficient $G(t)=(t^2-1)/t$ has one enclosed pole at zero and no enclosed zeros, because $\pm1$ are outside. Its winding index is therefore **$\kappa=-1$**. A homogeneous canonical pair is

$$
\boxed{X_+(z)=z^2-1,\qquad X_-(z)=z,\qquad X_+/X_-=G.}
$$

Each is analytic and nonvanishing in its required finite domain; the exterior growth $X_-\sim z$ encodes the negative index. Dividing the unknown by these factors gives an additive jump

$$
D_+-D_-=g(t),\qquad g(t)=\frac{t-1+K}{2t(t^2-1)}.
$$

The Cauchy-integral solution for $D$ normally has an exterior $z^{-1}$ coefficient $-(2\pi i)^{-1}\int_Lg$. Since $C_-=zD_-$ must decay, this coefficient must vanish. Thus the solvability condition is $\int_Lg(t)dt=0$. Its only enclosed pole is zero, with residue $(1-K)/2$, so

$$
\boxed{K=1.}
$$

These are the [negative-index scalar Riemann-Hilbert moment conditions](../../../../../../negative-index-scalar-riemann-hilbert-moment-conditions.md) for index minus one. There is no arbitrary [polynomial](../../../../../../polynomial-split.md) addition: an entire addition respecting $D_-=O(z^{-2})$ is zero by Liouville's theorem.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [31D](../../31d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
