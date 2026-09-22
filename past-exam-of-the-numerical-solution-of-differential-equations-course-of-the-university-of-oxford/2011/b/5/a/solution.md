<h1 id="b/5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The five-point equations for the [Poisson equation](../../../../../poisson-s-equation.md) are

$$
\boxed{(L_hU)_{jk}:=\frac{4U_{jk}-U_{j+1,k}-U_{j-1,k}-U_{j,k+1}-U_{j,k-1}}{h^2}=f(x_j,y_k),\quad1\leq j,k\leq n,}
$$

with prescribed boundary values. If $L_h\phi\leq0$, an interior maximal value is at most the average of its four neighbours. Since no neighbour exceeds the maximum, equality forces all four to equal it. Repeating along adjacent nodes propagates that value to the boundary. Thus the [discrete maximum principle](../../../../../discrete-maximum-principle.md) gives $\max\phi\leq\max_{\partial\Omega_h}\phi$, in particular the usual positive-maximum bound with zero included.

For an $O(h^2)$ error estimate assume the exact solution has bounded continuous fourth partial [derivatives](../../../../../derivative.md) up to the boundary. The [local truncation error](../../../../../local-truncation-error.md) $\tau=L_hu-f$ then satisfies $\|\tau\|_\infty\leq Ch^2$ by the [Taylor theorem](../../../../../taylor-s-theorem.md). Put $e=u|_{\Omega_h}-U$, so $L_he=\tau$ and $e=0$ on boundary nodes. The [Discrete Poisson barrier on a square](../../../../../discrete-poisson-barrier-on-a-square.md)

$$
B(x,y)=\frac{x(1-x)+y(1-y)}4
$$

satisfies $L_hB=1$ exactly, $B\geq0$ on the grid boundary, and $B\leq1/8$. Set $\varepsilon=\|\tau\|_\infty$. Then $L_h(\pm e-\varepsilon B)\leq0$, with nonpositive boundary values. Applying the [discrete maximum principle](../../../../../discrete-maximum-principle.md) twice gives

$$
\boxed{|e_{jk}|\leq\varepsilon B(x_j,y_k)\leq\frac18\|\tau\|_\infty=O(h^2).}
$$

For nonzero smooth [Dirichlet boundary data](../../../../../dirichlet-boundary-data.md) $g$, impose $U=g$ at the boundary nodes. The error still vanishes there, so **the same argument and order apply**, under the same fourth-derivative regularity of the exact solution. Smooth boundary values alone do not remove every possible corner-regularity issue.

## ↑ Ancestors (13)

1. [A](../a.md)
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
