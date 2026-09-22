<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Using the [semidiscrete Fourier transform](../../../../semidiscrete-fourier-transform.md) from (b), the explicit scheme has [amplification factor](../../../../amplification-factor.md)

$$
G_E(\theta)=1-4a\mu\sin^2(\theta/2)-i\nu\sin\theta.
$$

Set $r=a\mu$ and $s=\sin^2(\theta/2)\in[0,1]$, so $\sin^2\theta=4s(1-s)$. Direct expansion gives

$$
|G_E|^2=(1-4rs)^2+4\nu^2s(1-s),\qquad
|G_E|^2-1=4s\left[(\nu^2-2r)+(4r^2-\nu^2)s\right].
$$

The expression in square brackets is an [affine function](../../../../affine-function.md) of $s$. At the two endpoints its values are

$$
\nu^2-2r\leq0,\qquad 4r^2-2r=2r(2r-1)\leq0,
$$

using precisely $\nu^2\leq2r\leq1$. Every intermediate value is a [convex combination](../../../../convex-combination.md) of these endpoints, so $|G_E|^2\leq1$ for every frequency. The [Parseval identity](../../../../parseval-identity.md) proves

$$
\boxed{\|U^m\|_{\ell_2}\leq\|U^0\|_{\ell_2}\quad(m\geq0),\qquad\nu^2\leq2a\mu\leq1.}
$$

Thus the scheme is [practically stable](../../../../practical-stability-of-a-finite-difference-scheme.md) under the given condition. For $a>0$ it is equivalent to $\Delta t\leq2a$ and $\Delta t\leq(\Delta x)^2/(2a)$. This is the [Forward Euler stability for centered advection-diffusion](../../../../forward-euler-stability-for-centered-advection-diffusion.md) calculation with the diffusion coefficient retained. The proof does not require all three stencil weights to be nonnegative.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the numerical solutions of partial differential equations course of the University of Oxford](../../../split.md)
5. [Numerical solutions of partial differential equations course of the University of Oxford](../../../../numerical-solutions-of-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
