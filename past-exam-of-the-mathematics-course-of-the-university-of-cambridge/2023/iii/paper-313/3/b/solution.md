<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Because ${}^\star{}^\star=1$, the [exterior algebra](../../../../../../exterior-algebra.md) of two-forms has the orthogonal decomposition

$$
\Lambda^2=\Lambda^2_+\oplus\Lambda^2_-,
\qquad
F_\pm=\frac12(F\pm{}^\star F),
$$

where ${}^\star H=H$ for a [self-dual differential form](../../../../../../self-dual-differential-form.md) and ${}^\star G=-G$ for an [anti-self-dual differential form](../../../../../../anti-self-dual-differential-form.md). The Hodge star is self-adjoint, so

$$
\langle H,G\rangle
=\langle{}^\star H,{}^\star G\rangle
=-\langle H,G\rangle=0.
$$

It follows that

$$
\boxed{H\wedge G=-H\wedge{}^\star G
=-\langle H,G\rangle\operatorname{vol}=0}.
$$

For an $SU(n)$ connection, use the positive norm

$$
\|F\|^2=-\int_{\mathbb R^4}\operatorname{Tr}(F\wedge{}^\star F)
$$

and define the [Second Chern number](../../../../../../second-chern-number.md) by

$$
k=-\frac1{8\pi^2}\int_{\mathbb R^4}\operatorname{Tr}(F\wedge F).
$$

Orthogonality gives

$$
\|F\|^2=\|F_+\|^2+\|F_-\|^2,
\qquad
8\pi^2k=\|F_+\|^2-\|F_-\|^2.
$$

Therefore the Euclidean [Yang-Mills action](../../../../../../yang-mills-action.md)

$$
S_{\rm YM}=\frac1{g_{\rm YM}^2}\|F\|^2
$$

obeys the [Yang-Mills instanton Bogomolny bound](../../../../../../yang-mills-instanton-bogomolny-bound.md)

$$
\boxed{S_{\rm YM}\geq\frac{8\pi^2}{g_{\rm YM}^2}|k|}.
$$

Equality holds precisely when $F_-=0$ or $F_+=0$, according to the sign of $k$; these are the self-dual and anti-self-dual [Yang-Mills instantons](../../../../../../yang-mills-instanton.md). Other trace and orientation conventions may reverse $k$ but leave the absolute-value bound unchanged.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 313](../../../paper-313-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
