<h1 id="13f/solution">Solution</h1>

↑ **Parent:** [13F](../13f.md)

[Jordan lemma](../../../../../jordan-s-lemma.md) states that if $a>0$ and $g$ is analytic in the upper half-plane outside a fixed circle, with

$$
M_R=\max_{0\leq\theta\leq\pi}|g(Re^{i\theta})|\longrightarrow0,
$$

then on the upper semicircle $C_R$,

$$
\int_{C_R}e^{iaz}g(z)\,dz\longrightarrow0.
$$

Indeed, $|e^{iaRe^{i\theta}}|=e^{-aR\sin\theta}$. Using symmetry and $\sin\theta\geq2\theta/\pi$ on $0\leq\theta\leq\pi/2$ gives

$$
\left|\int_{C_R}e^{iaz}g(z)\,dz\right|
\leq2RM_R\int_0^{\pi/2}e^{-2aR\theta/\pi}\,d\theta
\leq\frac{\pi M_R}{a}\longrightarrow0.
$$

The [residue](../../../../../residue.md) of $f$ at an isolated singularity $a$ is the coefficient of $(z-a)^{-1}$ in its [Laurent series](../../../../../laurent-series.md), equivalently

$$
\operatorname{Res}(f,a)=\frac1{2\pi i}\oint f(z)\,dz.
$$

If $f(z)=g(z)/(z-a)^k$, the Taylor expansion of the analytic function $g$ shows that

$$
\boxed{\operatorname{Res}(f,a)=\frac{g^{(k-1)}(a)}{(k-1)!}}.
$$

For the real integral, apply [contour integration](../../../../../contour-integration.md) in the upper half-plane to

$$
F(z)=\frac{z^3e^{iz}}{(1+z^2)^2}.
$$

Jordan's lemma removes the semicircular arc. The only enclosed singularity is the double pole at $z=i$, whose residue is

$$
\operatorname{Res}(F,i)
=\left.\frac d{dz}\left(\frac{z^3e^{iz}}{(z+i)^2}\right)\right|_{z=i}
=\frac1{4e}.
$$

The [residue theorem](../../../../../residue-theorem.md) therefore gives

$$
\int_{-\infty}^{\infty}\frac{x^3e^{ix}}{(1+x^2)^2}\,dx
=\frac{\pi i}{2e}.
$$

Its real part vanishes because $x^3\cos x/(1+x^2)^2$ is an [odd function](../../../../../odd-function.md), while its imaginary part is the requested integral. Hence

$$
\boxed{\int_{-\infty}^{\infty}\frac{x^3\sin x}{(1+x^2)^2}\,dx=\frac\pi{2e}}.
$$

## ↑ Ancestors (10)

1. [13F](../13f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
