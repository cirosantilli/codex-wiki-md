<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The derivative hypothesis implies that $1/Q(\xi)$ is a symbol of order $-\delta N$ at high frequency. Choose cutoffs $\chi\prec\psi$ in $X$ and a high-frequency cutoff in $\xi$. The corresponding Fourier multiplier is a [parametrix](../../../../../../parametrix.md) for $Q(D)$, and the [symbol calculus](../../../../../../symbol-calculus.md), together with the product formula from part (b), gives the localized estimate

$$
\|\chi u\|_{H^{s+\delta N}}
\leq C\left(\|\psi Q(D)u\|_{H^s}
+\|\psi u\|_{H^t}\right)
$$

for some sufficiently negative $t$. The commutator terms contain derivatives $Q^{(\alpha)}$; the assumed factor $|\xi|^{-\delta|\alpha|}$ lowers their order and lets them be absorbed inductively. Therefore

$$
\boxed{Q(D)u\in H^s_{\rm loc}(X)
\Longrightarrow u\in H^{s+\delta N}_{\rm loc}(X)}.
$$

If $Q(D)u$ is smooth, it belongs locally to $H^s$ for every $s$. Starting from the fact that every compactly supported distribution has some negative Sobolev order and repeatedly applying the gain $\delta N>0$ places $u$ in every local Sobolev space. The [Sobolev embedding theorem](../../../../../../sobolev-embedding-theorem.md) then gives $u\in C^\infty(X)$. Thus $Q(D)$ is a [hypoelliptic differential operator](../../../../../../hypoelliptic-operator.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 327](../../../paper-327-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
