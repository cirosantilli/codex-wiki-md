<h1 id="b/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [log-cosh obstacle variational inequality](../../../../../log-cosh-obstacle-variational-inequality.md), the admissible [set](../../../../../set-split.md) is convex: for any $v\in M$, $u+t(v-u)$ remains above the obstacle and in $H_0^1$ for $0\le t\le1$. Minimality and the right [derivative](../../../../../derivative.md) at zero therefore give

$$
\boxed{\int_\Omega\nabla u\cdot\nabla(v-u)+\tanh(u)(v-u)\,dx\ge0\qquad(v\in M).}
$$

The one-sided sign comes from admissibility, which permits motion toward every $v\in M$ but does not permit an arbitrary negative variation at a contact point.

Now fix $\phi\in C_c^\infty(D)$. Smoothness on $D$ and [continuity](../../../../../continuous-function.md) of the obstacle give a strictly positive minimum of $u-g$ on the [compact support](../../../../../compact-support.md) of $\phi$. Hence $u+t\phi$ is admissible for both signs of sufficiently small $t$. Applying the inequality to both variations yields

$$
\int_D\nabla u\cdot\nabla\phi+\tanh(u)\phi\,dx=0.
$$

[Integration by parts](../../../../../integration-by-parts.md) gives $-\Delta u+\tanh u=0$ distributionally on $D$, and smoothness makes it [pointwise](../../../../../pointwise-convergence.md). Thus

$$
\boxed{-\Delta u+\tanh u=0\quad\text{where }u>g.}
$$

On the contact [set](../../../../../set-split.md) the [variational inequality](../../../../../variational-inequality.md), rather than unrestricted stationarity, remains the governing statement. [Convexity](../../../../../convex-function.md) of the energy also makes the inequality sufficient for minimization; [strict monotonicity](../../../../../strictly-monotone-operator.md) implies at most one [minimizer](../../../../../global-minimizer.md), although existence was already stipulated in this part.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the methods of applied functional analysis course of the University of Oxford](../../../../split.md)
6. [Methods of applied functional analysis course of the University of Oxford](../../../../../methods-of-applied-functional-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
