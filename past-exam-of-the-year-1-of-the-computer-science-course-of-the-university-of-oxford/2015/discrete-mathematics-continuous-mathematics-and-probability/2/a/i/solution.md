<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

There are $n(n-1)\cdots(n-k+1)$ ordered selections without replacement. Each unordered $k$-element [subset](../../../../../../subset.md) occurs in exactly $k!$ orders, so the [binomial coefficient](../../../../../../binomial-coefficient-split.md) is

$$
\boxed{\binom nk=\frac{n!}{k!(n-k)!}.}
$$

One precise specification of its [domain](../../../../../../domain-mathematical-analysis.md), [codomain](../../../../../../codomain.md), and map is

$$
\boxed{C:D\longrightarrow\mathbb N_0,\qquad
D=\{(n,k)\in\mathbb N_0^2:0\le k\le n\},\qquad
(n,k)\longmapsto\frac{n!}{k!(n-k)!}.}
$$

Here $\mathbb N_0=\{0,1,2,\ldots\}$, and $0!=1$ includes the single empty selection. The actual values on $D$ are positive, so $\mathbb N_+$ is also a valid [codomain](../../../../../../codomain.md). For fixed $n$, one can instead use the [function](../../../../../../function-split.md) $C_n:\{0,\ldots,n\}\to\mathbb N_+$ with $C_n(k)=\binom nk$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
