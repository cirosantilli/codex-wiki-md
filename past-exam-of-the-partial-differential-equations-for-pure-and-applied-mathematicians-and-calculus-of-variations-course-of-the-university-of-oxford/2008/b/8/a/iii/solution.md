<h1 id="b/8/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**The [compactness](../../../../../../compact-space.md) conclusion justified by the hypotheses is $u\in W^{1,1}$ with the prescribed traces; the printed claim $u\in W^{1,\infty}$ needs additional regularity.** Define

$$
u(x)=\alpha+\int_a^xv(t)dt.
$$

Then $u\in W^{1,1}$ and $u'=v$. Weak $L^1$ convergence tested against $\mathbf1_{(a,x)}$ gives $u_{j_k}(x)\to u(x)$ for every $x$, including the endpoint trace at $b$. [Uniform integrability](../../../../../../uniform-integrability.md) of the derivatives makes the functions equicontinuous: their increment over an interval is bounded by the integral of $|u_j'|$ on that interval, uniformly small for short intervals. Their fixed initial trace and common derivative $L^1$ bound also make them uniformly bounded. The [Arzelà-Ascoli theorem](../../../../../../arzela-ascoli-theorem.md) therefore upgrades the convergence to [uniform convergence](../../../../../../uniform-convergence.md), and in particular

$$
\boxed{u_{j_k}\to u\text{ in }L^1(a,b),\qquad u'=v,\quad u(a)=\alpha,\ u(b)=\beta.}
$$

[Uniform integrability](../../../../../../uniform-integrability.md) does not bound the derivative in $L^\infty$. The natural compact class here is absolutely continuous functions, rather than [Lipschitz functions](../../../../../../lipschitz-continuity.md). This distinction can affect attainment: smooth strictly convex superlinear integrands can have non-Lipschitz minimizing limits, so it is not repaired merely by adding [convexity](../../../../../../convex-function.md) in the last variable. If one additionally has a uniform Lipschitz bound on the [minimizing sequence](../../../../../../minimizing-sequence.md), weak testing on measurable subsets passes that bound to $v$ and proves the printed $u\in\mathcal A$. Alternatively one can formulate the direct method from the outset in the fixed-trace $W^{1,1}$ class. The proof above gives all the asserted convergence and trace conclusions without assuming the missing bound.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [8](../../../8.md)
4. [B](../../../../b.md)
5. [2008](../../../../../2008-split.md)
6. [Past exam of the partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../../split.md)
7. [Partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../../../partial-differential-equations-for-pure-and-applied-mathematicians-and-calculus-of-variations-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
