<h1 id="b/6/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Suppress the iteration subscript. From the quadratic subproblem, $As=-c$ and $g=-Bs+A^Ty$. Therefore

$$
\begin{aligned}
\nabla\Phi(x,\mu)^Ts
&=g^Ts+\mu^{-1}\sum_i c_i^{p-1}(As)_i\\
&=-s^TBs-c^Ty-\mu^{-1}\|c\|_p^p.
\end{aligned}
$$

When $|c^Ty|>0$, the stated bound on $\mu$ makes $\mu^{-1}\|c\|_p^p\geq|c^Ty|$. Consequently

$$
\boxed{\nabla\Phi(x,\mu)^Ts\leq-s^TBs<0\quad\text{if }s\ne0,}
$$

using positive definiteness of $B$. Thus every nonzero such SQP step is a [descent direction](../../../../../descent-direction.md) for the penalty function. If $c^Ty=0$, the quotient bound is unnecessary and the same conclusion follows for every $\mu>0$. A zero step has zero directional derivative and is not a strict [descent direction](../../../../../descent-direction.md); it corresponds to an already feasible stationary point. This nonzero-step qualification is implicit in the requested conclusion.

## ↑ Ancestors (13)

1. [V](../v.md)
2. [6](../../6.md)
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
