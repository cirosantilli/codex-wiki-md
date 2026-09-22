<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $f$ be [holomorphic](../../../../../complex-differentiability-at-a-point.md) on a neighborhood of the closure of a bounded region with piecewise smooth positively oriented boundary, with no boundary zeros and with $f$ not identically zero. The [argument principle](../../../../../argument-principle.md) states

$$
\boxed{\frac1{2\pi i}\int_{\partial G}\frac{f'(z)}{f(z)}\,dz=\sum_{a\in G:f(a)=0}m_a,}
$$

where $m_a$ is the zero [multiplicity](../../../../../multiplicity-mathematics.md). More generally a closed contour avoiding the zeros gives $\sum_a m_a\operatorname{Ind}(\Gamma,a)$, and the integral is the [winding number](../../../../../winding-number.md) of $f\circ\Gamma$ about zero.

To prove it, factor near a zero $a$ as $f(z)=(z-a)^{m_a}h(z)$ with $h(a)\ne0$. Then $f'/f=m_a/(z-a)+h'/h$. Remove small disjoint circles about the finitely many zeros in the region. On the remainder $f'/f$ is [holomorphic](../../../../../complex-differentiability-at-a-point.md), so the [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md) reduces the boundary integral to the sum of the small-circle integrals. Each is $2\pi i m_a$ because $h'/h$ is [holomorphic](../../../../../complex-differentiability-at-a-point.md) on its small disc. This proves the formula. Along a contour, the imaginary part of $d\log f$ is the change in a continuous argument, giving the winding interpretation and the indexed version.

Now choose a closed disc $\overline{D(z_0,r)}\subset\Omega$ on which $z_0$ is the only zero of the nonconstant limit $f$. Its boundary has $\min|f|>0$. [Local uniform convergence](../../../../../locally-uniform-convergence.md) gives $\max|f_n-f|<\min|f|$ there for all sufficiently large $n$. The contour functions $f+t(f_n-f)$, $0\le t\le1$, have no boundary zero. Their [winding numbers](../../../../../winding-number.md) are constant under this homotopy, so the [argument principle](../../../../../argument-principle.md) shows that $f_n$ has exactly the same positive number $m$ of zeros, counted with [multiplicity](../../../../../multiplicity-mathematics.md), inside the disc. This is the [Rouche theorem](../../../../../rouche-s-theorem.md) argument, here derived from the contour count.

Choose a zero $z_n$ in that disc. For every $0<\epsilon<r$, the compact annulus $\epsilon\le|z-z_0|\le r$ contains no zero of $f$, so [uniform convergence](../../../../../uniform-convergence.md) makes $f_n$ nonzero on it eventually. Therefore all of the chosen zeros eventually lie within $\epsilon$ of $z_0$. Consequently

$$
\boxed{f_n(z_n)=0,\qquad z_n\longrightarrow z_0.}
$$

The maps $f_n$ are eventually not identically zero, since they converge at any fixed point where $f$ is nonzero; thus their zero counts above are legitimate.

A double zero need not persist as a double zero. On the [unit disc](../../../../../unit-disc.md) take $f(z)=z^2$, $f_n(z)=z^2+1/n$. Its zeros $\pm i/\sqrt n$ converge to zero but are simple, while $f_n'$ vanishes only at zero and $f_n(0)=1/n\ne0$. Hence **the additional simultaneous [derivative](../../../../../derivative.md) condition cannot always be imposed**. [Local uniform convergence](../../../../../locally-uniform-convergence.md) preserves total nearby [multiplicity](../../../../../multiplicity-mathematics.md), not its concentration at a single point.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 86](../../paper-86-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
