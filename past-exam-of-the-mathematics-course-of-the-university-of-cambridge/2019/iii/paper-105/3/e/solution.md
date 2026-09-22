<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Assume $0<\varepsilon<1$ and set

$$
a=1-\varepsilon,
\qquad
S_\varepsilon=\operatorname{artanh}(a)
=\frac12\log\frac{2-\varepsilon}{\varepsilon}.
$$

The [travel-time coordinate for a one-dimensional variable-speed wave equation](../../../../../../travel-time-coordinate-for-a-one-dimensional-variable-speed-wave-equation.md)

$$
s=\operatorname{artanh}y
$$

sends the initial interval $I_\varepsilon=(-a,a)$ to $(-S_\varepsilon,S_\varepsilon)$. By the [characteristic curves for speed one minus y squared](../../../../../../characteristic-curves-for-speed-one-minus-y-squared.md), the two characteristic coordinates are $s-x$ and $s+x$. The [finite propagation speed](../../../../../../finite-propagation-speed.md) and uniqueness theorem for [hyperbolic partial differential equations](../../../../../../hyperbolic-partial-differential-equation.md) therefore give the maximal characteristic diamond

$$
\boxed{D_\varepsilon
=\left\{(x,y):|x|+|\operatorname{artanh}y|<S_\varepsilon\right\}.}
$$

Equivalently,

$$
D_\varepsilon
=\left\{(x,y):|x|<S_\varepsilon,
\ |y|<\tanh(S_\varepsilon-|x|)\right\}.
$$

In the $(x,s)$ plane this is a diamond with vertices $(0,\pm S_\varepsilon)$ and $(\pm S_\varepsilon,0)$; transforming back bends its four sides into the characteristic curves found in part 3(c). Beyond any one of those sides, a point's backward characteristics meet $x=0$ outside $I_\varepsilon$, where no [Cauchy data](../../../../../../cauchy-data.md) were prescribed, so uniqueness cannot be extended farther.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
