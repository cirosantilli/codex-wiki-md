<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The constant [Fourier coefficient](../../../../../../fourier-coefficient.md) is $A_0(y,s)=\int_0^1G(x+iy,s)\,dx$. The $m=0$ terms give $2\zeta(2s)y^s$. For fixed $m\ne0$, unfolding the sum over $n$ gives

$$
\sum_{n\in\mathbb Z}\int_0^1\frac{y^s\,dx}{((mx+n)^2+m^2y^2)^s}
=\int_{\mathbb R}\frac{y^s\,du}{(u^2+m^2y^2)^s}.
$$

Indeed, the substitution $u=mx+n$ introduces a factor $1/|m|$, while the translated intervals of length $|m|$ cover the real line exactly $|m|$ times, cancelling that factor. Now scale $u=|m|yt$. The [beta function](../../../../../../beta-function.md) integral yields

$$
\int_{\mathbb R}(1+t^2)^{-s}\,dt
=\sqrt\pi\,\frac{\Gamma(s-1/2)}{\Gamma(s)},
$$

which can be checked by inserting $(1+t^2)^{-s}=\Gamma(s)^{-1}\int_0^\infty v^{s-1}e^{-v(1+t^2)}\,dv$ and evaluating the inner [Gaussian integral](../../../../../../gaussian-integral.md). Thus the fixed-$m$ contribution is $|m|^{1-2s}y^{1-s}\sqrt\pi\,\Gamma(s-1/2)/\Gamma(s)$. Summing over positive and negative $m$ proves the [constant term of a nonholomorphic Eisenstein series](../../../../../../constant-term-of-a-nonholomorphic-eisenstein-series.md)

$$
A_0(y,s)=2\zeta(2s)y^s
+2\sqrt\pi\,\frac{\Gamma(s-1/2)}{\Gamma(s)}\zeta(2s-1)y^{1-s}.
$$

With the printed normalization $\xi(u)=\pi^{-u/2}\Gamma(u/2)\zeta(u)$ of the [completed Riemann zeta function](../../../../../../completed-riemann-zeta-function.md), this is exactly

$$
\boxed{\pi^{-s}\Gamma(s)A_0(y,s)=2\xi(2s)y^s+2\xi(2s-1)y^{1-s}.}
$$

Both the unfolding and the original series calculation are justified for $\operatorname{Re}s>1$. Beyond this region the identities are understood meromorphically: $G(\tau,s)$ is the [Epstein zeta function](../../../../../../epstein-zeta-function.md) of the unit-covolume lattice $(\mathbb Z\tau+\mathbb Z)/\sqrt y$, so question 4 supplies its continuation. The symbol $\xi$ here has the completed-zeta normalization displayed above, which has poles at zero and one; it does not include the extra polynomial factor sometimes used to define an entire xi function.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 126](../../../paper-126-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
