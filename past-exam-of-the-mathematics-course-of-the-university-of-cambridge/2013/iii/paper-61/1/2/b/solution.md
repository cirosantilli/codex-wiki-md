<h1 id="1/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The indexing of the [Fejér sums](../../../../../../../fejer-sum.md) gives

$$
(n+m)\sigma_{n+m}(f)=\sum_{j=0}^{n+m-1}s_j(f),\qquad
n\sigma_n(f)=\sum_{j=0}^{n-1}s_j(f).
$$

Subtracting removes precisely the initial $n$ [Fourier partial sums](../../../../../../../fourier-partial-sum.md). Thus

$$
\boxed{v_{n,m}(f)=\frac{(n+m)\sigma_{n+m}(f)-n\sigma_n(f)}m}.
$$

For $n=0$, omit the second term, so that no undefined $\sigma_0$ is needed. Apply the triangle inequality and the [uniform-norm contraction of Fejér summation](../../../../../../../fejer-summation-is-a-uniform-norm-contraction.md) estimate to get

$$
\|v_{n,m}(f)\|_\infty
\le\frac{n+m}{m}\|\sigma_{n+m}(f)\|_\infty
+\frac n m\|\sigma_n(f)\|_\infty
\le\left(1+\frac{2n}{m}\right)\|f\|_\infty.
$$

Hence the [operator norm](../../../../../../../operator-norm.md) of the [de la Vallée Poussin sum](../../../../../../../de-la-vallee-poussin-sum.md) is at most **$1+2n/m$**.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [1](../../../1.md)
4. [Paper 61](../../../../paper-61-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
