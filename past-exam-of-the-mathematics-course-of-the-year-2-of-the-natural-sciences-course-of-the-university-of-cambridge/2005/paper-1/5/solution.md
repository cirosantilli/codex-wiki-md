<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [unitary matrix](../../../../unitary-matrix.md) satisfies $U^\dagger U=I$ over the complex numbers; a real [orthogonal matrix](../../../../orthogonal-matrix.md) satisfies $Q^TQ=I$. Their inverses are their conjugate transposes and transposes, respectively.

With $d=-a$, the coordinate $e_2=(0,1,0)$ has [eigenvalue](../../../../eigenvalue.md) $c$. In the $x,z$ plane, the [traceless symmetric two-by-two matrix](../../../../traceless-symmetric-two-by-two-matrix.md) has eigenvalues $\pm s$, where $s=\sqrt{a^2+b^2}$. If $s>0$, choose $\theta$ with $\cos2\theta=a/s$ and $\sin2\theta=b/s$. Then an [orthonormal eigenbasis](../../../../orthonormal-eigenbasis.md) is

$$
\boxed{\lambda_+=s:\ v_+=(\cos\theta,0,\sin\theta),\quad\lambda_-=-s:\ v_-=(-\sin\theta,0,\cos\theta),\quad\lambda_2=c:\ e_2.}
$$

If $c$ equals $s$ or $-s$, the corresponding [eigenspace](../../../../eigenspace.md) is the span of the two listed vectors with that eigenvalue. If $s=0$, then $a=b=0$, the $x,z$ plane is the zero eigenspace, and $e_2$ retains eigenvalue $c$; if also $c=0$, every vector belongs to the zero eigenspace. This includes the degenerate cases that a division by $b$ would miss.

For the [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md), take $b\ne0$ and remove the [orthogonal projection](../../../../orthogonal-projection.md) of $a$ along $b$. Positivity of the squared norm gives

$$
0\leq\left\|a-b\frac{\langle b,a\rangle}{\|b\|^2}\right\|^2=\|a\|^2-\frac{|\langle b,a\rangle|^2}{\|b\|^2}.
$$

Multiplication by $\|b\|^2$ and square roots prove $|\langle a,b\rangle|\leq\|a\|\|b\|$; the case $b=0$ is immediate. Equality means linear dependence. Therefore

$$
\|a+b\|^2=\|a\|^2+\|b\|^2+2\operatorname{Re}\langle a,b\rangle\leq\|a\|^2+\|b\|^2+2\|a\|\|b\|=(\|a\|+\|b\|)^2.
$$

Taking the nonnegative square root proves the [triangle inequality](../../../../triangle-inequality.md).

## ↑ Ancestors (12)

1. [5](../5.md)
2. [Paper 1](../../paper-1-split.md)
3. [2005](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
