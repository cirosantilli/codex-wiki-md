<h1 id="2/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $J:C([0,1])\to L^1(0,1)$ send a [continuous function](../../../../../continuous-function.md) to its [almost everywhere](../../../../../almost-everywhere.md) equivalence class. The domain with the [supremum norm](../../../../../supremum-norm.md) and the target with the [L1 norm](../../../../../l1-norm.md) are [Banach spaces](../../../../../banach-space-split.md), and

$$
\|Jf\|_{L^1}=\int_0^1|f(t)|\,dt\leq\|f\|_\infty.
$$

Thus $J$ is a [bounded linear operator](../../../../../continuous-linear-operator.md), and the requested [vector subspace](../../../../../vector-subspace.md) is $J(C([0,1]))$.

To show this [image of a linear map](../../../../../image-of-a-linear-map.md) is not closed, consider the [continuous functions](../../../../../continuous-function.md)

$$
f_n(t)=\min\{1,\max\{0,n(t-1/2)\}\}\qquad(n\geq2)
$$

and $g=\mathbf1_{(1/2,1)}$. Their [L1 norm](../../../../../l1-norm.md) difference is the area of one triangle:

$$
\|Jf_n-g\|_{L^1}=\int_{1/2}^{1/2+1/n}\bigl(1-n(t-1/2)\bigr)\,dt=\frac1{2n}\longrightarrow0.
$$

But $g$ has no [continuous function](../../../../../continuous-function.md) representative. Indeed, a [continuous function](../../../../../continuous-function.md) equal to zero [almost everywhere](../../../../../almost-everywhere.md) on $(0,1/2)$ must be identically zero there: any nonzero value would persist on an open interval of positive [Lebesgue measure](../../../../../lebesgue-measure.md). Likewise any continuous representative would be identically one on $(1/2,1)$. Continuity at $1/2$ makes these requirements incompatible. Therefore $g\notin J(C([0,1]))$, although it lies in its [closure](../../../../../closure-topology.md).

The preceding [operator range category dichotomy](../../../../../operator-range-category-dichotomy.md) proves [continuous functions are meagre in L1](../../../../../continuous-functions-are-meagre-in-l1.md):

$$
\boxed{J(C([0,1]))\text{ is of the first category in }L^1(0,1).}
$$

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analysis II course of the University of Oxford](../../../../split.md)
6. [Functional analysis II course of the University of Oxford](../../../../../functional-analysis-ii-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
