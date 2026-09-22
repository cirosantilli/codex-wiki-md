<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The difference between the two cumulative sums of [Fourier partial sums](../../../../../../fourier-partial-sum.md) is

$$
(n+m)\sigma_{n+m}(f)-n\sigma_n(f)=\sum_{j=n}^{n+m-1}s_j(f).
$$

Hence the [de la Vallée Poussin sum](../../../../../../de-la-vallee-poussin-sum.md) satisfies

$$
\boxed{v_{n,m}(f)=\frac{n+m}{m}\sigma_{n+m}(f)-\frac nm\sigma_n(f).}
$$

Using the [uniform-norm contraction of Fejér summation](../../../../../../fejer-summation-is-a-uniform-norm-contraction.md) on each term and the [triangle inequality](../../../../../../triangle-inequality.md) in the [supremum norm](../../../../../../supremum-norm.md),

$$
\begin{aligned}
\|v_{n,m}(f)\|_\infty
&\leq\frac{n+m}{m}\|\sigma_{n+m}(f)\|_\infty+\frac nm\|\sigma_n(f)\|_\infty\\
&\leq\left(1+\frac{2n}{m}\right)\|f\|_\infty.
\end{aligned}
$$

This proves the requested [operator norm](../../../../../../operator-norm.md) bound. When $n=0$ the identity reduces to $v_{0,m}=\sigma_m$ and the bound is one.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
