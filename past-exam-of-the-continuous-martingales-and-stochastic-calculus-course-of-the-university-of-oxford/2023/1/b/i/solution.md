<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $S_N=\sum_{n=0}^N\sum_{k=0}^{2^n-1}a_{n,k}H_{n,k}$. The assumed [orthonormality](../../../../../orthonormal-set.md) of the [Haar wavelets](../../../../../haar-wavelet.md) gives

$$
\|S_N\|_{\mathcal H}^2=\sum_{n=0}^N\sum_{k=0}^{2^n-1}a_{n,k}^2.
$$

Enumerate the coefficients level by level as $A_1,A_2,\ldots$. They are [independent and identically distributed](../../../../../independent-and-identically-distributed-random-variables.md) [standard normal random variables](../../../../../standard-normal-random-variable.md), so the squares have [mean](../../../../../expected-value-split.md) one. The [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) implies

$$
\frac1m\sum_{j=1}^mA_j^2\longrightarrow1\quad\text{almost surely}.
$$

Consequently,

$$
\boxed{\|S_N\|_{\mathcal H}^2\longrightarrow\infty\quad\text{almost surely}.}
$$

A convergent sequence in a [Hilbert space](../../../../../hilbert-space-split.md) must be bounded in [norm](../../../../../norm.md). Hence this random [Haar wavelet](../../../../../haar-wavelet.md) series diverges in $\mathcal H$ [almost surely](../../../../../almost-sure-convergence.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the continuous martingales and stochastic calculus course of the University of Oxford](../../../../split.md)
6. [Continuous martingales and stochastic calculus course of the University of Oxford](../../../../../continuous-martingales-and-stochastic-calculus-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
