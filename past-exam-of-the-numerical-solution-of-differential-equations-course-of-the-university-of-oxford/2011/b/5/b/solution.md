<h1 id="b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Replace $L_h$ by $\boxed{\widetilde L_h=L_h+I}$. At a positive interior maximum $v>0$, the neighbour average is no larger than $v$, so $(\widetilde L_h\phi)_{jk}\geq v>0$. Thus $\widetilde L_h\phi\leq0$ cannot have such an interior maximum. The positive-maximum form of the [discrete maximum principle](../../../../../discrete-maximum-principle.md) therefore remains valid:

$$
\max\phi\leq\max(0,\max_{\partial\Omega_h}\phi).
$$

With $e=u|_{\Omega_h}-U$ the error equation is $\widetilde L_he=\tau$, where $\tau=O(h^2)$ under the preceding regularity assumptions. Since $\widetilde L_hB=1+B\geq1$ for the same [Discrete Poisson barrier on a square](../../../../../discrete-poisson-barrier-on-a-square.md), the comparison functions $\pm e-\|\tau\|_\infty B$ prove

$$
\boxed{|e_{jk}|\leq\tfrac18\|\tau\|_\infty=O(h^2).}
$$

There is **no loss of uniqueness**: apply the positive-maximum argument to both signs of a homogeneous discrete solution. The continuous [weak formulation](../../../../../weak-formulation.md) also has the [coercive bilinear form](../../../../../coercive-bilinear-form.md) $\int_\Omega(|\nabla v|^2+v^2)$, so the added positive reaction term strengthens its positive energy.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the numerical solution of differential equations course of the University of Oxford](../../../../split.md)
6. [Numerical solution of differential equations course of the University of Oxford](../../../../../numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
