<h1 id="12g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $f$ is a [bounded linear operator](../../../../../../continuous-linear-operator.md), linearity gives $\|f(u)-f(v)\|\leq C\|u-v\|$. It is therefore Lipschitz and continuous everywhere.

Conversely, suppose $f$ is continuous at zero. There is $\delta>0$ such that $\|u\|<\delta$ implies $\|f(u)\|<1$. For $u\ne0$, apply this to $v=\delta u/(2\|u\|)$ and use homogeneity:

$$
\frac{\delta}{2\|u\|}\|f(u)\|=\|f(v)\|<1.
$$

The value at $u=0$ is zero by linearity. Consequently

$$
\boxed{\|f(u)\|\leq\frac2\delta\|u\|\text{ for every }u.}
$$

Thus **boundedness and continuity are equivalent for linear maps between normed spaces**. No finite dimensionality or completeness is needed for this equivalence.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12G](../../12g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
