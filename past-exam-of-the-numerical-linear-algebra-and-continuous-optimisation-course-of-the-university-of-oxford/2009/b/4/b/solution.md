<h1 id="b/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [line search](../../../../../line-search.md) chooses a positive [step size](../../../../../step-size.md) giving useful decrease along the chosen direction. Fix $\sigma,\beta\in(0,1)$ and a trial step $\bar\alpha>0$. The [Armijo condition](../../../../../armijo-condition.md) is

$$
\boxed{f(x+\alpha s)\leq f(x)+\sigma\alpha\nabla f(x)^Ts.}
$$

The [backtracking line search](../../../../../backtracking-line-search.md) tests $\bar\alpha,\beta\bar\alpha,\beta^2\bar\alpha,\ldots$ and takes the first accepted value. A [Lipschitz gradient](../../../../../lipschitz-gradient.md) has $\|\nabla f(y)-\nabla f(x)\|_2\leq L\|y-x\|_2$ with a constant $L$ independent of $x,y$.

Integrating the [gradient](../../../../../gradient.md) along a segment gives the [descent lemma](../../../../../descent-lemma.md)

$$
f(x+\alpha s)\leq f(x)+\alpha g^Ts+\frac L2\alpha^2\|s\|_2^2.
$$

For $s=-g$, every $0<\alpha\leq\tau=2(1-\sigma)/L$ satisfies the [Armijo condition](../../../../../armijo-condition.md). Thus backtracking terminates. If the trial step is accepted, $\alpha=\bar\alpha$; otherwise the immediately preceding step $\alpha/\beta$ failed, so it exceeded $\tau$. Consequently

$$
\boxed{\alpha\geq c=\min\{\bar\alpha,\,2\beta(1-\sigma)/L\}>0.}
$$

The same global Lipschitz constant and fixed search parameters make $c$ independent of $x$. If $g=0$, the zero direction passes the first test. If $L=0$, the gradient is constant and the first test passes, so take $c=\bar\alpha$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
