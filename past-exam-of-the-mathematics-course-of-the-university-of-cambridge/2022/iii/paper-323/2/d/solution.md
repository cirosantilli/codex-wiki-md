<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $q_j=\langle z_j|\rho|z_j\rangle$, $r_j=\langle z_j|Y(\rho)|z_j\rangle$, and $c=\max_{i,j}|\langle y_i|z_j\rangle|^2$. Then

$$
r_j=\sum_ip_i|\langle z_j|y_i\rangle|^2\leq c,
$$

and therefore

$$
D(Z(\rho)\|Z(Y(\rho)))
=\sum_jq_j\log\frac{q_j}{r_j}
\geq-S(Z(\rho))-\log c.
$$

The [data-processing inequality for quantum relative entropy](../../../../../../data-processing-inequality-for-quantum-relative-entropy.md) applied to $Z$ and part c give

$$
S(Y(\rho))-S(\rho)
\geq D(Z(\rho)\|Z(Y(\rho))).
$$

Combining them proves

$$
\boxed{S(Y(\rho))+S(Z(\rho))\geq-\log c+S(\rho)}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
