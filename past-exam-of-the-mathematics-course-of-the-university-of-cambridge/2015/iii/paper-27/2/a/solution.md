<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The points are $\delta$-spaced if their [circular spacing](../../../../../../circular-spacing.md) satisfies $\|\theta_r-\theta_s\|\geq\delta$ for $r\ne s$, where $\|t\|$ is distance to the nearest [integer](../../../../../../integer.md). Ordinary distance on the real line would be insufficient because the [complex exponential](../../../../../../complex-exponential-function.md) is periodic.

Let $S(t)=\sum_{M<n\leq M+N}a_ne(nt)$ and $F(t)=e(-Mt)S(t)$. Multiplication by this unit-modulus factor leaves $|S(t)|$ unchanged and places the frequencies of $F$ in $1,\ldots,N$. Put $E=\sum|a_n|^2$. The permitted [Sobolev–Gallagher inequality](../../../../../../sobolev-gallagher-inequality.md), in the form needed here, is

$$
|F(t)|^2\leq\delta^{-1}\int_{t-\delta/2}^{t+\delta/2}|F(u)|^2\,du
+\int_{t-\delta/2}^{t+\delta/2}|F(u)F\prime(u)|\,du.
$$

For $0<\delta\leq1$, the arcs about the $\theta_r$ have disjoint interiors on the [circle group](../../../../../../circle-group.md). Summing and applying the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
\sum_r|S(\theta_r)|^2\leq\delta^{-1}\int_0^1|F|^2
+\left(\int_0^1|F|^2\right)^{1/2}\left(\int_0^1|F\prime|^2\right)^{1/2}.
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) here follows by expanding $0\leq\int|u-cv|^2$ and minimizing over $c\in\mathbb C$. For completeness, the [finite-interval Parseval identities](../../../../../../finite-interval-parseval-identities.md) follow by expanding the squares: $\int_0^1e(kt)\,dt$ is one at $k=0$ and zero at every other [integer](../../../../../../integer.md) $k$. Thus $\int|F|^2=E$ and $\int|F\prime|^2\leq4\pi^2N^2E$. We obtain the [exponential-sum large sieve](../../../../../../exponential-sum-large-sieve.md) bound

$$
\boxed{\sum_r|S(\theta_r)|^2\leq(\delta^{-1}+2\pi N)E.}
$$

If $\delta>1$, there is at most one point, and the direct [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) bound $|S|^2\leq NE$ proves the same assertion.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
