<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The bounded classical solution is the [heat-kernel convolution](../../../../../heat-kernel-convolution.md)

$$
\boxed{u(x,t)=\frac1{4\pi t}\int_{\mathbb R^2}\exp\!\left(-\frac{|x-y|^2}{4t}\right)g(y)\,dy,\qquad t>0.}
$$

The two-dimensional [heat kernel](../../../../../heat-kernel.md) has integral one. Boundedness of $g$ permits differentiation under the integral for $t>0$, proving $u_t=\Delta u$ and $|u|\le\|g\|_\infty$. Its [approximate identity](../../../../../approximate-identity.md) property gives $u(x,t)\to g(x)$, locally uniformly since $g$ is [continuous](../../../../../continuous-function.md). This bounded solution satisfies the required Gaussian-growth bound.

For [heat-equation uniqueness under Gaussian growth](../../../../../heat-equation-uniqueness-under-gaussian-growth.md), let $w$ be the difference of two solutions, so $w(x,0)=0$ and $|w|\le M_0e^{a|x|^2}$ on a finite time interval. Choose $b>a$ and a slab $0\le t\le\tau<1/(4b)$. The positive comparison solution

$$
\Phi_b(x,t)=\frac1{1-4bt}\exp\!\left(\frac{b|x|^2}{1-4bt}\right)
$$

satisfies $(\Phi_b)_t=\Delta\Phi_b$. For any $\varepsilon>0$, its faster spatial growth makes $|w|\le\varepsilon\Phi_b$ on a sufficiently large lateral cylinder boundary. At the initial boundary, $w=0$. The [heat equation maximum principle](../../../../../heat-equation-maximum-principle.md) applied to $\pm w-\varepsilon\Phi_b$ proves the same inequality inside. First allow the cylinder radius to increase, then let $\varepsilon\downarrow0$. Repeating these slabs proves uniqueness on every finite interval with the stated uniform growth bound. No spatial integrability of $g$ is required.

At time $T$, this is [Gaussian filtering](../../../../../gaussian-blur.md) with covariance $2T I$, hence **$\sigma=\sqrt{2T}$ per coordinate**. With the angular-frequency [Fourier transform](../../../../../fourier-transform.md) convention $\widehat f(\xi)=\int e^{-ix\cdot\xi}f(x)\,dx$, the [Gaussian filtering Fourier multiplier](../../../../../gaussian-filtering-fourier-multiplier.md) is

$$
\boxed{\widehat u(\xi,T)=e^{-T|\xi|^2}\widehat g(\xi)=e^{-\sigma^2|\xi|^2/2}\widehat g(\xi).}
$$

For merely bounded $g$, this identity is understood through [tempered distributions](../../../../../tempered-distribution.md). The multiplier leaves the zero frequency unchanged and attenuates large [frequencies](../../../../../frequency.md) exponentially: it suppresses rapid noise fluctuations but blurs [image edges](../../../../../image-edge.md). In cycles-per-length frequency $k$, the multiplier is $e^{-4\pi^2T|k|^2}$.

For the printed [Perona-Malik equation](../../../../../perona-malik-equation.md), retain the supplied conductance $c(s)=s e^{-s^2/(2\lambda^2)}$, which includes an extra factor $s$. In one dimension write $p=u_x$ and $F(p)=c(|p|)p=p|p|e^{-p^2/(2\lambda^2)}$. Then $u_t=F'(u_x)u_{xx}$, with

$$
F'(p)=|p|e^{-p^2/(2\lambda^2)}\left(2-\frac{p^2}{\lambda^2}\right)\quad(p\ne0),\qquad F'(0)=0.
$$

The [forward-backward threshold for gradient-weighted exponential diffusion](../../../../../forward-backward-threshold-for-gradient-weighted-exponential-diffusion.md) is therefore

$$
\boxed{0<|u_x|<\sqrt2\lambda:\ \text{forward diffusion};\quad |u_x|>\sqrt2\lambda:\ \text{backward diffusion}.}
$$

At $|u_x|=0$ and $\sqrt2\lambda$ the coefficient vanishes, giving degenerate diffusion. Increasing $\lambda$ increases the forward-diffusion range. Small nonzero slopes smooth, while large slopes formally sharpen; a negative coefficient produces short-wave growth and [ill-posedness](../../../../../ill-posed-problem.md), so this is a dynamics explanation, not a general existence theorem for arbitrary data. Replacing the printed conductance by $e^{-s^2/(2\lambda^2)}$ would give threshold $\lambda$, but that is a different equation.

The [four-neighbour mean expansion](../../../../../four-neighbour-mean-expansion.md) follows by [Taylor expansion](../../../../../taylor-expansion.md): opposing first and third [derivatives](../../../../../derivative.md) cancel, so

$$
\operatorname{mean}_h(u)(x)=u(x)+\frac{h^2}{4}\Delta u(x)+\frac{h^4}{48}\bigl(u_{xxxx}(x)+u_{yyyy}(x)\bigr)+O(h^6).
$$

If $u(x_0)=\operatorname{mean}_h(u)(x_0)$ for every sufficiently small $h$, division by $h^2$ and passage to the [limit](../../../../../limit-of-a-function.md) give **$\Delta u(x_0)=0$**. This is a pointwise conclusion; it does not assert harmonicity in a whole neighbourhood.

For the area [median](../../../../../median.md) over the disk, the [disk-median curvature expansion](../../../../../disk-median-curvature-expansion.md), at a point where $|\nabla u|\ne0$, is

$$
\operatorname{median}_{B_h(x_0)}u=u(x_0)+\frac{h^2}{6}\left(\Delta u-\frac{\nabla u^T(D^2u)\nabla u}{|\nabla u|^2}\right)(x_0)+o(h^2).
$$

Consequently the analogous [median](../../../../../median.md) fixed-point condition yields

$$
\boxed{\Delta u(x_0)-\frac{\nabla u(x_0)^T(D^2u(x_0))\nabla u(x_0)}{|\nabla u(x_0)|^2}
=|\nabla u(x_0)|\operatorname{div}\!\left(\frac{\nabla u}{|\nabla u|}\right)(x_0)=0.}
$$

This is the vanishing of the [level-line curvature](../../../../../level-line-curvature.md) at $x_0$: to second order the level line is straight there. It need not be a straight segment. For example $u(x,y)=y+x^3$ has zero disk [median](../../../../../median.md) at the origin for every radius, by odd symmetry, but its zero level line is the cubic $y=-x^3$. Vanishing [curvature](../../../../../curvature.md) on an entire connected regular level arc would force that arc to be straight. The factor $1/6$ is for the disk's uniform area measure; a circle-boundary [median](../../../../../median.md) has a different scale factor, while producing the same zero-curvature equation.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
