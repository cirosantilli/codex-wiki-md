<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The chain is a random walk on the finite abelian group $(\mathbb Z/n\mathbb Z)^d$, so its stationary distribution is uniform and its characters diagonalize the transition operator. For one coordinate and $\theta=2\pi k/n$, the eigenvalue is

$$
\lambda_{p}(\theta)=\frac12+
rac p2e^{i\theta}+
rac{1-p}{2}e^{-i\theta}.
$$

Uniformly in $p\in[0,1]$,

$$
|\lambda_p(\theta)|^2
\leq1-c\min\left\{\frac{k^2}{n^2},1\right\}
$$

for an absolute $c>0$. Hence the one-coordinate chi-squared distance after $t\geq n^2$ is at most $Ce^{-ct/n^2}$. The coordinates evolve independently, so the product formula for chi-squared distance gives

$$
1+\chi^2_d(t)
=\prod_{j=1}^d(1+\chi^2_j(t))
\leq\exp\left(Cd e^{-ct/n^2}\right).
$$

The [chi-squared divergence](../../../../../../chi-squared-divergence.md) bound on [total variation distance](../../../../../../total-variation-distance.md) now yields

$$
\boxed{t_{\mathrm{mix}}=O(n^2\log(d+1)),}
$$

uniformly in $p_1,\ldots,p_d$.

For $d=1$, the first nonconstant character has eigenvalue modulus $1-O(n^{-2})$, uniformly in $p$. Testing against its real or imaginary part gives a fixed positive total-variation distance until time $cn^2$. Thus

$$
\boxed{t_{\mathrm{mix}}=\Theta(n^2)\quad(d=1).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
