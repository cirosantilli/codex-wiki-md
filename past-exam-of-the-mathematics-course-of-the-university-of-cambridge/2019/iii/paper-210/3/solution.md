<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $K=K_n$, $\epsilon=\epsilon_n$, and choose

$$
\delta=\frac{M\epsilon}{8}.
$$

Take a $\delta$-net $(\theta^1,\ldots,\theta^N)$ of $H_1$ in $\ell^2$, with centers in $H_1$. Since every alternative lies in the $K$-dimensional Euclidean ball of radius $n$, the [volumetric covering bound](../../../../../volumetric-covering-bound.md) gives

$$
N\leq\left(1+\frac{2n}{\delta}\right)^K,
\qquad
\log N\leq C K\log n
$$

for all large $n$. Put $v_j=\theta^j-\theta_0$ and define the [Gaussian net test](../../../../../gaussian-net-test.md)

$$
\Psi_n
=\mathbf1\left\{
\max_{j\leq N}\left(
\langle Y-\theta_0,v_j\rangle
-\frac12\|v_j\|_2^2
\right)\geq0
\right\}.
$$

The inner products are well-defined Gaussian linear functionals because $v_j\in\ell^2$. Under $H_0$,

$$
\langle Y-\theta_0,v_j\rangle
\sim N\left(0,\frac{\|v_j\|_2^2}{n}\right),
$$

and $\|v_j\|_2\geq M\epsilon$. A Gaussian tail bound and a union bound give

$$
\mathbb E_{\theta_0}\Psi_n
\leq N\exp\left(-\frac{nM^2\epsilon^2}{8}\right).
$$

For any $\theta\in H_1$, choose $j$ with $\|\theta-\theta^j\|_2\leq\delta$. Then

$$
\mathbb E_\theta\langle Y-\theta_0,v_j\rangle
=\langle\theta-\theta_0,v_j\rangle
\geq\|v_j\|_2^2-\delta\|v_j\|_2
\geq\frac78\|v_j\|_2^2.
$$

Another Gaussian tail bound gives

$$
\mathbb E_\theta(1-\Psi_n)
\leq\exp\left(-\frac{9n\|v_j\|_2^2}{128}\right)
\leq\exp\left(-\frac{9M^2K\log n}{128}\right).
$$

Because $n\epsilon_n^2=K_n\log n$, the entropy term in the type-I bound is dominated by the signal exponent when $M$ is sufficiently large. Also $\epsilon_n^2\to0$ implies $K_n<n$ eventually, so $\log n\geq\log K_n$. Given $c_1>0$, choose $M$ large enough to obtain

$$
\boxed{
\max\left\{
\mathbb E_{\theta_0}\Psi_n,
\sup_{\theta\in H_1}\mathbb E_\theta(1-\Psi_n)
\right\}
\leq e^{-c_1K_n\log K_n}.}
$$

Enlarging $M$ if necessary handles the finitely many initial $n$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
