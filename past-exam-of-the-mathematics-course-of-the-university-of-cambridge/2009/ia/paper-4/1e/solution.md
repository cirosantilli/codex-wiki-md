<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

Write $\Delta_A=\{(x,x):x\in A\}$ and regard each [binary relation](../../../../../binary-relation.md) as a subset of $A\times A$. Then $R=Q\cup\Delta_A$ is the [reflexive closure](../../../../../reflexive-closure.md) of $Q$: every $x\in A$ satisfies $xRx$ because $x=x$. The relation $S=R\cup R^{-1}$ is its [symmetric closure](../../../../../symmetric-closure.md). It is a [reflexive relation](../../../../../reflexive-relation.md) since it contains $R$, and $xSy$ means either $xRy$ or $yRx$, either of which also gives $ySx$.

For $T$, a one-step chain $(x,x)$ is allowed because $xSx$, so $xTx$. If $(x_0,\ldots,x_n)$ witnesses $xTy$, the reversed chain $(x_n,\ldots,x_0)$ witnesses $yTx$, since $S$ is a [symmetric relation](../../../../../symmetric-relation.md). Finally, concatenate a chain from $x$ to $y$ with a chain from $y$ to $z$ to obtain a positive-length chain from $x$ to $z$. Hence $T$ is a [transitive relation](../../../../../transitive-relation.md) as well, and

$$
\boxed{R\text{ is reflexive},\quad S\text{ is reflexive and symmetric},\quad T\text{ is an equivalence relation}.}
$$

Thus $T$ is the [transitive closure of a relation](../../../../../transitive-closure-relation.md) applied to $S$.

Now suppose $E$ is an [equivalence relation](../../../../../equivalence-relation.md) containing $Q$. Its reflexivity implies $\Delta_A\subseteq E$, hence $R\subseteq E$. Its symmetry then implies $R^{-1}\subseteq E$, hence $S\subseteq E$. Along a chain witnessing $xTy$, every consecutive pair is $E$-related. Induction on the chain length using [transitivity](../../../../../transitive-relation.md) gives $xEy$: the one-step case is $S\subseteq E$, and the last step joins $xEx_{n-1}$ to $x_{n-1}Ey$. Therefore

$$
\boxed{T\subseteq E\text{ for every equivalence relation }E\supseteq Q.}
$$

Together with $Q\subseteq T$, this proves that $T$ is exactly the [equivalence closure](../../../../../equivalence-closure.md) of $Q$. The reasoning also covers an empty $A$, where all assertions about elements are vacuous.

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
