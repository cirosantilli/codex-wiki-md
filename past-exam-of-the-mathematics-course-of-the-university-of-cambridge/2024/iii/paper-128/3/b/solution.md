<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume the forcing relation and the forcing theorem have been constructed for $\varphi(x,\vec y)$. Define

$$
p\Vdash\exists x\,\varphi(x,\vec\tau)
$$

to mean that

$$
D_p=\{q\le p:\exists\sigma\in M\;q\Vdash\varphi(\sigma,\vec\tau)\}
$$

is dense below $p$. This definition is first-order over $M$, so the definability lemma is preserved.

Suppose $p\in G$ forces the existential statement. Genericity below $p$ gives $q\in G\cap D_p$ and a name $\sigma$ with $q\Vdash\varphi(\sigma,\vec\tau)$. The truth lemma for $\varphi$ yields

$$
M[G]\models\varphi(\sigma^G,\vec\tau^G),
$$

so the existential statement is true. Conversely, if $M[G]\models\exists x\,\varphi(x,\vec\tau^G)$, choose a name $\sigma$ for a witness. The truth lemma for $\varphi$ gives $q\in G$ with $q\Vdash\varphi(\sigma,\vec\tau)$, and then $q\Vdash\exists x\,\varphi(x,\vec\tau)$. This proves both directions of the forcing theorem for the existential formula.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 128](../../../paper-128-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
