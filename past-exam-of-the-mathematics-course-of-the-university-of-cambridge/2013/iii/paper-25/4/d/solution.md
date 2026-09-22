<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Under $\mathbb Q$, $X_T=x+W_T^{\mathbb Q}$ has density $\varphi_T(z-x)=(2\pi T)^{-1/2}\exp(-(z-x)^2/(2T))$. The reciprocal [Radon-Nikodym derivative](../../../../../../radon-nikodym-derivative.md) depends only on $X_T$:

$$
\frac{d\mathbb P}{d\mathbb Q}=\frac{\cosh X_T}{\cosh x}e^{-T/2}.
$$

Consequently the [probability density function](../../../../../../probability-density-function.md) under the original measure is

$$
\boxed{p_T(x,z)=\frac{\cosh z}{\cosh x}\frac{e^{-T/2}}{\sqrt{2\pi T}}\exp\left(-\frac{(z-x)^2}{2T}\right),\qquad z\in\mathbb R.}
$$

It integrates to one because $\mathbb E_{\mathbb Q}\cosh X_T=e^{T/2}\cosh x$. Completing the square also gives the useful [mixture distribution](../../../../../../mixture-distribution.md) form

$$
p_T(x,z)=\frac{e^x}{2\cosh x}\varphi_T(z-x-T)+\frac{e^{-x}}{2\cosh x}\varphi_T(z-x+T).
$$

Thus the terminal law is a mixture of $N(x+T,T)$ and $N(x-T,T)$ with the displayed positive weights. The [diffusion with hyperbolic tangent drift](../../../../../../diffusion-with-hyperbolic-tangent-drift.md) density also exhibits the [Doob h-transform](../../../../../../doob-h-transform.md) with $h(z)=\cosh z$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
