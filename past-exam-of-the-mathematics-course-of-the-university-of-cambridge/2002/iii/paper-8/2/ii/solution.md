<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $F=f_2$. Split the integral in the assumed tail bound according to whether $g\leq a/2$ or $g>a/2$:

$$
a\mu\{F>a\}\leq\frac a2\mu\{F>a\}+\int_{\{g>a/2\}}g\,d\mu.
$$

The finite-superlevel hypothesis permits subtraction of the first term. With $a=2b$, this becomes

$$
b\mu\{F>2b\}\leq\int_{\{g>b\}}g\,d\mu.
$$

Thus $F/2$ satisfies part (i), which proves finiteness and the preliminary estimate

$$
\boxed{\|F\|_p^p\leq2^p q\|g\|_p^p}.
$$

Now integrate the original tail bound against $pa^{p-2}$. The [layer cake representation](../../../../../../layer-cake-representation.md) and [Tonelli theorem](../../../../../../tonelli-theorem.md) give

$$
\|F\|_p^p\leq q\int_XgF^{p-1}\,d\mu\leq q\|g\|_p\|F\|_p^{p-1},
$$

where the second step is [Hölder's inequality](../../../../../../holder-s-inequality.md). The preliminary estimate justified the finiteness needed here. If $\|F\|_p=0$ the result is immediate; otherwise divide by its $(p-1)$st power. This proves the [Lp bound from a tail domination inequality](../../../../../../lp-bound-from-a-tail-domination-inequality.md):

$$
\boxed{\|F\|_p\leq q\|g\|_p,\qquad \|F\|_p^p\leq q^p\|g\|_p^p}.
$$

The printed strict signs cannot hold when $g=F=0$: both sides are zero. The universally valid formulation therefore has non-strict inequalities. If $\|g\|_p>0$, the sharper estimate is actually strict, as follows.

Suppose equality held and $\|F\|_p>0$. Equality in [Hölder's inequality](../../../../../../holder-s-inequality.md) and the norm relation force $g=F/q$ [almost everywhere](../../../../../../almost-everywhere.md); equality in the preceding integrated tail inequality forces equality in that tail inequality for almost every $a>0$. Put $H(a)=\mu\{F>a\}$ and $J(a)=\int_a^\infty H(t)\,dt$. The layer-cake identity on $\{F>a\}$ gives $\int_{\{F>a\}}F=aH(a)+J(a)$, so equality implies

$$
J(a)=(q-1)aH(a)\quad\text{for almost every }a>0.
$$

Because $F\in L^p$ and $p>1$, $J$ is finite for positive $a$, locally absolutely continuous, and $J'=-H$ [almost everywhere](../../../../../../almost-everywhere.md). It follows that $J'=-(p-1)J/a$, whose solutions on $(0,\infty)$ are $J(a)=c a^{1-p}$. If $c>0$, then $H(a)=c(p-1)a^{-p}$ almost everywhere, and $p\int_0^\infty a^{p-1}H(a)\,da$ diverges. If $c=0$, then $F=0$ almost everywhere. Both contradict the assumed nonzero finite equality case. If $F=0$ but $g\ne0$, strictness is immediate.

Thus both requested strict estimates hold when $\|g\|_p>0$: the coarse constant is strictly larger than the sharp one since $q^{1/q}\leq e^{1/e}<2$, so $q^p<2^p q$. The zero-data exception is the only qualification needed here.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
