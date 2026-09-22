<h1 id="30b/solution">Solution</h1>

↑ **Parent:** [30B](../30b.md)

Under local integrability and suitable bounds away from zero, [Watson's lemma](../../../../../watson-s-lemma.md) gives

$$
\int_0^Ae^{-\lambda t}f(t)\,dt\sim\sum_{n\ge0}a_n\Gamma(\alpha+n\beta+1)\lambda^{-\alpha-n\beta-1},\qquad\lambda\to+\infty.
$$

Each term follows by $u=\lambda t$ and the [Gamma function](../../../../../gamma-function.md) integral; a finite local remainder is bounded in the same way, and the region away from zero is exponentially small.

For [Laplace's method](../../../../../laplace-s-method.md), assume an isolated nondegenerate global minimum $t_*$ of $p$, with $p''(t_*)>0$ and suitable tail bounds. Expand $p,q$ near $t_*$ and set $t-t_*=v/\sqrt z$. The leading term is $e^{-zp(t_*)}q(t_*)\sqrt{2\pi/(zp''(t_*))}$; successive terms come from Gaussian moments of the Taylor expansions. Several equally low minima contribute additively, while degenerate minima need a different scale.

Here the integrand is entire in $t$, so deform the contour to the line at imaginary part $-\pi$, the vertical segment from $-i\pi$ to $i\pi$, and the line at imaginary part $\pi$. The two horizontal tails sum to $2\int_0^\infty e^{-z\cosh x}\,dx=O(e^{-z}z^{-1/2})$. The vertical segment contributes $i\int_{-\pi}^{\pi}e^{z\cos\theta}\,d\theta$. Its maximum is at zero; putting $\theta=v/\sqrt z$ and using $\cos\theta=1-\theta^2/2+\theta^4/24+\cdots$ gives

$$
i e^zz^{-1/2}\int_{\mathbb R}e^{-v^2/2}\left(1+\frac{v^4}{24z}+O(z^{-2})\right)dv.
$$

The fourth Gaussian moment is three times the zeroth, so

$$
\boxed{\int_{-\infty-i\pi}^{\infty+i\pi}e^{z\cosh t}\,dt
=i\sqrt{2\pi}\,e^z\left(z^{-1/2}+\tfrac18z^{-3/2}+O(z^{-5/2})\right).}
$$

Since $\Gamma(1/2)=\sqrt\pi$, this has the required normalization.

## ↑ Ancestors (10)

1. [30B](../30b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
