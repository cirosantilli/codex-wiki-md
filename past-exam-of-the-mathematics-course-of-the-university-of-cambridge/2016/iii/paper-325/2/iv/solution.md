<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Here $L$-smooth means that $f$ is differentiable on the entire Euclidean space and has an $L$-[Lipschitz gradient](../../../../../../lipschitz-gradient.md), with $L>0$. Together with [convexity](../../../../../../convex-function.md), this implies **$1/L$-[cocoercivity](../../../../../../cocoercivity.md)**:

$$
\boxed{\langle\nabla f(u)-\nabla f(v),u-v\rangle\geq\frac1L\|\nabla f(u)-\nabla f(v)\|_2^2}.
$$

First, integration of the [Lipschitz gradient](../../../../../../lipschitz-gradient.md) along a line segment proves the [descent lemma](../../../../../../descent-lemma.md):

$$
f(w)\leq f(v)+\langle\nabla f(v),w-v\rangle+\frac L2\|w-v\|_2^2.
$$

Indeed, subtract the linear term and integrate $\langle\nabla f(v+t(w-v))-\nabla f(v),w-v\rangle$ for $0\leq t\leq1$; its absolute value is at most $Lt\|w-v\|_2^2$.

Fix $u$ and define $q(w)=f(w)-\langle\nabla f(u),w\rangle$. This is a [convex function](../../../../../../convex-function.md), has the same [Lipschitz gradient](../../../../../../lipschitz-gradient.md) constant, and $\nabla q(u)=0$, so $u$ is a global minimizer. Put $d=\nabla f(v)-\nabla f(u)=\nabla q(v)$. The [descent lemma](../../../../../../descent-lemma.md) at $v$ with $w=v-d/L$ gives

$$
q(u)\leq q(v-d/L)\leq q(v)-\frac1{2L}\|d\|_2^2.
$$

Therefore

$$
f(v)-f(u)-\langle\nabla f(u),v-u\rangle\geq\frac1{2L}\|\nabla f(v)-\nabla f(u)\|_2^2.
$$

Interchange $u,v$ and add the inequalities. The function values cancel, leaving the asserted [cocoercivity](../../../../../../cocoercivity.md). This is a proof of the [Baillon–Haddad theorem](../../../../../../baillon-haddad-theorem.md) without assuming a second derivative. [Convexity](../../../../../../convex-function.md) is essential: $f(u)=-\|u\|_2^2/2$ has a $1$-[Lipschitz gradient](../../../../../../lipschitz-gradient.md) but its gradient is not [cocoercive](../../../../../../cocoercivity.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 325](../../../paper-325-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
