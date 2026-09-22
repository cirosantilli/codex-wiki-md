<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Remove the apparent singularity at $x=0$ by defining

$$
\phi(t,x)=\begin{cases}\sin(tx)/x,&x>0,\\t,&x=0.\end{cases}
$$

This is jointly continuous: write $\phi(t,x)=t\,\operatorname{sinc}(tx)$ using the [unnormalized sinc function](../../../../unnormalized-sinc-function.md), whose value at zero is one. Its [partial derivative](../../../../partial-derivative.md) in $t$ is

$$
\partial_t\phi(t,x)=\cos(tx)
$$

also at $x=0$, since there $\phi(t,0)=t$. This [partial derivative](../../../../partial-derivative.md) is jointly continuous on the whole strip.

The value at the single endpoint $x=0$ does not change a [Lebesgue integral](../../../../lebesgue-integral.md). Part (b), whose [dominated convergence](../../../../dominated-convergence-theorem.md) proof applies to $\phi$, therefore makes $g$ continuously differentiable on $[0,\infty)$, with a [right derivative](../../../../right-derivative.md) at zero, and

$$
g'(t)=\int_0^1\cos(tx)\,dx.
$$

For $t>0$, direct [integration](../../../../integral-split.md) gives

$$
\boxed{g'(t)=\frac{\sin t}{t},\qquad tg'(t)=\sin t.}
$$

At zero the same integral gives $\boxed{g'_+(0)=1}$, so no division by zero is required. Also $g(0)=0$. The [substitution rule](../../../../integration-by-substitution.md) $u=tx$ identifies $g(t)=\int_0^t\sin u/u\,du$ for $t>0$, the [sine integral](../../../../sine-integral.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the integration course of the University of Oxford](../../../split.md)
5. [Integration course of the University of Oxford](../../../../integration-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
