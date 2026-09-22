<h1 id="2/a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A direct [exponential minimization construction of a bounded pricing kernel](../../../../../../../exponential-minimization-construction-of-a-bounded-pricing-kernel.md) proves the reverse implication without using a course theorem. Consider

$$
F(h)=\mathbb E[e^{-h\cdot P}]+h\cdot p,\qquad h\in\mathbb R^n.
$$

Boundedness of $P$ makes $F$ finite, continuous, and differentiable. On every bounded set of $h$, the exponential and its derivatives have deterministic bounds, so differentiation under expectation is justified.

We first prove [coercivity](../../../../../../../coercive-function.md): $F(h)\to\infty$ as $|h|\to\infty$. Otherwise there would be a sequence $h_j$ with $|h_j|\to\infty$ along which $F(h_j)$ stays bounded above. Pass to a subsequence with $h_j/|h_j|\to u$, $|u|=1$. There are two cases.

If $\mathbb P(u\cdot P<0)>0$, choose $a>0$ with $\delta=\mathbb P(u\cdot P\leq-a)>0$. The bound on $P$ gives $h_j\cdot P\leq-a|h_j|/2$ on this event for all large $j$. Therefore

$$
F(h_j)\geq\delta e^{a|h_j|/2}-|p|\,|h_j|\longrightarrow\infty.
$$

If instead $u\cdot P\geq0$ almost surely, the portfolio condition forces $u\cdot p>0$, since $u\ne0$. Hence $h_j\cdot p\to\infty$, and the nonnegative exponential term again forces $F(h_j)\to\infty$. Both cases contradict the chosen sequence.

A minimizing sequence is consequently bounded. It has a convergent subsequence, and continuity of $F$ gives a global minimizer $h_*$. At a minimizer each directional derivative vanishes, so

$$
0=\nabla F(h_*)=p-\mathbb E[Pe^{-h_*\cdot P}].
$$

Thus

$$
\boxed{Y=e^{-h_*\cdot P}>0,\qquad \mathbb E[PY]=p.}
$$

If $|P|\leq L$, then $e^{-|h_*|L}\leq Y\leq e^{|h_*|L}$: the constructed [pricing kernel](../../../../../../../state-price-density.md) is bounded and even bounded away from zero. The compactness, coercivity, and differentiation arguments above supply the needed proof rather than appealing to the [fundamental theorem of asset pricing](../../../../../../../fundamental-theorem-of-asset-pricing.md).

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
