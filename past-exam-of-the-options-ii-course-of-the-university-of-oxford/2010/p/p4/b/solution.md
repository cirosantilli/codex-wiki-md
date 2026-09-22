<h1 id="p/p4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The intended orthogonal-[polynomial](../../../../../polynomial-split.md) convention is **$\deg p_k=k$**. An arbitrary [orthonormal basis](../../../../../orthonormal-basis.md) without this degree ordering does not satisfy the claim: permuting a standard [basis](../../../../../basis.md) can place the nonzero constant [polynomial](../../../../../polynomial-split.md) last, where it has no [roots](../../../../../root-of-a-root-system.md) rather than $n+1$. The following proof uses the required degree ordering.

It makes $p_k$ orthogonal to every [polynomial](../../../../../polynomial-split.md) of degree less than $k$, since $p_0,\ldots,p_{k-1}$ form a [basis](../../../../../basis.md) of that lower-degree space. Let $c_1,\ldots,c_r$ be the distinct [roots](../../../../../root-of-a-root-system.md) in $(a,b)$ at which $p_k$ changes sign, and put $q(x)=\prod_{j=1}^r(x-c_j)$, with $q=1$ if $r=0$. The product $p_kq$ has constant sign on $(a,b)$ except at its finitely many zeros: each sign change of $p_k$ is canceled by that of $q$.

If $r<k$, then $q$ has degree below $k$, so [orthogonality](../../../../../orthogonal-vectors.md) gives $\int_a^bp_kqw=0$. But a nonzero constant-sign continuous product against the positive weight has a nonzero integral, a contradiction. Thus $r\geq k$. Since $\deg p_k=k$, there are exactly $k$ such [roots](../../../../../root-of-a-root-system.md), all simple, with no additional endpoint [roots](../../../../../root-of-a-root-system.md). In particular

$$
\boxed{p_k\text{ has exactly }k\text{ distinct roots, all in }(a,b).}
$$

This also includes $k=0$, where the [polynomial](../../../../../polynomial-split.md) is nonzero constant and has no [roots](../../../../../root-of-a-root-system.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [P4](../../p4.md)
3. [P](../../../p.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
