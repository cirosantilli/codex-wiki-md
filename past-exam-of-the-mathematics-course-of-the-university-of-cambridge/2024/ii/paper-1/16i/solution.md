<h1 id="16i/solution">Solution</h1>

↑ **Parent:** [16I](../16i.md)

The [soundness theorem for propositional logic](../../../../../soundness-theorem-for-propositional-logic.md) says that if $\Gamma\vdash t$, then every valuation satisfying every member of $\Gamma$ also satisfies $t$.

The proposed [function](../../../../../function-split.md) need not respect the connectives. For example, if a primitive proposition $p$ is independent of $S$, then neither $p$ nor $\neg p$ is provable from $S$, so the definition gives

$$
v(p)=v(\neg p)=0.
$$

Order the consistent supersets of $S$ by inclusion. The union of a chain is consistent, since a finite proof of a contradiction would already use assumptions from one member of the chain. [Zorn lemma](../../../../../zorn-s-lemma.md) therefore gives a maximal consistent extension $T$. It is deductively closed: if $T\vdash t$, adjoining $t$ preserves consistency, so maximality forces $t\in T$. Moreover, for every $t$, exactly one of $t$ and $\neg t$ belongs to $T$. They cannot both belong by consistency; if neither belonged, the inconsistency of both proper extensions would give $T\vdash\neg t$ and $T\vdash\neg\neg t$, again a contradiction. The usual induction on formulae now shows that

$$
v(t)=1\quad\Longleftrightarrow\quad t\in T
$$

defines a valuation satisfying $T$, and hence $S$.

Now suppose every finite subset of $S$ has a model. By soundness every finite subset is consistent. Any proof of a contradiction from $S$ uses only finitely many assumptions, so $S$ itself is consistent. Applying the preceding maximal-consistent-extension construction gives a model of $S$. This proves the [propositional compactness theorem](../../../../../propositional-compactness-theorem.md).

## ↑ Ancestors (10)

1. [16I](../16i.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
