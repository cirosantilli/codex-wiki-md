<h1 id="18c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Insert the exact solution into the [linear multistep method](../../../../../../linear-multistep-method.md) and expand about $t_n$. Its defect is

$$
\sum_{l=0}^s\rho_l y(t_n+lh)-h\sum_{l=0}^s\sigma_l y'(t_n+lh).
$$

The coefficient of $h^k y^{(k)}(t_n)$ is

$$
\frac1{k!}\sum_l\rho_l l^k-\frac1{(k-1)!}\sum_l\sigma_l l^{k-1}
$$

for $k\geq1$, while the constant coefficient is $\sum_l\rho_l$. The method has order at least $p$ exactly when these coefficients vanish for $0\leq k\leq p$.

On the other hand,

$$
\rho(e^z)-z\sigma(e^z)
=\sum_l\rho_l e^{lz}-z\sum_l\sigma_l e^{lz}.
$$

The coefficient of $z^k$ in this expression is precisely the preceding order-condition coefficient. Therefore all coefficients through degree $p$ vanish exactly when

$$
\boxed{\rho(e^z)-z\sigma(e^z)=O(z^{p+1})},
$$

which proves the equivalence.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18C](../../18c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
