<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Weak Harnack inequality](../../../../../../weak-harnack-inequality.md) is an estimate for a nonnegative [weak supersolution](../../../../../../weak-supersolution-of-a-divergence-form-elliptic-equation.md). Write $F=(f^1,\ldots,f^n)$, let $B_{2R}(x_0)\subset\subset\Omega$, and assume $u\geq0$ almost everywhere on this ball. There are $p>0$ and $C<\infty$, depending only on the dimension, the [uniform ellipticity](../../../../../../uniformly-elliptic-operator.md) bounds, $q$, and the scaled norms of the lower-order coefficients, such that

$$
\boxed{\left(\frac{1}{|B_R(x_0)|}\int_{B_R(x_0)}u^p\right)^{1/p}\leq C\left(\operatorname*{ess\,inf}_{B_R(x_0)}u+R^{1-n/q}\|F\|_{L^q(B_{2R})}+R^{2-2n/q}\|g\|_{L^{q/2}(B_{2R})}\right).}
$$

Here $\langle v\rangle_E=|E|^{-1}\int_Ev$ is the [integral average](../../../../../../integral-average.md). The [weak supersolution](../../../../../../weak-supersolution-of-a-divergence-form-elliptic-equation.md) inequality uses the sign convention $Lu\leq\operatorname{div}F+g$. For instance, the coefficient dependence can be expressed using

$$
R^{1-n/q}(\|b\|_{L^q(B_{2R})}+\|c\|_{L^q(B_{2R})}),\qquad R^{2-2n/q}\|d\|_{L^{q/2}(B_{2R})}.
$$

Thus one may use the same $p,C$ on all sufficiently small balls when the global coefficient norms and [uniform ellipticity](../../../../../../uniformly-elliptic-operator.md) bounds are fixed. The nonnegativity condition is essential to this formulation; a signed [weak supersolution](../../../../../../weak-supersolution-of-a-divergence-form-elliptic-equation.md) may first be shifted, with the resulting change in its forcing included. As usual, supremum and infimum statements for functions in a [Sobolev space](../../../../../../sobolev-space-split.md) mean [essential suprema](../../../../../../essential-supremum.md) and [essential infima](../../../../../../essential-infimum.md). The standard multidimensional statement uses $n\geq2$, so $q/2>1$. In dimension one the analogous formulation requires $q\geq2$; the printed restriction $q>n$ alone would allow $q/2<1$, which does not suffice. To see the obstruction, smooth the nonnegative capped function $\min\{1,|x|/\varepsilon\}$ by a [mollifier](../../../../../../mollifier.md) of width $\tau$. Its positive second derivative is a bump of mass $2/\varepsilon$ and has $L^{q/2}$ size of order $\varepsilon^{-1}\tau^{2/q-1}$. For fixed $\varepsilon$ and $1<q<2$, this size and the minimum both tend to zero as $\tau\downarrow0$, whereas the average on a fixed larger interval stays positive. Thus the [Weak Harnack inequality](../../../../../../weak-harnack-inequality.md) cannot have the displayed uniform forcing bound in that range. Shrinking $\varepsilon$ and choosing $\tau$ still smaller likewise defeats a uniform Hölder estimate based on that norm alone.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
