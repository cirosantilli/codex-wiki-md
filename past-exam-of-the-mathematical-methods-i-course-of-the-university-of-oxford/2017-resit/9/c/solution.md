<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With a fixed [unit normal](../../../../unit-normal.md) $n$, the [Householder reflection](../../../../householder-transformation.md) is $P=I-2nn^T$. It is a [linear map](../../../../linear-map.md) because both the identity and the map $v\mapsto n(n^Tv)$ are linear. Decompose $v=v_\parallel+v_\perp$, where $v_\perp=(n\cdot v)n$ and $v_\parallel\cdot n=0$. Then

$$
Pv=v_\parallel-v_\perp.
$$

Thus the tangential component is unchanged and the normal component reverses. Its norm and absolute normal component are preserved, proving equality of the physical incidence and reflection angles measured against the appropriate normal. Angles of the incident and reflected _directed vectors_ to one fixed oriented normal are instead supplementary; equality uses the conventional acute angle to the normal line, or reverses the incident direction.

Since $(nn^T)^2=nn^T$, direct multiplication gives $P^2=I$. Every [eigenvalue](../../../../eigenvalue.md) therefore satisfies $\lambda^2=1$. More specifically, the tangent plane is the $+1$ [eigenspace](../../../../eigenspace.md) and the normal line the $-1$ [eigenspace](../../../../eigenspace.md). In the stated [orthonormal basis](../../../../orthonormal-basis.md), with the first two vectors tangent to the plane,

$$
\boxed{[P]_{\{e_1,e_2,n\}}=\operatorname{diag}(1,1,-1).}
$$

This also proves both signs occur, rather than merely showing that any eigenvalue must belong to $\{+1,-1\}$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [9](../../9.md)
3. [2017 resit](../../../2017-resit-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
