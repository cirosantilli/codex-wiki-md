<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Work in the centre-of-mass frame and define $I=\sum_i m|\mathbf r_i|^2$, $T=\tfrac12\sum_i m|\mathbf v_i|^2$. Differentiation gives

$$
\frac12\ddot I=2T+\sum_i\mathbf r_i\cdot\mathbf F_i.
$$

For each gravitational pair, the two contributions combine to

$$
(\mathbf r_i-\mathbf r_j)\cdot\mathbf F_{ij}
=-\frac{Gm^2}{|\mathbf r_i-\mathbf r_j|}.
$$

Summing pairs therefore gives the exact scalar [virial theorem](../../../../../../virial-theorem.md)

$$
\boxed{\frac12\ddot I=2T+W,\qquad
W=-\sum_{i<j}\frac{Gm^2}{r_{ij}}.}
$$

In a stationary equilibrium, or a bounded long-time average with vanishing average $\ddot I$, $2T=-W$. With $M=Nm$, the stated [gravitational radius](../../../../../../gravitational-radius.md) gives $W=-GM^2/R_g$, hence

$$
\boxed{\langle v_{\rm eq}^2\rangle=\frac{2T}M=\frac{GNm}{R_g}.}
$$

The rms speed itself is $[GNm/R_g]^{1/2}$. This is a three-dimensional mean-square speed; for an isotropic system the one-component [velocity dispersion](../../../../../../velocity-dispersion.md) is smaller by a factor of three in its square. No assumption about a uniform spatial density was used.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
