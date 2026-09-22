<h1 id="23g/solution">Solution</h1>

↑ **Parent:** [23G](../23g.md)

For $s\in\mathbb R$, the [Sobolev space](../../../../../sobolev-space-split.md) $H^s(\mathbb R^n)$ consists of tempered distributions $u$ such that

$$
\|u\|_{H^s}^2
=\int_{\mathbb R^n}
(1+|\xi|^2)^s|\widehat u(\xi)|^2\,d\xi
<\infty.
$$

For a multi-index $\alpha$,

$$
\widehat{D^\alpha u}(\xi)=(i\xi)^\alpha\widehat u(\xi).
$$

Since

$$
(1+|\xi|^2)^{s-|\alpha|}|\xi|^{2|\alpha|}
\leq(1+|\xi|^2)^s,
$$

we obtain the [Sobolev derivative estimate](../../../../../sobolev-derivative-estimate.md)

$$
\boxed{
\|D^\alpha u\|_{H^{s-|\alpha|}}
\leq\|u\|_{H^s}
}.
$$

Thus differentiation is bounded and linear between the stated spaces.

Taking the [Fourier transform](../../../../../fourier-transform.md) of

$$
-\Delta u+u=f
$$

gives

$$
(1+|\xi|^2)\widehat u(\xi)=\widehat f(\xi).
$$

The only possible solution is therefore

$$
\widehat u(\xi)=\frac{\widehat f(\xi)}{1+|\xi|^2}.
$$

Moreover,

$$
\|u\|_{H^{s+2}}^2
=\int(1+|\xi|^2)^{s+2}
\frac{|\widehat f(\xi)|^2}{(1+|\xi|^2)^2}\,d\xi
=\|f\|_{H^s}^2.
$$

This proves existence, uniqueness, and bounded dependence. Conversely, $u\mapsto(-\Delta+1)u$ maps $H^{s+2}$ boundedly to $H^s$, so

$$
\boxed{
-\Delta+1:H^{s+2}(\mathbb R^n)\longrightarrow H^s(\mathbb R^n)
}
$$

is a linear isomorphism with inverse multiplier $(1+|\xi|^2)^{-1}$. This is the [massive Laplacian isomorphism on Sobolev spaces](../../../../../massive-laplacian-isomorphism-on-sobolev-spaces.md).

Finally, the assumed estimate and [Plancherel theorem](../../../../../plancherel-theorem.md) imply

$$
\int_{\mathbb R^n}
(1+|\xi|^2)^2|\widehat u_j(\xi)|^2\,d\xi
\leq
C\bigl(\|u_j\|_2^2+\|\Delta u_j\|_2^2\bigr)
\leq C K^2.
$$

Thus $(u_j)$ is bounded in $H^2(\mathbb R^n)$. The functions and all their first derivatives are supported in the fixed bounded set $\overline\Omega$. Their $H^1$ bounds give uniform translation estimates

$$
\|v(\,\cdot+h)-v\|_2
\leq|h|\,\|\nabla v\|_2
$$

for $v=u_j$ and $v=D_\ell u_j$. Tight support and the [Rellich-Kondrashov compactness theorem for H01](../../../../../rellich-kondrashov-compactness-theorem-for-h01.md), equivalently the Fourier compactness criterion, therefore provide a common subsequence for which $u_j$ and every first derivative converge strongly in $L^2$. Hence

$$
\boxed{u_{j_k}\longrightarrow u\quad\text{strongly in }H^1(\mathbb R^n)}.
$$

This is [compactness from bounded support and an H2 bound](../../../../../compactness-from-bounded-support-and-an-h2-bound.md).

## ↑ Ancestors (10)

1. [23G](../23g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
