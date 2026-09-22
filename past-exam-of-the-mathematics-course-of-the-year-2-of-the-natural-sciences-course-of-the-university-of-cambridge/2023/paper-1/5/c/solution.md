<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The plane spanned by $u_1,v_1$ is an [invariant subspace](../../../../../invariant-subspace.md) for $M$, since

$$
Mu_1=\mu_1v_1,\qquad Mv_1=\frac1{\mu_1}M^2u_1=-\mu_1u_1.
$$

Its [orthogonal complement](../../../../../orthogonal-complement.md) is also invariant: for $w$ orthogonal to both, $u_1^TMw=-(Mu_1)^Tw=0$ and $v_1^TMw=-(Mv_1)^Tw=0$. The restriction of the real [symmetric matrix](../../../../../symmetric-matrix.md) $M^2$ to this nonempty complement therefore has a unit [eigenvector](../../../../../eigenvector.md) $u_2$, by the [spectral theorem for real symmetric matrices](../../../../../spectral-theorem-for-real-symmetric-matrices.md).

If its [eigenvalue](../../../../../eigenvalue.md) is $-\mu_2^2<0$, the argument in part (b) shows that $v_2=Mu_2/\mu_2$ is a unit [eigenvector](../../../../../eigenvector.md) orthogonal to $u_2$. It also lies in the same complement; explicitly,

$$
u_1^Tv_2=-\frac{\mu_1}{\mu_2}v_1^Tu_2=0,\qquad v_1^Tv_2=\frac{\mu_1}{\mu_2}u_1^Tu_2=0.
$$

Repeating the construction decomposes every negative [eigenspace](../../../../../eigenspace.md) into orthogonal pairs. The zero [eigenspace](../../../../../eigenspace.md) has dimension $n-2r$ for some number $r$ of pairs, and therefore has the same parity as $n$. This is the [paired eigenspaces of the square of a real skew-symmetric matrix](../../../../../paired-eigenspaces-of-the-square-of-a-real-skew-symmetric-matrix.md) property.

For $n=2m$, there can be $m$ distinct negative [eigenvalues](../../../../../eigenvalue.md) and no zero, or at most $m-1$ negative ones plus zero, because a nonempty zero [eigenspace](../../../../../eigenspace.md) has dimension at least two. For $n=2m+1$, there are at most $m$ distinct negative ones plus the mandatory zero. Hence

$$
\boxed{\text{maximum number of distinct eigenvalues of }M^2=\left\lceil\frac n2\right\rceil.}
$$

The bound is attained by skew two-by-two blocks with distinct positive parameters, adding one zero direction when $n$ is odd.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
