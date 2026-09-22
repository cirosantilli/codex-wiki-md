<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

One useful form of the [modified logarithmic Sobolev inequality](../../../../../../modified-logarithmic-sobolev-inequality.md) is the following. For a function $F$ of independent coordinates, let

$$
F_i(x^{(i)})=\inf_{z\in[0,1]}F(x_1,\ldots,x_{i-1},z,x_{i+1},\ldots,x_n)
$$

and $V^+(x)=\sum_i(F(x)-F_i(x^{(i)}))^2$. If $V^+\leq v$ and $\lambda\geq0$, the inequality gives

$$
\operatorname{Ent}(e^{\lambda F})
\leq\frac{\lambda^2v}{2}\mathbb Ee^{\lambda F},
$$

and the [Herbst argument](../../../../../../herbst-argument.md) yields

$$
\mathbb P(F-\mathbb EF\geq t)\leq e^{-t^2/(2v)}.
$$

[Talagrand's one-sided bounded differences inequality](../../../../../../talagrand-s-one-sided-bounded-differences-inequality.md) gives the complementary tail under the same one-sided bounded-difference condition:

$$
\mathbb P(F-\mathbb EF\leq-t)\leq e^{-t^2/(2v)}.
$$

Equivalent versions use an independent coordinate replacement and its conditional positive-part variance proxy.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
