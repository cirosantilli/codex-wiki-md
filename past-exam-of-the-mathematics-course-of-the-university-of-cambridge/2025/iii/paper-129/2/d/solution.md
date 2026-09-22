<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $d=|\Gamma|$ and identify each character with a residue $r_j\in\mathbb Z/N\mathbb Z$. Partition the $d$-dimensional torus into $Q^d$ cubes of side $1/Q$, where $Q$ is comparable to $N^{1/d}$. Applying the [pigeonhole principle](../../../../../../pigeonhole-principle.md) to the points

$$
\left(\frac{kr_1}{N},\ldots,\frac{kr_d}{N}\right),
\qquad 0\leq k\leq Q^d,
$$

gives a nonzero residue $q$ satisfying

$$
\left\|\frac{qr_j}{N}\right\|_{\mathbb R/\mathbb Z}\leq\frac1Q
\qquad(1\leq j\leq d).
$$

Consequently $|e^{2\pi imqr_j/N}-1|\leq\rho$ whenever $|m|\leq\rho Q/(4\pi)$. After allowing for integer parts and the small values of $Q$, this produces the centered [arithmetic progression](../../../../../../arithmetic-progression.md)

$$
\{-Lq,\ldots,0,\ldots,Lq\}\subseteq B(\Gamma,\rho)
$$

of length at least $\frac18\rho N^{1/d}$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
