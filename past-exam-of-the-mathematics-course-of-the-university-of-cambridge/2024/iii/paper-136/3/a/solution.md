<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A Lubin–Tate series for $\pi$ is a power series $f(X)\in\mathcal O_K[[X]]$ such that

$$
f(X)\equiv\pi X\pmod{X^2},
\qquad
f(X)\equiv X^q\pmod\pi.
$$

The key Lubin–Tate lemma is that if $f$ and $g$ are such series and $L(X_1,\ldots,X_r)=\sum_i a_iX_i$ with $a_i\in\mathcal O_K$, there is a unique series $F\in\mathcal O_K[[X_1,\ldots,X_r]]$ satisfying

$$
F\equiv L\pmod{(X_1,\ldots,X_r)^2},
\qquad
F(f(X_1),\ldots,f(X_r))=g(F(X_1,\ldots,X_r)).
$$

Taking $g=f$ and $L=X+Y$ defines $\mathcal F_f(X,Y)$. Uniqueness applied to the two sides of each identity proves the identity, associativity, and commutativity axioms, so $\mathcal F_f$ is a [formal group law](../../../../../../formal-group-law.md). Taking $L=aX$ defines endomorphisms $[a]_f$, and uniqueness gives

$$
[a+b]_f=\mathcal F_f([a]_f,[b]_f),
\qquad
[ab]_f=[a]_f\circ[b]_f.
$$

Thus $\mathcal F_f$ is the [Lubin–Tate formal group](../../../../../../lubin-tate-formal-group.md) as a formal $\mathcal O_K$-module, with $[\pi]_f=f$.

For another Lubin–Tate series $g$, apply the lemma with $L=X$ to obtain

$$
h(X)\equiv X\pmod{X^2},
\qquad h\circ f=g\circ h.
$$

Uniqueness shows that $h$ respects both formal addition and every scalar endomorphism. Its linear coefficient is the unit one, so it has a compositional inverse; equivalently, applying the lemma with $f$ and $g$ reversed supplies the inverse. Hence this [Lubin–Tate change of series](../../../../../../lubin-tate-change-of-series.md) is an isomorphism $\mathcal F_f\cong\mathcal F_g$ of formal $\mathcal O_K$-modules.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 136](../../../paper-136-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
