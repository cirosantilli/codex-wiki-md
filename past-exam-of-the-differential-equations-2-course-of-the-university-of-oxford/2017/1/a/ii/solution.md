<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Differentiate the [Wronskian](../../../../../wronskian.md) using the [product rule](../../../../../product-rule.md) and substitute the common [homogeneous linear differential equation](../../../../../homogeneous-linear-differential-equation.md):

$$
\begin{aligned}
W'&=(y_1y_2'-y_1'y_2)'=y_1y_2''-y_1''y_2\\
&=y_1(-py_2'-qy_2)-(-py_1'-qy_1)y_2=-pW.
\end{aligned}
$$

Multiplying this first-order equation by the [integrating factor](../../../../../integrating-factor.md) $\exp(\int_{x_0}^x p(t)\,dt)$ and integrating gives [Abel's identity](../../../../../abel-s-identity.md):

$$
\boxed{W(x)=W(x_0)\exp\!\left(-\int_{x_0}^x p(t)\,dt\right).}
$$

The exponential factor is finite and nonzero for every $x$ in the given [interval](../../../../../interval-mathematics.md), because $p$ is continuous on the compact interval between $x_0$ and $x$. Hence $W(x_0)\ne0$ implies $W(x)\ne0$ everywhere in that interval. Using an integrating factor avoids dividing by $W$, which would assume the conclusion.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
