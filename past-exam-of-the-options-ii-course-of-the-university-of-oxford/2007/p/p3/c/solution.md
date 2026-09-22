<h1 id="p/p3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the corrected interpolant from part (a). The error has $e(x_i)=e'(x_i)=0$, and the chosen auxiliary function has $\phi(x_i)=\phi'(x_i)=0$ as well as $\phi(x)=0$. There are $n+2$ distinct zeros of $\phi$: all the nodes and the additional evaluation point. [Rolle's theorem](../../../../../rolle-theorem.md) supplies $n+1$ zeros of $\phi'$ between these ordered zeros. Together with its $n+1$ nodal zeros, this gives $2n+2$ distinct derivative zeros. Repeated Rolle applications therefore give an interior $\xi$ such that $\phi^{(2n+2)}(\xi)=0$.

**The extra claim that $x$ itself must be a zero of $\phi'$ is false.** For nodes zero and one and $f(t)=t^5$, the Hermite interpolant is $3t^3-2t^2$, so $e(t)=t^2(t-1)^2(t+2)$. The auxiliary function is then $\phi(t)=t^2(t-1)^2(t-x)$, and $\phi'(x)=x^2(x-1)^2\ne0$ at any interior evaluation point. The corrected zero count above is all that is needed.

Since $h$ has degree at most $2n+1$ and $\pi^2$ is monic of degree $2n+2$, differentiating the auxiliary function at the supplied $\xi$ gives

$$
0=f^{(2n+2)}(\xi)-\frac{e(x)}{\pi(x)^2}(2n+2)!.
$$

Hence

$$
\boxed{e(x)=\pi(x)^2\frac{f^{(2n+2)}(\xi)}{(2n+2)!}}.
$$

At interpolation nodes the error and the prefactor are zero, so the formula remains valid there as well.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [P3](../../p3.md)
3. [P](../../../p.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
