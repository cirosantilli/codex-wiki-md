<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take $M=\mathbb R$ and the constant [contraction mapping](../../../../contraction-mapping.md) $f(x)=0$. For $p=(0,0)$, $q=(0,1)$,

$$
\delta(p,q)=1,\qquad F(p)=(0,0),\quad F(q)=(1,0),\qquad\delta(F(p),F(q))=1.
$$

No Lipschitz constant less than one can work, so **$F$ need not be a contraction**. More generally, differing only in the second input coordinate already prevents a strict contraction whenever $M$ has two points.

If $f$ has contraction constant $0\leq c<1$, two iterations give

$$
F^2(m,m')=(f(m),f(m')),
$$

and consequently

$$
\boxed{\delta(F^2(p),F^2(q))\leq c\,\delta(p,q).}
$$

Thus **$F^2$ is a [contraction mapping](../../../../contraction-mapping.md)**. The [swap lift of a contraction](../../../../swap-lift-of-a-contraction.md) shows why an iterate can contract even when one step does not.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
