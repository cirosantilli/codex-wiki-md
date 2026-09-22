<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $y\in\mathbb R^m$ and $\gamma\geq0$, define the [optimization Lagrangian](../../../../optimization-lagrangian.md)

$$
\mathcal L(x,y,\gamma)=c^Tx+y^T(b-Ax)+\gamma(x^TQx-1).
$$

The Lagrangian primal is

$$
\boxed{\inf_{x\in\mathbb R^n}\ \sup_{y\in\mathbb R^m,\,\gamma\geq0}
\mathcal L(x,y,\gamma).}
$$

For feasible $x$, the supremum is $c^Tx$: equality terms vanish and the nonpositive inequality term has maximum zero at $\gamma=0$. If $Ax\ne b$, scale $y$ in the direction $b-Ax$ to make the supremum infinite. If the inequality fails, send $\gamma\to\infty$. Thus the inner supremum is exactly the objective extended to $+\infty$ off the [feasible set](../../../../feasible-region.md). This proves equivalence with the original problem, including its infeasible case.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the continuous optimisation course of the University of Oxford](../../../split.md)
5. [Continuous optimisation course of the University of Oxford](../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
