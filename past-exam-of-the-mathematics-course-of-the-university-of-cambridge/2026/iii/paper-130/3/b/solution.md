<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\forall_{\mathcal U}x\,\varphi(x)$ to mean $\{x:\varphi(x)\}\in\mathcal U$. For each $x$, exactly one of the red-neighbour set $R_x$ and the blue-neighbour set $B_x$ belongs to $\mathcal U$. Applying the ultrafilter dichotomy once more to

$$
\{x:R_x\in\mathcal U\}
$$

shows that exactly one of

$$
\forall_{\mathcal U}x\,\forall_{\mathcal U}y
\ (xy\text{ is red}),
\qquad
\forall_{\mathcal U}x\,\forall_{\mathcal U}y
\ (xy\text{ is blue})
$$

holds. They cannot both hold because the two outer sets are complementary; the diagonal causes no problem because a nonprincipal ultrafilter contains no singleton.

Assume the red statement and put $X=\{x:R_x\in\mathcal U\}\in\mathcal U$. Choose $x_1\in X$. Recursively choose

$$
x_n\in X\cap\bigcap_{i<n}R_{x_i}
$$

outside the finitely many previously chosen points. Every set in this finite intersection belongs to $\mathcal U$, so a choice is always possible. Then $M=\{x_1,x_2,\ldots\}$ is infinite and all of its edges are red.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
