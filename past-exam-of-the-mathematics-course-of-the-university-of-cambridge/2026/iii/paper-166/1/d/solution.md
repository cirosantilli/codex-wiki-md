<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Fix a finite set $S$ of [primes](../../../../../../prime-number.md). We prove that only finitely many denominators $q_n$ can be [S-smooth number](../../../../../../s-smooth-number.md). This is the standard finite-place corollary of the [Schmidt subspace theorem](../../../../../../schmidt-subspace-theorem.md) for [best approximations of the first kind](../../../../../../best-rational-approximation.md); the reduction is recalled here because the target $\alpha$ need not be algebraic.

Apply the [Dirichlet approximation theorem](../../../../../../dirichlet-s-approximation-theorem.md) at each cutoff between two successive record denominators. Its approximant can be replaced by the last record without increasing the error. Apply the finite-place [Schmidt subspace theorem](../../../../../../schmidt-subspace-theorem.md) to the resulting pairs of primitive vectors, using $X-\alpha Y,Y$ at the real place only after eliminating $\alpha$ between two successive pairs, and $X,Y$ at every place belonging to $S$. The factors

$$
\prod_{\ell\in S}|q_n|_\ell=q_n^{-1}
$$

for an $S$-smooth denominator supply the required height saving. If infinitely many such records existed, one fixed rational subspace would contain infinitely many of the paired vectors. Eliminating its rational linear relation has two possible outcomes: either all sufficiently late records represent one rational number, which contradicts the irrationality of $\alpha$, or $\alpha$ is algebraic and, for some $\eta>0$, infinitely many of the records satisfy

$$
\left|\alpha-\frac{p_n}{q_n}\right|<q_n^{-2-\eta}.
$$

The latter alternative contradicts the [Roth theorem](../../../../../../roth-s-theorem.md). Thus only finitely many $q_n$ are $S$-smooth.

If the [largest prime factor](../../../../../../largest-prime-factor.md) of $q_n$ did not tend to infinity, some bound $B$ would contain the largest prime factor for infinitely many $n$. Taking $S$ to be the finite set of primes at most $B$ would make those denominators $S$-smooth, contrary to the preceding conclusion. Therefore $P^+(q_n)\to\infty$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 166](../../../paper-166-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
