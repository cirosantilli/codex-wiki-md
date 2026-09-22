<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $G=L^{-1}$ and use the bound from part (b),

$$
|Gh|_{2,\alpha;B}\leq M|h|_{0,\alpha;B}.
$$

On the closed ball $\mathcal B_\varepsilon\subset C_0^{2,\alpha}(B)$ define

$$
T(u)=G(f-cu-g(u)).
$$

The Hölder product estimate and part (i) give

$$
|T(u)|_{2,\alpha}
\leq M\big(|f|_{0,\alpha}+C|c|_{0,\alpha}\varepsilon+\varepsilon^2\big),
$$

and

$$
|T(u)-T(v)|_{2,\alpha}
\leq M\big(C|c|_{0,\alpha}+2\varepsilon\big)|u-v|_{2,\alpha}.
$$

Choose $\varepsilon_0$ so that $2M\varepsilon_0<1/2$, then choose $\delta_0$ so that the remaining terms make $T$ preserve $\mathcal B_{\varepsilon_0}$ and have contraction constant less than one. The [Banach fixed-point theorem](../../../../../../../contraction-mapping-theorem.md) gives a unique $u$ in that ball satisfying

$$
\boxed{Lu+g(u)+cu=f,
\qquad u|_{\partial B}=0.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 107](../../../../paper-107-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
