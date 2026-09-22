<h1 id="11f/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $n\geq1$, substitute $s=e^{t/n}$ in the [probability generating function](../../../../../../probability-generating-function.md). The [moment-generating function](../../../../../../moment-generating-function.md) of $X_n/n$ is

$$
\boxed{M_{X_n/n}(t)=\frac{n-(n-1)e^{t/n}}{n+1-ne^{t/n}}},\qquad
\boxed{t<n\log(1+1/n)}.
$$

The domain follows from convergence of the generating series; at or above that positive threshold the expectation diverges, even though a rational continuation can be written.

Conditioning on survival, the [probability mass function](../../../../../../probability-mass-function.md) from part (ii) becomes a positive-integer [geometric distribution](../../../../../../geometric-distribution.md):

$$
P(X_n=j\mid X_n>0)=\frac1{n+1}\left(\frac n{n+1}\right)^{j-1},\qquad j\geq1.
$$

Its conditional [moment-generating function](../../../../../../moment-generating-function.md) is $e^{t/n}/[n+1-ne^{t/n}]$, tending to $1/(1-t)$ for fixed $t<1$. We can prove the required limit directly, without invoking a continuity theorem. Set $r_n=n/(n+1)$. For every $x\geq0$, the strict upper tail is exactly

$$
P(X_n/n>x\mid X_n>0)=r_n^{\lfloor nx\rfloor}.
$$

Since $\log r_n=-1/n+O(n^{-2})$ and $\lfloor nx\rfloor/n\to x$,

$$
\boxed{P(X_n/n>x\mid X_n>0)\longrightarrow e^{-x}}.
$$

At $x=0$ both tails equal one. This is the [exponential limit of surviving geometric branching](../../../../../../exponential-limit-of-surviving-geometric-branching.md). Conditioning is essential: the unconditional variable has [probability](../../../../../../probability.md) $n/(n+1)$ of being zero, whereas the rare surviving population has size of order $n$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
