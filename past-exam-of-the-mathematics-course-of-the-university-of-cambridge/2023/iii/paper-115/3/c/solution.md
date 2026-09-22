<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a path $\gamma:[0,1]\to B$, a section $s(t)$ of $\gamma^*E$ is parallel when

$$
\dot s+A(\dot\gamma)s=0.
$$

Existence and uniqueness for this linear ordinary differential equation define the [parallel transport](../../../../../../parallel-transport.md)

$$
\mathcal P_\gamma^{\mathcal A}:E_{\gamma(0)}\longrightarrow E_{\gamma(1)}.
$$

Transport along the reversed path solves the inverse initial-value problem, so

$$
\mathcal P_{\bar\gamma}^{\mathcal A}
=(\mathcal P_\gamma^{\mathcal A})^{-1}.
$$

If $P(t)$ denotes transport from $0$ to $t$, then

$$
\mu(t)=P(t)\mu(0)P(t)^{-1}
$$

satisfies the horizontal equation for the induced endomorphism connection. Uniqueness therefore gives

$$
\boxed{\mathcal P_\gamma^{\operatorname{End}(\mathcal A)}(\mu)
=\mathcal P_\gamma^{\mathcal A}\,
\mu\,
(\mathcal P_\gamma^{\mathcal A})^{-1}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
