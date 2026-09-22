<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [quadratic function](../../../../quadratic-function.md), write $r_j=b-Ax_j$ and restrict to the full line $x_j+\alpha p_j$. [Symmetry](../../../../symmetry-physics.md) of $A$ gives

$$
f(x_j+\alpha p_j)=f(x_j)-\alpha p_j^Tr_j+\frac{\alpha^2}{2}p_j^TAp_j.
$$

The coefficient $p_j^TAp_j$ is positive by [positive definiteness](../../../../positive-definiteness.md) and $p_j\ne0$. The unique [minimizer](../../../../global-minimizer.md) is therefore

$$
\boxed{\alpha_j=\frac{p_j^Tr_j}{p_j^TAp_j},\qquad x_{j+1}=x_j+\alpha_jp_j.}
$$

[Quadratic minimization along a line](../../../../quadratic-minimization-along-a-line.md) also gives the exact change

$$
f(x_{j+1})-f(x_j)=-\frac{(p_j^Tr_j)^2}{2p_j^TAp_j}.
$$

Thus **strict decrease holds exactly when $p_j^Tr_j\ne0$**. The search is over the whole line, so $\alpha_j$ can be negative; a positive [step size](../../../../step-size.md) would require the additional [descent direction](../../../../descent-direction.md) condition $p_j^Tr_j>0$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the numerical linear algebra course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra course of the University of Oxford](../../../../numerical-linear-algebra-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
