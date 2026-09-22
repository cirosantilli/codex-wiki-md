<h1 id="b/7/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [backtracking line search](../../../../../backtracking-line-search.md) starts with $\alpha_{\mathrm{init}}>0$, tests the [Armijo condition](../../../../../armijo-condition.md), and repeatedly replaces a failed step by $\tau\alpha$, with fixed $\tau\in(0,1)$. It accepts the first step that passes. Backtracking makes an overambitious trial step small enough for a local linear model to predict the change reliably; part (ii) ensures finite termination. The [Armijo condition](../../../../../armijo-condition.md) guarantees a decrease of at least $-\alpha\beta g^Tp>0$ along a nonzero [descent direction](../../../../../descent-direction.md). Merely obtaining some decrease without this quantitative lower bound would not provide the convergence estimate in the following parts.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
