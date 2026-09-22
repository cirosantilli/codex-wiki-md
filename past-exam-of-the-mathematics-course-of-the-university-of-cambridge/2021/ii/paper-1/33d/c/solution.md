<h1 id="33d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

When $u$ is independent of $y$ and $z=x+iy$,

$$
\partial_z=\partial_{\bar z}=\frac12\frac d{dx}.
$$

Put

$$
L=U-V,\qquad M=U+V.
$$

The zero-curvature equation becomes

$$
\frac12L_x+[U,V]=0.
$$

Since

$$
[M,L]=[U+V,U-V]=-2[U,V],
$$

we obtain the [Isospectral Lax equation](../../../../../../isospectral-lax-equation.md)

$$
\boxed{L_x=[M,L]}.
$$

Therefore, for every positive integer $n$, the cyclic property of the [matrix trace](../../../../../../matrix-trace.md) gives

$$
\begin{aligned}
\frac d{dx}\operatorname{tr}(L^n)
&=n\operatorname{tr}(L^{n-1}[M,L])\\
&=n\operatorname{tr}(L^{n-1}ML-ML^n)=0.
\end{aligned}
$$

These are the [trace invariants of a Lax equation](../../../../../../trace-invariants-of-a-lax-equation.md).

The PDE from part (b) reduces to

$$
\frac14u_{xx}=\frac12\sinh(2u).
$$

With $\phi=2u$, this is

$$
\phi''=4\sinh\phi.
$$

To extract a nontrivial invariant, use $n=2$. Writing $p=u_x$, direct multiplication gives

$$
\operatorname{tr}(L^2)
=\frac12\left[
p^2+\lambda^2+\lambda^{-2}-2\cosh(2u)
\right].
$$

The terms involving $\lambda$ are constant, and $p=\phi'/2$. Hence

$$
\boxed{
\frac12(\phi')^2-4\cosh\phi=C
}
$$

is a [first integral](../../../../../../first-integral.md). Direct differentiation verifies it:

$$
\boxed{\frac d{dx}
\left[\frac12(\phi')^2-4\cosh\phi\right]
=\phi'(\phi''-4\sinh\phi)=0.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [33D](../../33d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
