<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the tilted probability measure $Q$ by $dQ=Z\,dP$; this is normalized because $\mathbb EZ=1$. Then

$$
\operatorname{Ent}_P(Z)=\mathbb E_P[Z\log Z]=D(Q\Vert P).
$$

Let $\mathbb E_i$ average only coordinate $i$, keeping $X^{(i)}$ fixed. The marginal density of $Q_{X^{(i)}}$ relative to $P_{X^{(i)}}$ is $\mathbb E_iZ$, and hence

$$
D(Q_{X^{(i)}}\Vert P_{X^{(i)}})
=\operatorname{Ent}_P(\mathbb E_iZ).
$$

Moreover,

$$
\mathbb E_P\operatorname{Ent}_i(Z)
=\operatorname{Ent}_P(Z)-\operatorname{Ent}_P(\mathbb E_iZ).
$$

Substituting [Han's inequality for relative entropy](../../../../../../han-s-inequality-for-relative-entropy.md) and rearranging gives the [tensorization of entropy](../../../../../../tensorization-of-entropy.md)

$$
\boxed{\operatorname{Ent}_P(Z)
\leq\sum_{i=1}^n\mathbb E_P\operatorname{Ent}_i(Z).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
