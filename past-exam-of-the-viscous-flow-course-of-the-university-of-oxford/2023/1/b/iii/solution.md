<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Subtract the particular [plane Poiseuille flow](../../../../../plane-poiseuille-flow.md) profile from the full [rectangular duct flow](../../../../../rectangular-duct-flow.md). The remainder is a [harmonic function](../../../../../harmonic-function.md):

$$
\begin{gathered}
w_2=w-w_1,\qquad w_{2,xx}+w_{2,yy}=0,\\
w_2(x,\pm b)=0,\qquad
w_2(\pm a,y)=-\frac G{2\mu}(b^2-y^2).
\end{gathered}
$$

The data are even in $x$ and $y$. The [boundary value problem](../../../../../boundary-value-problem-split.md) is unique: if two solutions differed by $v$, [Green's first identity](../../../../../green-s-first-identity.md) and the zero [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) would give

$$
\int_{-a}^{a}\int_{-b}^{b}|\nabla v|^2\,dy\,dx
=\int_{\partial\Omega}v\partial_n v\,ds-\int_\Omega v\nabla^2v\,dA=0.
$$

Thus $v$ is constant, and its zero boundary values force $v=0$. Reflection of a solution in either coordinate axis therefore gives the same solution. We may seek even separated [eigenfunctions](../../../../../eigenfunction.md).

Use [separation of variables](../../../../../separation-of-variables.md) with

$$
k_n=\frac{(2n+1)\pi}{2b},\qquad
w_2(x,y)=\sum_{n=0}^{\infty}A_n
\frac{\cosh(k_nx)}{\cosh(k_na)}\cos(k_ny).
$$

Each summand solves the [Laplace equation](../../../../../laplace-equation.md), vanishes at $y=\pm b$, and has the required evenness. The [hyperbolic cosine](../../../../../hyperbolic-cosine.md) ratio equals one at either side wall. The functions $\cos(k_ny)$ have [orthogonality](../../../../../orthogonal-vectors.md) relation

$$
\int_{-b}^{b}\cos(k_ny)\cos(k_my)\,dy
=\begin{cases}b,&m=n,\\0,&m\ne n.\end{cases}
$$

They are the even [Dirichlet eigenfunctions](../../../../../dirichlet-eigenfunction.md) on $[-b,b]$, so their [Fourier series](../../../../../fourier-series-split.md) represents the even boundary data. Projecting that data onto the $n$th [eigenfunction](../../../../../eigenfunction.md) yields the [Fourier coefficient](../../../../../fourier-coefficient.md)

$$
A_n=-\frac{G}{2\mu b}\int_{-b}^{b}(b^2-y^2)\cos(k_ny)\,dy
=-\frac{16Gb^2}{\mu\pi^3}\frac{(-1)^n}{(2n+1)^3}.
$$

For completeness, two [integrations by parts](../../../../../integration-by-parts.md) give the [quadratic arch expansion in half-integer cosine modes](../../../../../quadratic-arch-expansion-in-half-integer-cosine-modes.md): the displayed [integral](../../../../../integral-split.md) is $4(-1)^n/k_n^3$, agreeing with the identity supplied in the paper.

Adding the particular solution gives

$$
\boxed{\begin{aligned}
w(x,y)&=\frac{G}{2\mu}(b^2-y^2)\\
&\quad-\frac{16Gb^2}{\mu\pi^3}\sum_{n=0}^{\infty}
\frac{(-1)^n}{(2n+1)^3}
\frac{\cosh(k_nx)}{\cosh(k_na)}\cos(k_ny),\\
k_n&=\frac{(2n+1)\pi}{2b}.
\end{aligned}}
$$

The coefficients are absolutely summable and the [hyperbolic cosine](../../../../../hyperbolic-cosine.md) ratio is at most one throughout the closed rectangle, giving [uniform convergence](../../../../../uniform-convergence.md) and the prescribed boundary values. On compact subsets of the interior, the [hyperbolic cosine](../../../../../hyperbolic-cosine.md) ratio supplies exponential decay in $n$, justifying differentiation of the [series](../../../../../series-mathematics.md) and the [Laplace equation](../../../../../laplace-equation.md). The side-wall correction slows the [plane Poiseuille flow](../../../../../plane-poiseuille-flow.md) enough to satisfy all four [no-slip boundary conditions](../../../../../no-slip-boundary-condition.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the viscous flow course of the University of Oxford](../../../../split.md)
6. [Viscous flow course of the University of Oxford](../../../../../viscous-flow-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
