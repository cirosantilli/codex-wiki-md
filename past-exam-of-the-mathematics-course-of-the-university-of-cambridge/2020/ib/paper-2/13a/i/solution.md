<h1 id="13a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let

$$
u(x)=J_0(\alpha x),
\qquad
v(x)=J_0(\beta x).
$$

Their [Bessel equations](../../../../../../bessel-differential-equation.md) in self-adjoint form are

$$
(xu')'+\alpha^2xu=0,
\qquad
(xv')'+\beta^2xv=0.
$$

Multiply the first by $v$, the second by $u$, subtract, and integrate. The left side becomes a boundary term:

$$
\left[x(vu'-uv')\right]_0^1
+(\alpha^2-\beta^2)\int_0^1uvx\,dx=0.
$$

Regularity at zero makes the lower boundary term vanish, while

$$
u'(1)=\alpha J_0'(\alpha),
\qquad
v'(1)=\beta J_0'(\beta).
$$

Therefore

$$
\boxed{
\int_0^1J_0(\alpha x)J_0(\beta x)x\,dx
=\frac{\beta J_0(\alpha)J_0'(\beta)
-\alpha J_0(\beta)J_0'(\alpha)}
{\alpha^2-\beta^2}}.
$$

If $\alpha=\gamma_k$ and $\beta=\gamma_\ell$ with $k\ne\ell$, both endpoint values of $J_0$ vanish, so the integral is zero. This is the weighted [orthogonality](../../../../../../orthogonal-vectors.md) of distinct eigenfunctions in a [Sturm-Liouville problem](../../../../../../sturm-liouville-problem.md). For the norm, hold $\alpha=\gamma_k$ and let $\beta\to\gamma_k$. Since

$$
J_0(\beta)=J_0'(\gamma_k)(\beta-\gamma_k)
+o(\beta-\gamma_k),
$$

the quotient tends to

$$
\boxed{\int_0^1J_0(\gamma_kx)^2x\,dx
=\frac12J_0'(\gamma_k)^2}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [13A](../../13a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
