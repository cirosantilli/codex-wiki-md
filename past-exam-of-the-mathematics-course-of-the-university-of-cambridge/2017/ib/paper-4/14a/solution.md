<h1 id="14a/solution">Solution</h1>

↑ **Parent:** [14A](../14a.md)

The PDF specifies decay as $y\to\infty$; the local TeX drops this limit from its displayed boundary data. Take $a=4\pi$, so the [conformal map](../../../../../conformal-map.md) is $w=\sin(z/4)$. Its components are

$$
\xi=\sin(x/4)\cosh(y/4),\qquad \eta=\cos(x/4)\sinh(y/4).
$$

For $-2\pi<x<2\pi$ and $y>0$, $\eta>0$. The bottom edge maps monotonically to $(-1,1)$, and the two vertical sides map to the real rays $(-\infty,-1)$ and $(1,\infty)$. The [derivative](../../../../../derivative.md) $\cos(z/4)/4$ never vanishes in the interior. Injectivity follows from the identities for equal sines: the alternatives $z_1/4=z_2/4+2\pi n$ and $z_1/4=\pi-z_2/4+2\pi n$ give only the identical point within this strip. Surjectivity can be seen directly: for fixed $\xi$ and $v=y/4>0$, solve $\sin(x/4)=\xi/\cosh v$; then

$$
\eta^2=\sinh^2v-\xi^2\tanh^2v.
$$

On $v>\max(0,\operatorname{arcosh}|\xi|)$, with the lower endpoint read as $0$ when $|\xi|\leq1$, the right side increases strictly from zero to infinity. Thus every point of the [upper half-plane](../../../../../upper-half-plane-complex-analysis.md) has a unique preimage.

By [conformal invariance of harmonicity](../../../../../conformal-invariance-of-harmonicity.md), write the transformed [harmonic function](../../../../../harmonic-function.md) as $\Phi(\xi,\eta)$. Its real-axis boundary data are

$$
\boxed{F(s)=\begin{cases}f(4\arcsin s),&-1<s<1,\\0,&|s|>1.\end{cases}}
$$

The [inverse sine](../../../../../inverse-sine.md) on $(-1,1)$ is its real principal branch. For bounded integrable data, take the [Fourier transform](../../../../../fourier-transform.md) convention $\widehat\Phi(k,\eta)=\int_\mathbb R\Phi(\xi,\eta)e^{-ik\xi}\,d\xi$. The [Laplace equation](../../../../../laplace-equation.md) becomes $\widehat\Phi_{\eta\eta}-k^2\widehat\Phi=0$, with the bounded decaying solution $\widehat\Phi=\widehat F(k)e^{-|k|\eta}$. Inverting the [Fourier transform](../../../../../fourier-transform.md) gives

$$
\frac1{2\pi}\int_\mathbb Re^{ik u-|k|\eta}\,dk=\frac{\eta}{\pi(\eta^2+u^2)}.
$$

Consequently the [Poisson kernel for the upper half-plane](../../../../../poisson-kernel-for-the-upper-half-plane.md) yields

$$
\boxed{\phi(x,y)=\Phi(\xi,\eta)=\frac{\eta}{\pi}\int_{-1}^1\frac{F(s)}{\eta^2+(\xi-s)^2}\,ds}.
$$

The decay is uniform across the strip: $|w|^2=\sin^2(x/4)+\sinh^2(y/4)\geq\sinh^2(y/4)$ and, for $|w|>1$, $|\Phi|\leq\|F\|_{L^1}|w|/(\pi(|w|-1)^2)\to0$. This verifies the printed decay condition. Boundary limits give the prescribed values at continuity points away from the corners.

For the given sine data,

$$
\boxed{F(s)=s\quad(-1<s<1),\qquad F(s)=0\quad(|s|>1)}.
$$

Values assigned at $s=\pm1$ do not alter the integral. **There is no solution [continuous](../../../../../continuous-function.md) on the entire closed half-strip for these data**: the bottom edge has corner limits $\pm1$, but the side edges have corner limits zero. The formula is the bounded [Dirichlet problem](../../../../../dirichlet-problem.md) solution with the specified limits away from those two corners. This is the usual interpretation of the printed problem; boundedness excludes additional boundary-singular [harmonic functions](../../../../../harmonic-function.md), while decay alone without a regularity or boundedness condition does not establish uniqueness.

## ↑ Ancestors (10)

1. [14A](../14a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
