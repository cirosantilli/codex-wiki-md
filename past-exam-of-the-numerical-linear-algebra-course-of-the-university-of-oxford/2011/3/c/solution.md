<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Nonzero [vectors](../../../../vector.md) $p_1,\ldots,p_k$ are [conjugate directions](../../../../conjugate-direction.md) with respect to $A$ when $p_i^TAp_j=0$ for $i\ne j$. They are [linearly independent](../../../../linear-independence.md): if $\sum_i c_ip_i=0$, multiplication by $p_j^TA$ gives $c_jp_j^TAp_j=0$, hence $c_j=0$ by [positive definiteness](../../../../positive-definiteness.md). There are consequently at most $n$ such directions.

The [finite termination of conjugate directions](../../../../finite-termination-of-conjugate-directions.md) follows from the residual orthogonality maintained by the exact line minimizations. At step $j$,

$$
r_{j+1}=r_j-\alpha_jAp_j,\qquad p_j^Tr_{j+1}=0.
$$

For $i<j$, conjugacy gives $p_i^Tr_{j+1}=p_i^Tr_j$. By [mathematical induction](../../../../mathematical-induction.md), $r_{j+1}$ is [orthogonal](../../../../orthogonal-vectors.md) to every $p_1,\ldots,p_j$. After $n$ nonzero conjugate directions they form a [basis](../../../../basis.md) of $\mathbb R^n$, forcing $r_{n+1}=0$. Thus **the method reaches $Ax=b$ in at most $n$ steps**, and [positive definiteness](../../../../positive-definiteness.md) makes that solution unique. The claim is in exact arithmetic; rounding errors need not preserve exact conjugacy.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the numerical linear algebra course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra course of the University of Oxford](../../../../numerical-linear-algebra-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
