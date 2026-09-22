<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

Introduce the vector $x=(t,y,y',\ldots,y^{(k-1)})\in\mathbb R^{k+1}$. Its autonomous [ordinary differential equation](../../../../../ordinary-differential-equation.md) is

$$
\dot x=(1,x_2,x_3,\ldots,x_k,g(x_0,x_1,\ldots,x_k)),
$$

where the coordinate indices start at zero. Appending the clock removes the explicit time dependence.

For a [vector field](../../../../../vector-field.md) with local existence and uniqueness, its [flow](../../../../../flow.md) $\phi_t(x)$ is the solution at elapsed time $t$ starting at $x$. The [uniqueness theorem for ordinary differential equations](../../../../../uniqueness-theorem-for-ordinary-differential-equations.md) gives $\phi_s(\phi_t(x))=\phi_{s+t}(x)$ whenever both sides are defined. The [orbit](../../../../../orbit-dynamical-system.md) is $O(x)=\{\phi_t(x):t\text{ lies in its maximal interval}\}$. For a forward-complete solution its [omega-limit set](../../../../../omega-limit-set.md) is

$$
\omega(x)=\bigcap_{T\ge0}\overline{\{\phi_t(x):t\ge T\}},
$$

equivalently the set of [limits](../../../../../limit-of-a-function.md) along sequences $t_n\to\infty$. A [homoclinic orbit](../../../../../homoclinic-orbit.md) is a nonconstant complete orbit approaching the same [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) as $t\to-\infty$ and $t\to\infty$. This last definition concerns a general autonomous system; the appended clock itself cannot approach an equilibrium.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
