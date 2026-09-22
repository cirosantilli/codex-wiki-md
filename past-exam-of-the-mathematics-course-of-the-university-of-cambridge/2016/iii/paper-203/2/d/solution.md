<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $g=g_K$ and $f=g^{-1}$. We use the [real boundary bounds for a unit-disc H-hull](../../../../../../real-boundary-bounds-for-a-unit-disc-h-hull.md) from part (c), including their reflected version. Set

$$
\alpha=\lim_{x\uparrow-1}g(x),\qquad
\beta=\lim_{x\downarrow1}g(x).
$$

Strict monotonicity and those bounds give $-2\leq\alpha\leq-1$ and $1\leq\beta\leq2$. The inverse $f$ extends across $\mathbb R\setminus[\alpha,\beta]$ and maps these intervals onto $(-\infty,-1)$ and $(1,\infty)$.

Consider the [holomorphic function](../../../../../../holomorphic-function.md) $F(w)=w-f(w)$ on $\mathbb H$. If $w$ approaches a real $u$ outside $[\alpha,\beta]$, its inverse tends to a real $x$ with $|x|>1$. Part (c) gives

$$
|u-f(u)|=|g(x)-x|\leq\frac1{|x|}\leq1.
$$

If $u\in[\alpha,\beta]$, every cluster point of $f(w)$ as $w\to u$ lies in the closed unit disc. To justify this without a boundary regularity assumption, first note that $f(w)$ cannot tend to infinity for bounded $w$, since $g(z)=z+O(1/z)$ there. An interior cluster point in $H$ would be mapped to the real number $u$, impossible for $g:H\to\mathbb H$. A real cluster point $x$ with $|x|>1$ would, by the reflected extension and strict monotonicity, have $g(x)$ outside $[\alpha,\beta]$, also impossible. All remaining finite boundary points lie in $K$ or in $[-1,1]$, hence in the unit disc.

It follows for every such $u$ that

$$
\limsup_{\substack{w\to u\\w\in\mathbb H}}|F(w)|
\leq |u|+1\leq3.
$$

Finally $f(w)=w+O(1/w)$ at infinity, so $F(w)\to0$ there. Apply the [maximum modulus principle](../../../../../../maximum-modulus-principle.md) on large upper half-discs, using the boundary limsup just obtained, to conclude $|F(w)|\leq3$ everywhere in $\mathbb H$. Taking $w=g(z)$ proves **the [sharp displacement bound for a compact H-hull](../../../../../../sharp-displacement-bound-for-a-compact-h-hull.md), including irregular hulls**:

$$
\boxed{|g_K(z)-z|\leq3\qquad(z\in H).}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
