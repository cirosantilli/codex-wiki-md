<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $K$ contain the support of $u\in\mathcal E'(\mathbb R^n)$. Choose a [cutoff function](../../../../../../cutoff-function.md) that equals one near $K$. It makes

$$
\widehat u(\lambda)=\langle u(x),e^{-i\lambda\cdot x}\rangle
$$

well-defined, and differentiating the parameter under the pairing gives

$$
\partial_\lambda^\gamma\widehat u(\lambda)
=\langle u(x),(-ix)^\gamma e^{-i\lambda\cdot x}\rangle.
$$

Thus the [Fourier transform of a compactly supported distribution](../../../../../../fourier-transform-of-a-compactly-supported-distribution.md) is a [smooth function](../../../../../../smooth-function.md). Since a compactly supported distribution has finite order, some $N$ and $C$ satisfy

$$
|\langle u,\psi\rangle|\leq C\sum_{|\alpha|\leq N}\sup_K|\partial^\alpha\psi|.
$$

Applying this estimate to the exponential yields $|\widehat u(\lambda)|\leq C'\langle\lambda\rangle^N$.

Now take $v\in\mathcal E'(X)$, multiply by a [cutoff function](../../../../../../cutoff-function.md) supported in $X$ and equal to one near $\operatorname{supp}v$, and regard the result as an element of $\mathcal E'(\mathbb R^n)$. Choose $m$ so large that

$$
g(\lambda)=\langle\lambda\rangle^{-2m}\widehat v(\lambda)
$$

is [Lebesgue integrable](../../../../../../lebesgue-integrable-function.md). The inverse [Fourier transform](../../../../../../fourier-transform.md) $f=\mathcal F^{-1}g$ is a bounded [continuous function](../../../../../../continuous-function.md), and the [Fourier transform of a derivative](../../../../../../fourier-transform-of-a-derivative.md) gives

$$
v=(1-\Delta)^m f
$$

as a [distributional identity](../../../../../../distributional-identity.md). This is the [Bessel potential](../../../../../../bessel-potential.md) proof of the [structure theorem for compactly supported distributions](../../../../../../structure-theorem-for-compactly-supported-distributions.md).

The function $f$ itself need not have [compact support](../../../../../../compact-support.md). Choose another cutoff $\rho\in\mathcal D(X)$ equal to one near $\operatorname{supp}v$. Then $v=\rho(1-\Delta)^mf$. Repeatedly using

$$
\rho\,\partial^\alpha f
=\sum_{\beta\leq\alpha}(-1)^{|\alpha-\beta|}\binom{\alpha}{\beta}
\partial^\beta\bigl(f\,\partial^{\alpha-\beta}\rho\bigr)
$$

expresses $v$ as a finite sum $\sum_\beta\partial^\beta f_\beta$, where every coefficient $f_\beta$ is continuous and compactly supported in $X$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 327](../../../paper-327-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
