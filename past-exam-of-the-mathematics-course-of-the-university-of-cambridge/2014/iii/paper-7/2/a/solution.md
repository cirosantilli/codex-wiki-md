<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the unit-period [circle](../../../../../../circle.md) $\mathbb T=\mathbb R/\mathbb Z$, with total measure one. The free [characteristic flow map](../../../../../../characteristic-flow-map.md) gives

$$
 f_t(x,v)=f_0(x-tv,v).
$$

Translations in $x$ preserve its periodic measure. The [Tonelli theorem](../../../../../../tonelli-theorem.md) and the [integral](../../../../../../integral.md) [triangle inequality](../../../../../../triangle-inequality.md) yield

$$
 \boxed{\|\rho_t\|_{L^1(\mathbb T)}
 \leq\int_{\mathbb T}\int_{\mathbb R}|f_0(x-tv,v)|\,dv\,dx
 =\|f_0\|_{L^1(\mathbb T\times\mathbb R)}.}
$$

The [Fubini's theorem](../../../../../../fubini-s-theorem.md) therefore applies also to signed data, and the same translation gives

$$
 \boxed{\int_{\mathbb T}\rho_t(x)\,dx=\int_{\mathbb T}\int_{\mathbb R}f_0(x,v)\,dv\,dx=\rho_\infty.}
$$

This holds for positive or negative time. The printed $L^1(\mathbb R)$ in this subpart is a domain typo: the spatial variable is periodic, so the correct space is $L^1(\mathbb T)$. For example, the smooth initial value $f_0(x,v)=e^{-v^2}$ gives the constant density $\sqrt\pi$, whose periodic extension is not integrable on the real line.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
