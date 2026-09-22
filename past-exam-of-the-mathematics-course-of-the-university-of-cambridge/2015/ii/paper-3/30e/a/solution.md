<h1 id="30e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a [Fourier transform](../../../../../../fourier-transform.md) convention for which $-\Delta$ has symbol $|\xi|^2$. The distributional equation gives $\hat u=\hat f/(|\xi|^2+m^2)$ for real nonzero $m$, since this smooth positive multiplier has no zeros. Consequently

$$
\|u\|_{H^{s+2}}^2=\int(1+|\xi|^2)^s\left(\frac{1+|\xi|^2}{|\xi|^2+m^2}\right)^2|\hat f|^2\,d\xi\leq C_m^2\|f\|_{H^s}^2,
$$

where $\boxed{C_m=\max(1,m^{-2})}$. This bound is independent of $s$. For $f\in H^s$, the same multiplier defines $u\in H^{s+2}$; alternatively approximate $f$ by [Schwartz functions](../../../../../../schwartz-function.md) and pass to the limit using the estimate. This is the [massive Laplacian isomorphism on Sobolev spaces](../../../../../../massive-laplacian-isomorphism-on-sobolev-spaces.md).

For $a=1+|\xi|^2$, the inequality $a\leq\epsilon a^2+1/(4\epsilon)$, integrated against $|\hat v|^2$, gives **the interpolation estimate**

$$
\boxed{\|v\|_{H^1}^2\leq\epsilon\|v\|_{H^2}^2+\frac1{4\epsilon}\|v\|_{L^2}^2.}
$$

For a finite global bound in the last request, assume $\|u\|_{L^2}<\infty$ as well as boundedness. This assumption is necessary: the smooth bounded solution $u\equiv m$ has infinite $H^2$ norm on $\mathbb R^n$. Put $M=\|u\|_\infty$, $U=\|u\|_2$. Then $u^3\in L^2$ with norm at most $M^2U$. Incorporate the constant drift on the left:

$$
(-\Delta-\alpha\cdot\nabla+m^2)u=u^3,\qquad (|\xi|^2+m^2-i\alpha\cdot\xi)\hat u=\widehat{u^3}.
$$

The [constant-drift massive elliptic estimate](../../../../../../constant-drift-massive-elliptic-estimate.md) follows because the modulus of this symbol is at least $|\xi|^2+m^2$, so the same multiplier argument first establishes $u\in H^2$ and then gives the stronger **a priori bound**

$$
\boxed{\|u\|_{H^2}\leq C_mM^2U.}
$$

It is allowed to depend on $\alpha$ but in fact does not need to. Once regularity has been established, the earlier estimate and interpolation also give the conventional absorption proof: $\|u\|_{H^2}\leq C_m(M^2U+|\alpha|\|u\|_{H^1})$, and choosing $\epsilon$ small absorbs the $H^2$ term.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30E](../../30e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
