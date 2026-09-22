<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $c\in\{0,1\}$ set

$$
\zeta_c=\exp(cY-Y^2-\|X\|^2).
$$

The quadratic negative terms make

$$
F_c(h)=\mathbb E[e^{-h\cdot X}\zeta_c]
$$

everywhere finite and smooth. Existence of the assumed $\rho$ rules out the arbitrage direction in part (c) by part (a). Hence each $F_c$ has a bounded minimizing sequence, and part (b) supplies

$$
\rho_c=\frac{
\exp(-h_c\cdot X+cY-Y^2-\|X\|^2)}{F_c(h_c)}
$$

with $\mathbb E\rho_c=1$ and $\mathbb E(\rho_cX)=0$. Uniqueness forces $\rho_0=\rho_1$. Taking logarithms and cancelling the common quadratic terms gives

$$
Y=(h_1-h_0)\cdot X+\log F_1(h_1)-\log F_0(h_0).
$$

Thus

$$
\boxed{Y=a+b\cdot X}
$$

with $b=h_1-h_0$ and $a=\log F_1(h_1)-\log F_0(h_0)$. Since $Y$ was arbitrary, the one-period market is complete.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
