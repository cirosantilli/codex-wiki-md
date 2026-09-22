<h1 id="3/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write the [semimartingale decomposition](../../../../../../../semimartingale-decomposition.md) as $U=M+A$, where $M$ is a continuous local martingale and $A$ has finite variation. Applying [Itô formula](../../../../../../../ito-s-lemma.md) to $\log Z_t(z)$ shows that its finite-variation part is

$$
\frac{2}{Z_t(z)^2}dt
-\frac1{Z_t(z)}dA_t
-\frac1{2Z_t(z)^2}d\langle M\rangle_t.
$$

It vanishes for every $z$. Multiplying by $Z_t(z)^2$ gives

$$
2dt-Z_t(z)dA_t-\frac12d\langle M\rangle_t=0.
$$

Subtract this identity for two points with distinct $Z_t$ to obtain $dA_t=0$; then $d\langle M\rangle_t=4dt$. Since the curve starts at zero, $U_0=0$. The [Lévy characterization of Brownian motion](../../../../../../../levy-characterization-of-brownian-motion.md) now gives $U_t=2B_t$. Hence the Loewner chain is

$$
\boxed{\operatorname{SLE}_4.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Paper 203](../../../../paper-203-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
