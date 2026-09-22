<h1 id="16c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Here $b>0$ because $a=0$ and the two cost coefficients are not both zero. The interior [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) makes $V$ quadratic. Imposing each displayed pair of endpoint data and the distance constraint gives the following formal profiles and their costs:

$$
\begin{array}{c|c|c}
\text{choice}&V(t)&b\int_0^T\dot V^2\,dt\\ \hline
1&3Lt^2/T^3&12bL^2/T^3\\
2&6Lt(T-t)/T^3&12bL^2/T^3\\
3&3Lt(2T-t)/(2T^3)&3bL^2/T^3
\end{array}
$$

Thus **choice (3) is the best strategy**, and its true minimum cost is

$$
\boxed{E_{\min}=\frac{3bL^2}{T^3}.}
$$

The qualification from part (b) applies to row (1): its formal quadratic is not a minimizer with free terminal speed, since $\dot V(T)\ne0$. Row (2) is a genuine minimizer for its fixed zero terminal speed, and row (3) is the genuine free-terminal-speed minimizer, satisfying its natural condition $\dot V(T)=0$.

A direct lower bound makes the comparison rigorous. For every admissible speed with $V(0)=0$,

$$
L=\int_0^T(T-t)\dot V(t)\,dt,
$$

by [integration by parts](../../../../../../integration-by-parts.md). The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives $L^2\leq(T^3/3)\int_0^T\dot V^2\,dt$. Equality requires $\dot V$ to be proportional to $T-t$, giving exactly row (3). Row (1)'s zero initial acceleration excludes equality; however short initial layers, as in part (b), approach that same infimum. Hence choice (1) has infimum $3bL^2/T^3$ but does not attain it, while choice (3) does. This distinction resolves the boundary-condition issue in the printed minimization request.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [16C](../../16c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
