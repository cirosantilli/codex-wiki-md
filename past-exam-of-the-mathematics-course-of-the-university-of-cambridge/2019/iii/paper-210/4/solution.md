<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Because white-noise observations are not themselves in $\ell^2$, define the least-squares estimator as a minimizer of the [Gaussian least-squares contrast](../../../../../gaussian-least-squares-contrast.md), equivalently a maximizer over $\theta\in\Theta$ of

$$
\mathcal L_n(\theta)
=2\langle Y,\theta\rangle-\|\theta\|_2^2
=2\langle\theta_0,\theta\rangle
+\frac2{\sqrt n}W(\theta)-\|\theta\|_2^2,
$$

where $W$ is the [isonormal Gaussian process](../../../../../isonormal-gaussian-process.md) on $\ell^2$. The entropy assumption makes $W$ sample-continuous on compact $\Theta$, so a maximizer exists.

Put $\Delta=\widehat\theta-\theta_0$. Comparison with $\theta_0$ gives the basic inequality

$$
\|\Delta\|_2^2
\leq\frac2{\sqrt n}W(\Delta).
$$

For

$$
Z(r)=\sup\{W(\theta-\theta_0):
\theta\in\Theta,\ \|\theta-\theta_0\|_2\leq r\},
$$

the entropy assumption and the [Dudley entropy integral](../../../../../dudley-entropy-integral.md) give

$$
\mathbb EZ(r)
\leq C\int_0^r
\sqrt{\log N(u,\Theta,\|\cdot\|_2)}du
\leq C\int_0^ru^{-1/8}du
\leq C'r^{7/8}.
$$

The [Borell-TIS inequality](../../../../../borell-tis-inequality.md) further gives

$$
\mathbb P\{Z(r)>\mathbb EZ(r)+rx\}
\leq e^{-x^2/2}.
$$

Set $r_n=cn^{-4/9}$. This is the balance

$$
r_n^2\asymp n^{-1/2}r_n^{7/8}.
$$

On the shell $2^jr_n\leq\|\theta-\theta_0\|_2<2^{j+1}r_n$, the basic inequality would require

$$
Z(2^{j+1}r_n)
\geq\frac{\sqrt n}{2}(2^jr_n)^2.
$$

For $c$ sufficiently large, the expectation bound is at most half this threshold for every $j$. Borell concentration then bounds the shell probability by

$$
\exp(-c_0\,4^j n r_n^2)
=\exp(-c_0c^2\,4^j n^{1/9}).
$$

Summing the geometric sequence of shell bounds gives a quantity tending to zero, uniformly in $\theta_0\in\Theta$. Therefore

$$
\boxed{
\mathbb P_{\theta_0}^Y
\left(\|\widehat\theta-\theta_0\|_{\ell^2}
\geq cn^{-4/9}\right)\longrightarrow0.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
