<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the bound in part (a) as $e^{-nD(x\Vert p)}$, where the Bernoulli [Kullback-Leibler divergence](../../../../../kullback-leibler-divergence.md) with natural logarithms is

$$
D(x\Vert p)=x\log\frac xp+(1-x)\log\frac{1-x}{1-p}.
$$

For fixed $p\in(0,1)$, $D(p\Vert p)=0$, its first [derivative](../../../../../derivative.md) with respect to $x$ vanishes at $p$, and

$$
\frac{d^2}{dx^2}D(x\Vert p)=\frac1{x(1-x)}\geq4.
$$

Integrating this lower bound twice, on either side of $p$, gives the [Bernoulli relative entropy lower bound](../../../../../bernoulli-relative-entropy-lower-bound.md) $D(x\Vert p)\geq2(x-p)^2$. Apply the two tails from part (a) at $x=p+h$ and $x=p-h$ and use the [union bound](../../../../../boole-s-inequality.md):

$$
\boxed{P(|X-np|\geq nh)\leq2e^{-2nh^2}.}
$$

A tail with threshold outside $[0,1]$ is empty; thresholds at the endpoints follow by [continuity](../../../../../continuous-function.md) of the bound. For $h=0$ the right-hand side is $2$, so the assertion is immediate. This is the binomial form of [Hoeffding inequality](../../../../../hoeffding-inequality.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
