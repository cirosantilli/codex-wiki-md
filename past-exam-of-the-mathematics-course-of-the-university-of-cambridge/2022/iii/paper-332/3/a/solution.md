<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Newtonian shallow-ice flux](../../../../../../newtonian-shallow-ice-flux.md) on the flat bed is

$$
q=-\frac{gh^3}{3\nu}h_x,
$$

so [mass conservation](../../../../../../mass-conservation.md) gives

$$
\boxed{
h_t=\frac g{3\nu}(h^3h_x)_x+A\quad(0<x<x_s),
\qquad
h_t=\frac g{3\nu}(h^3h_x)_x-A\quad(x_s<x<x_N).}
$$

At the [ice divide](../../../../../../ice-divide.md), symmetry gives $h_x(0,t)=q(0,t)=0$. At the terminus, $h(x_N,t)=0$ and the moving-front mass balance applies; in a steady state $q(x_N)=0$. At the [snowline](../../../../../../snowline.md), $h(x_s,t)=h_s$ and both $h$ and $q$ are continuous, hence $h_x$ is continuous because $h_s>0$.

In a steady state, $q_x=A$ in the accumulation region and $q_x=-A$ in the ablation region. Therefore

$$
q=Ax\quad(0<x<x_s),
\qquad
q=A(x_N-x)\quad(x_s<x<x_N).
$$

Flux continuity gives $x_N=2x_s$. Integrating the flux law gives the piecewise shape

$$
\boxed{
h^4=h_0^4-\frac{6\nu A}{g}x^2
\quad(0\leq x\leq x_s),}
$$



$$
\boxed{
h^4=\frac{6\nu A}{g}(x_N-x)^2
\quad(x_s\leq x\leq x_N).}
$$

Matching $h(x_s)=h_s$ yields

$$
\boxed{x_s=\left(\frac g{6\nu A}\right)^{1/2}h_s^2,
\qquad x_N=2x_s,
\qquad h_0=2^{1/4}h_s.}
$$

The largest surface slope is of order $\sqrt{\nu A/g}/h_s$, so the [shallow-ice approximation](../../../../../../shallow-ice-approximation.md) requires

$$
\boxed{A\ll\frac{gh_s^2}{\nu}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
