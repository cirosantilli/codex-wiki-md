<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The rational translate $g(\tau)=f(a/N+\tau)$ has [Fourier coefficients](../../../../../../fourier-coefficient.md) $e^{2\pi ian/N}c_n$, with the same polynomial bound as $c_n$. Thus the preceding [Mellin transform](../../../../../../mellin-transform.md) gives, initially for $\operatorname{Re}s$ large, the completion of the [additive twist of a cusp-form L-function](../../../../../../additive-twist-of-a-cusp-form-l-function.md)

$$
M_a(s)=\left(\frac N{2\pi}\right)^s\Gamma(s)\sum_{n\geq1}e^{2\pi ian/N}c_nn^{-s}=\int_0^\infty f\!\left(\frac aN+iy\right)(Ny)^s\frac{dy}{y}.
$$

Write $\varepsilon=i^k=(-1)^{k/2}$. Nonzero level-one forms have even weight, so $\varepsilon^2=1$. Split the integral at $1/N$. In its lower part substitute $y=1/(N^2v)$, and use [rational-cusp inversion of a level-one cusp form](../../../../../../rational-cusp-inversion-of-a-level-one-cusp-form.md) with $\tau=iv$:

$$
f\!\left(\frac aN+\frac i{N^2v}\right)=\varepsilon(Nv)^kf\!\left(-\frac dN+iv\right),\qquad(Ny)^s=(Nv)^{-s},\qquad\frac{dy}{y}=-\frac{dv}{v}.
$$

The bounds reverse from $(0,1/N)$ to $(\infty,1/N)$, so

$$
\boxed{M_a(s)=\int_{1/N}^\infty\left[f\!\left(\frac aN+iy\right)(Ny)^s+\varepsilon f\!\left(-\frac dN+iy\right)(Ny)^{k-s}\right]\frac{dy}{y}.}
$$

Both cusp values in this integral are $O(e^{-2\pi y})$ as $y\to\infty$. On any compact set of $s$-values, the remaining powers of $Ny$ are bounded by fixed positive powers of $y$; differentiation in $s$ merely introduces powers of $\log(Ny)$. The integral and its differentiated integrals therefore converge uniformly on compact sets. It defines an [entire function](../../../../../../entire-function.md) of $s$, agreeing with the original completion in its half-plane of convergence, and hence supplies the required [analytic continuation](../../../../../../analytic-continuation.md) to $\mathbb C$.

For the opposite rational cusp, $a'=-d$ has inverse $d'=-a$ modulo $N$. Denote the two individual upper integrals by $I_a(s)$ and $I_{-d}(s)$. The representation gives

$$
M_a(s)=I_a(s)+\varepsilon I_{-d}(k-s),\qquad M_{-d}(s)=I_{-d}(s)+\varepsilon I_a(k-s).
$$

Replacing $s$ by $k-s$ in the first equality and using $\varepsilon^2=1$ proves the [functional equation of an additive cusp-form twist](../../../../../../functional-equation-of-an-additive-cusp-form-twist.md):

$$
\boxed{M(f,a/N,k-s)=(-1)^{k/2}M(f,-d/N,s).}
$$

For $N=1$ this specializes to the entire completion and [functional equation](../../../../../../functional-equation.md) of the ordinary [L-function of a cusp form](../../../../../../l-function-of-a-cusp-form.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
