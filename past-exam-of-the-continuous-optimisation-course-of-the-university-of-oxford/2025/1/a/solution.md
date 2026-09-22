<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix an iteration and abbreviate $x=x^k$, $s=s^k$, $d=\nabla f(x)^Ts$. Since $s$ is a [descent direction](../../../../descent-direction.md), $d<0$. The [directional derivative](../../../../directional-derivative.md) gives

$$
f(x+\alpha s)-f(x)-\beta_1\alpha d=(1-\beta_1)\alpha d+o(\alpha).
$$

Choose $\bar\alpha>0$ so that $|o(\alpha)|\leq\tfrac12(1-\beta_1)(-d)\alpha$ for $0<\alpha\leq\bar\alpha$. Then

$$
f(x+\alpha s)-f(x)-\beta_1\alpha d\leq\tfrac12(1-\beta_1)\alpha d<0.
$$

This is the [Armijo condition](../../../../armijo-condition.md) for every such positive [step size](../../../../step-size.md), and $\alpha=0$ gives equality. In particular, a [backtracking line search](../../../../backtracking-line-search.md) terminates after finitely many reductions.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the continuous optimisation course of the University of Oxford](../../../split.md)
5. [Continuous optimisation course of the University of Oxford](../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
