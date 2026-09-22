<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $e_N(t)=e^{2\pi it/N}$ and use normalized averages $\mathbb E_x=N^{-1}\sum_{x\in\mathbb Z/N\mathbb Z}$. Our convention for [Fourier coefficients on a finite abelian group](../../../../../fourier-coefficient-on-a-finite-abelian-group.md) is

$$
\boxed{\widehat f(r)=\mathbb E_xf(x)e_N(-rx),\qquad r\in\mathbb Z/N\mathbb Z.}
$$

The underlying [orthogonality of complex exponentials](../../../../../orthogonality-of-complex-exponentials.md) is $\mathbb E_xe_N(rx)=1$ for $r=0$ and zero otherwise. For nonzero $r$ this is the finite [geometric series](../../../../../geometric-series.md) with ratio $e_N(r)\ne1$; its sum vanishes because that ratio has $N$th power one. The identical orthogonality statement holds when averaging over $r$ instead of $x$.

Using this orthogonality to sum the definition over $r$ proves [Fourier inversion on a finite group](../../../../../fourier-inversion-on-a-finite-group.md):

$$
\sum_r\widehat f(r)e_N(rx)
=\mathbb E_yf(y)\sum_re_N(r(x-y))=f(x).
$$

Indeed $\mathbb E f\overline g=\sum_r\overline{\widehat g(r)}\mathbb E_x f(x)e_N(-rx)=\sum_r\widehat f(r)\overline{\widehat g(r)}$. This proves the [Parseval identity on a finite group](../../../../../parseval-identity-on-a-finite-group.md) and its squared-norm case:

$$
\mathbb E_xf(x)\overline{g(x)}=\sum_r\widehat f(r)\overline{\widehat g(r)},\qquad
\sum_r|\widehat f(r)|^2=\mathbb E_x|f(x)|^2.
$$

For [normalized convolution on a finite group](../../../../../normalized-convolution-on-a-finite-group.md), write $(f*g)(x)=\mathbb E_yf(y)g(x-y)$. Changing variables $x=y+z$ in its transform gives

$$
\widehat{f*g}(r)
=\mathbb E_{y,z}f(y)g(z)e_N(-r(y+z))
=\widehat f(r)\widehat g(r),
$$

the [convolution theorem on a finite group](../../../../../convolution-theorem-on-a-finite-group.md). [Linearity](../../../../../linearity.md) of the transform follows directly from its definition. [Translation](../../../../../translation-geometry.md) $\tau_tf(x)=f(x+t)$ gives $\widehat{\tau_tf}(r)=e_N(rt)\widehat f(r)$ by changing variables. [Complex conjugation](../../../../../complex-conjugation.md) gives $\widehat{\overline f}(r)=\overline{\widehat f(-r)}$; for $\widetilde f(x)=\overline{f(-x)}$, the corresponding identity is $\widehat{\widetilde f}(r)=\overline{\widehat f(r)}$. Finally $\widehat f(0)=\mathbb E f$ and $|\widehat f(r)|\leq\mathbb E|f|$ by the [triangle inequality](../../../../../triangle-inequality.md). These identities establish the basic [normalized Fourier analysis on a finite abelian group](../../../../../normalized-fourier-analysis-on-a-finite-abelian-group.md) needed below, with all normalizations fixed.

For completeness, pointwise multiplication has the dual convolution formula $\widehat{fg}(r)=\sum_s\widehat f(s)\widehat g(r-s)$: insert the inversion formula for $g$ into the defining average and collect its frequencies. If $c\ne0$ modulo $N$, the change of variables $u=cx$ gives $\widehat{f(c\,\cdot)}(r)=\widehat f(rc^{-1})$. These also follow directly from the same [additive character](../../../../../additive-character.md) orthogonality.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
