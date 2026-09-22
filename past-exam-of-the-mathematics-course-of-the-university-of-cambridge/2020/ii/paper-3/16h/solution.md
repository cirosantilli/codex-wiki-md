<h1 id="16h/solution">Solution</h1>

↑ **Parent:** [16H](../16h.md)

A [class in set theory](../../../../../class-set-theory.md) in the model $V$ is a collection

$$
C=\{x\in V:V\models\varphi(x,a_1,\ldots,a_k)\}
$$

defined by a first-order formula with parameters $a_i\in V$. A [set-theoretic class function](../../../../../set-theoretic-class-function.md) is a definable class relation $F$ for which every input in its domain has exactly one output. Informally, the [Axiom schema of replacement](../../../../../axiom-schema-of-replacement.md) says that the image $F``a$ of any set $a$ under any such function class is again a set.

Define the class function $F:\omega\to V$ by the [natural-number recursion theorem](../../../../../natural-number-recursion-theorem.md),

$$
F(0)=\omega,
\qquad
F(n+1)=\mathcal P(F(n)).
$$

Then $F(n)=z_n$, and [Replacement](../../../../../axiom-schema-of-replacement.md) applied to the set $\omega$ gives

$$
y=F``\omega=\{z_n:n\in\omega\}
$$

as a set.

Call a set small when it injects into some $z_n$. Every [natural number](../../../../../natural-number.md) $m$ is finite, and every member of $\operatorname{TC}(\{m\})$ is finite, so each injects into $z_0=\omega$. Hence $m\in\mathbf{HS}$. The set $\omega$ itself injects into $z_0$, and its hereditary members are natural numbers, so $\omega\in\mathbf{HS}$.

We next prove $z_n\in\mathbf{HS}$ by [mathematical induction](../../../../../mathematical-induction.md). The case $z_0=\omega$ was just proved. If $z_n\in\mathbf{HS}$ and $u\in z_{n+1}=\mathcal P(z_n)$, then $u\subseteq z_n$, so inclusion injects $u$ into $z_n$ and makes $u$ small. Every set below $u$ in its [transitive closure](../../../../../transitive-closure.md) is already below $z_n$ and is small by the induction hypothesis. The set $z_{n+1}$ itself injects into $z_{n+1}$. Thus every member of $\operatorname{TC}(\{z_{n+1}\})$ is small.

By [Cantor theorem](../../../../../cantor-s-theorem.md), $|z_{n+1}|>|z_n|$, so the $z_n$ are distinct and $z_n\mapsto n$ injects $y$ into $\omega=z_0$. Thus $y$ is small. Every other member of $\operatorname{TC}(\{y\})$ belongs to $\operatorname{TC}(\{z_n\})$ for some $n$, and is small by the preceding paragraph. Therefore $y\in\mathbf{HS}$. This proves the [finite-power-set hereditary-small construction](../../../../../finite-power-set-hereditary-small-construction.md).

The structure $(\mathbf{HS},\in)$ is not a model of ZF because it fails the [Axiom of union](../../../../../axiom-of-union.md). If $\bigcup y$ were small, it would inject into some $z_m$. But $z_{m+1}\subseteq\bigcup y$, since $z_{m+1}\in y$, so restriction would inject

$$
z_{m+1}=\mathcal P(z_m)\longrightarrow z_m.
$$

Together with the singleton injection $z_m\to\mathcal P(z_m)$, the [Cantor-Schröder-Bernstein theorem](../../../../../cantor-schroder-bernstein-theorem.md) would produce a bijection, contradicting [Cantor theorem](../../../../../cantor-s-theorem.md). Hence $\bigcup y$ is not small and therefore does not belong to $\mathbf{HS}$. Since $y\in\mathbf{HS}$ has no union inside the class, the Union axiom fails.

## ↑ Ancestors (10)

1. [16H](../16h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
