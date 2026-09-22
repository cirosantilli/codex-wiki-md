<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose a spatial interval with [periodic boundary conditions](../../../../../../periodic-boundary-conditions.md) and a uniform grid, so no separate inflow [boundary closure of a difference scheme](../../../../../../boundary-closure-of-a-difference-scheme.md) is required. The [discrete Fourier transform](../../../../../../discrete-fourier-transform.md) is a [unitary operator](../../../../../../unitary-operator.md) in the [discrete L2 norm](../../../../../../discrete-l2-norm.md). Every circulant stencil is diagonal in that transform, and a one-step [Fourier multiplier](../../../../../../fourier-multiplier.md) is a contraction exactly when its modulus is at most one for every grid frequency. For a mesh-uniform statement, use all $\theta\in[-\pi,\pi]$, the limiting frequency range.

A [Fourier mode](../../../../../../fourier-mode.md) $e^{im\theta}$ gives

$$
G(\theta)=\frac{N(\theta)}{D(\theta)},\qquad
N=d+ee^{i\theta},\qquad D=ae^{-i\theta}+b+ce^{i\theta},
$$

with the coefficients from (a). Squaring moduli and putting $v=\cos\theta$ yields

$$
\boxed{|D|^2-|N|^2
=\frac{\mu(\mu-2)(\mu-1)(\mu+1)}9(1-\cos\theta)^2.}
$$

This has the required nonnegative sign for every frequency exactly when

$$
\boxed{\mu\in(-\infty,-1]\cup[0,1]\cup[2,\infty).}
$$

One must also check that the implicit equation is solvable, rather than divide by a vanishing symbol. Here

$$
\operatorname{Im}D=\frac{1-2\mu}{3}\sin\theta,\qquad D(0)=1,
\qquad D(\pi)=\frac{1+2\mu-2\mu^2}{3}.
$$

For $\mu\ne1/2$, a zero would have to occur at zero or $\pi$; the latter occurs only at $(1\pm\sqrt3)/2$, both outside the displayed stable intervals. At $\mu=1/2$, $D=3/4+(1/4)\cos\theta\geq1/2$. Thus there is no denominator zero in the stable range. For fixed such $\mu$, continuity on the compact frequency interval gives a uniformly bounded inverse, and $|G|\leq1$ proves $\|U^n\|_{2,h}\leq\|U^0\|_{2,h}$ for all steps.

Outside these intervals the displayed difference is negative at every nonzero frequency where $D\ne0$, so $|G|>1$. On periodic refining meshes there are frequencies approaching any selected such value. Their amplification is bounded away from one and is repeated $O(h^{-1})$ times over a fixed physical interval when $k=\mu h$, violating a mesh-uniform stability bound. At the two singular parameters the implicit operator itself fails on meshes containing the Nyquist mode. These observations prove necessity as well as sufficiency.

For the physical convention $k>0$, $h>0$, the result is **$0<\mu\leq1$ or $\mu\geq2$**, with zero admitted as the identity limit. The negative intervals describe the algebraic contraction result for signed [Courant numbers](../../../../../../courant-number.md). In particular, the additional large positive interval must not be discarded by imposing the usual explicit-scheme [Courant–Friedrichs–Lewy condition](../../../../../../courant-friedrichs-lewy-condition.md): this scheme is implicit. Stability at large fixed [Courant number](../../../../../../courant-number.md) is not a guarantee of a small error constant.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
