<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Each run of [Simon's algorithm](../../../../simon-s-algorithm.md) uses **one oracle call** and returns one uniform sample from $s^\perp$. Collect samples as rows of a [matrix](../../../../matrix.md) $Z$ and solve $Zs=0$ over the two-element [field](../../../../field.md) using [Gaussian elimination](../../../../gaussian-elimination.md). Once the rows have [matrix rank](../../../../matrix-rank.md) $n-1$, the [kernel](../../../../kernel-of-a-linear-map-split.md) is $\{0,s\}$, so the promised nonzero vector is uniquely determined. Dependent samples, including $z=0$, must be allowed for; exactly $n-1$ runs need not suffice.

For a rough quantitative estimate, put $d=n-1$. When the existing samples span an $r$-dimensional [vector subspace](../../../../vector-subspace.md) of $s^\perp$, the next sample increases the [matrix rank](../../../../matrix-rank.md) with [probability](../../../../probability.md) $1-2^{r-d}$. The [random spanning of a binary vector space](../../../../random-spanning-of-a-binary-vector-space.md) estimate gives

$$
\mathbb E Q=\sum_{r=0}^{d-1}\frac1{1-2^{r-d}}
=d+\sum_{j=1}^d\frac1{2^j-1}<d+2=n+1.
$$

Alternatively, $m=d+t$ samples fail to span with [probability](../../../../probability.md) less than $2^{-t}$: failure means some nonzero [linear functional](../../../../linear-functional.md) on the $d$-dimensional space vanishes on every sample, and a [union bound](../../../../boole-s-inequality.md) gives $(2^d-1)2^{-m}$. Consequently

$$
\boxed{Q_{\rm quantum}=O(n)\text{ for fixed error},\qquad
Q_{\rm quantum}=O\bigl(n+\log(1/\varepsilon)\bigr)\text{ for error }\varepsilon.}
$$

The [Gaussian elimination](../../../../gaussian-elimination.md) requires only a polynomial amount of classical work, for example $O(n^3)$ bit operations for $O(n)$ samples. The degenerate case $n=1$ needs no calls because the promise already specifies $s=1$.

Classically, distinct inputs with equal function values reveal $s=x\oplus x'$. Uniformly sampling distinct inputs finds such a [function collision](../../../../function-collision.md) after roughly $\sqrt{2^n}$ calls, by the [birthday square-root scale](../../../../birthday-square-root-scale.md). For $q$ sampled inputs, the expected number of colliding pairs is $\binom q2/(2^n-1)$. The usual randomized classical [query complexity](../../../../query-complexity.md) of [Simon's problem](../../../../simon-s-problem.md) is therefore exponential in $n$, on the scale

$$
\boxed{Q_{\rm classical}=\Theta(2^{n/2})\text{ for bounded error},\qquad
Q_{\rm quantum}=O(n).}
$$

A straightforward exhaustive classical search instead uses $O(2^n)$ calls. The square-root collision estimate is the sharper classical comparison; the quantum advantage concerns access to the promised [quantum oracle](../../../../quantum-oracle.md), rather than an explicit table of all function values.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the introduction to quantum information course of the University of Oxford](../../../split.md)
5. [Introduction to quantum information course of the University of Oxford](../../../../introduction-to-quantum-information-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
