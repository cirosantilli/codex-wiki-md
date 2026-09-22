<h1 id="20g/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Start with any generator $I=(\beta)$ and use the decomposition from part (d). For each $i$, choose an integer $n_i$ such that

$$
-\frac12\leq\lambda_i+n_i\leq\frac12,
$$

and put

$$
u=u_1^{n_1}\cdots u_m^{n_m},
\qquad
\alpha=\beta u.
$$

Since $u$ is a unit, $(\alpha)=(\beta)=I$. Moreover,

$$
\operatorname{Log}(\alpha)
=te+h,
\qquad
h=\sum_{i=1}^m(\lambda_i+n_i)\operatorname{Log}(u_i).
$$

The vector $h$ lies in the fixed compact parallelepiped

$$
P=\left\{\sum_i c_i\operatorname{Log}(u_i):|c_i|\leq\frac12\right\}.
$$

Hence there is a constant $M_K$ such that every real coordinate of every $h\in P$ is at most $M_K$, and every complex coordinate is at most $2M_K$.

For a real embedding $\sigma_i$,

$$
\log|\sigma_i(\alpha)|=t+h_i
\leq\frac{\log N(I)}{[K:\mathbb Q]}+M_K.
$$

For a chosen complex embedding $\tau_j$, the weighted coordinate gives

$$
2\log|\tau_j(\alpha)|=2t+h_{r+j}
\leq2\frac{\log N(I)}{[K:\mathbb Q]}+2M_K.
$$

The conjugate embedding has the same modulus. Exponentiating and taking any $C>e^{M_K}$ proves the [archimedean balancing of a principal ideal generator](../../../../../../archimedean-balancing-of-a-principal-ideal-generator.md):

$$
\boxed{
|\sigma(\alpha)|<C N(I)^{1/[K:\mathbb Q]}
}
$$

for every embedding $\sigma:K\to\mathbb C$, with $C$ depending only on $K$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [20G](../../20g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
