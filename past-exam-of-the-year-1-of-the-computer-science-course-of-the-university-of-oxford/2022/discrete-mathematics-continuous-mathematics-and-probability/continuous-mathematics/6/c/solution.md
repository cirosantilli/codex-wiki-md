<h1 id="continuous-mathematics/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the equality-constrained [minimization problem](../../../../../../minimization-problem.md), $y=8/x$ and $x\ne0$. Put $t=x^2>0$. The restricted objective is

$$
f(x,8/x)=t^2+\frac{128}{t}-28=:F(t),\qquad F'(t)=2t-\frac{128}{t^2}.
$$

The only zero has $t^3=64$, so $t=4$. Since $F''(t)=2+256/t^3>0$, the [second-derivative criterion for convexity](../../../../../../second-derivative-criterion-for-convexity.md) proves a unique minimizing $t$. Consequently **the equality constraint has minimizers $(2,4)$ and $(-2,-4)$, with minimum $20$**.

For the inequality-constrained [minimization problem](../../../../../../minimization-problem.md), the identity $f=(x^2-1)^2+2(y-x)^2+3$ supplies the universal lower bound $3$. Both equality points for that bound, $(1,1)$ and $(-1,-1)$, satisfy $xy=1\le8$. Hence **the inequality constraint has exactly these two minimizers, with minimum $3$**.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [Continuous mathematics](../../../continuous-mathematics.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
