<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Suppose for contradiction that $\|\widehat\theta(Z_{\gamma,\tau})\|_2\leq M$ uniformly in $\gamma,\tau$. Choose $\gamma>M+1$, so part d applies to every fitted value and gives $L(\widehat\theta)\geq\rho(\tau)$. For this fixed $\gamma$, part c gives the competing bound

$$
L(\theta_\gamma)
\leq h\rho\!\left(M_y+\gamma\max_i|x_{i1}|\right)+\lambda\gamma,
$$

which is independent of $\tau$. Since $\rho(\tau)\to\infty$, choose $\tau$ so that the lower bound exceeds this upper bound, contradicting optimality. Thus $n-h+1$ replacements can make the estimate unbounded, and

$$
\epsilon^*(Z,\widehat\theta)\leq\frac{n-h}{n}.
$$

Together with part b, the [replacement breakdown point](../../../../../../replacement-breakdown-point.md) is exactly $(n-h)/n$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
