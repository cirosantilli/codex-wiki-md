<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In three dimensions the [Sobolev embedding theorem](../../../../../../sobolev-embedding-theorem.md) gives

$$
H^2(U)\hookrightarrow L^\infty(U),
\qquad
H^2(U)\hookrightarrow W^{1,4}(U).
$$

Consequently, for $w\in H^2(U)\cap H_0^1(U)$,

$$
\||Dw|^2w\|_{L^2}
\leq\|Dw\|_{L^4}^2\|w\|_{L^\infty}
\leq C\|w\|_{H^2}^3.
$$

Thus $f+|Dw|^2w\in L^2(U)$. The [Dirichlet Poisson regularity theorem](../../../../../../dirichlet-poisson-regularity-theorem.md) on a bounded $C^2$ domain says that

$$
-\Delta v=f+|Dw|^2w,qquad v|_{\partial U}=0,
$$

has a unique $v\in H^2(U)\cap H_0^1(U)$ and

$$
\|v\|_{H^2}\leq C\bigl(\|f\|_2+\||Dw|^2w\|_2\bigr).
$$

**Hence $\Phi(w)=v$ is well defined.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
