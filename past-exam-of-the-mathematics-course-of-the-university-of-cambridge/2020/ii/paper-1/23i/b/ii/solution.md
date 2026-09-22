<h1 id="23i/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For every positive integer $k$, additivity gives $f(kx)=kf(x)$. Hence

$$
x\in f^{-1}(B_\varepsilon)
\implies kx\in f^{-1}(B_{k\varepsilon}).
$$

Conversely, if $z\in f^{-1}(B_{k\varepsilon})$, write $z=k(z/k)$. Then

$$
k|f(z/k)|=|f(z)|<k\varepsilon,
$$

so $z/k\in f^{-1}(B_\varepsilon)$. Thus

$$
\boxed{f^{-1}(B_{k\varepsilon})=k f^{-1}(B_\varepsilon)}.
$$

To prove continuity, fix $\varepsilon>0$ and put

$$
E_k=f^{-1}(B_{k\varepsilon/2}).
$$

These sets are [measurable](../../../../../../../lebesgue-measurable-set.md) and $\mathbb R^n=\bigcup_{k\ge1}E_k$, so at least one $E_k$ has positive [Lebesgue measure](../../../../../../../lebesgue-measure.md). Part (ii) gives $E_k=kE_1$, and therefore $E_1$ also has positive measure. By the [Steinhaus theorem](../../../../../../../steinhaus-theorem.md), $E_1-E_1$ contains an open neighbourhood $U$ of zero. Part (i) gives

$$
U\subseteq E_1-E_1
\subseteq f^{-1}(B_\varepsilon).
$$

This proves continuity at zero. Finally,

$$
f(x+h)-f(x)=f(h)\longrightarrow0
$$

as $h\to0$, so $f$ is continuous at every $x$. Thus every such map is an instance of the theorem that a [measurable additive function is continuous](../../../../../../../measurable-additive-function-is-continuous.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [23I](../../../23i.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
