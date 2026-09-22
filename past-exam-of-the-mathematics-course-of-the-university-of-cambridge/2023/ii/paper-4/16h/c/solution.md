<h1 id="16h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let

$$
i:K\times L\longrightarrow K\sqcup L
$$

be the injection witnessing $\kappa\lambda\leq\kappa+\lambda$, and fix $(k_*,l_*)\in K\times L$. Extend the inverse of $i$ to a surjection

$$
p:K\sqcup L\longrightarrow K\times L
$$

by setting

$$
p(z)=
\begin{cases}
i^{-1}(z),&z\in i[K\times L],\\
(k_*,l_*),&z\notin i[K\times L].
\end{cases}
$$

This construction uses only the fixed pair, not the [axiom of choice](../../../../../../axiom-of-choice.md).

Restrict $p$ to the $K$-summand and take its second coordinate:

$$
r:K\longrightarrow L,
\qquad r(k)=\pi_L(p(k,0)).
$$

If $r$ is onto, it is the required [surjective function](../../../../../../surjective-function.md) from $K$ to $L$.

Otherwise choose one $l_0\in L\setminus r[K]$. For each $k\in K$, surjectivity of $p$ gives a preimage of $(k,l_0)$. No such preimage lies in the $K$-summand, by the choice of $l_0$, so it lies in the $L$-summand. Unless $(k,l_0)=(k_*,l_*)$, this preimage is exactly $i(k,l_0)$ and is unique: all points outside the range of $i$ map only to the default pair. Distinct $k$ give distinct preimages because $i$ is injective.

If $l_0\ne l_*$, these unique preimages therefore define an [injective function](../../../../../../injective-function.md) $K\to L$. The only exceptional case is $l_0=l_*$, where they initially define an injection

$$
j:K\setminus\{k_*\}\longrightarrow L.
$$

If $j$ is onto, extend it arbitrarily at $k_*$ to obtain a surjection $K\to L$. If it is not onto, choose one $l'\in L\setminus j[K\setminus\{k_*\}]$ and set $j(k_*)=l'$; this gives an injection $K\to L$. These cases prove the [product-sum comparison lemma](../../../../../../product-sum-comparison-lemma.md) entirely in ZF.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [16H](../../16h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
