<h1 id="6/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Fix $p$ and a name $\dot f$ such that $p$ forces a two-coloring of $[\lambda]^{<\omega}$. For each ground-model finite set $a\subseteq\lambda$, record its full [forcing decision pattern](../../../../../../../forcing-decision-pattern.md)

$$
F(a)(q)=\begin{cases}
0,&q\leq p\text{ and }q\Vdash\dot f(\check a)=0,\\
1,&q\leq p\text{ and }q\Vdash\dot f(\check a)=1,\\
2,&\text{otherwise}.
\end{cases}
$$

There are at most $3^{|\mathbb P|}<\lambda$ such patterns, since $\lambda$ is a [strong limit cardinal](../../../../../../../strong-limit-cardinal.md) and $|\mathbb P|<\lambda$. For finite $\mathbb P$ the number of patterns is finite, also below $\lambda$. Encode the patterns by an ordinal $\beta<\lambda$ and apply the assumed [finite-subset partition property](../../../../../../../finite-subset-partition-property.md) to obtain $H\subseteq\lambda$ of size $\lambda$ such that $F$ is constant on $[H]^n$ for every $n<\omega$.

For each $n$, choose one $a_n\in[H]^n$. Conditions below $p$ deciding $\dot f(a_n)$ are dense. Whenever one such condition decides the value, equality of patterns means it forces that same value at every $a\in[H]^n$. A [generic filter](../../../../../../../generic-filter.md) containing $p$ meets this dense set for each $n$, so $f$ is constant on each $[H]^n$ in the extension. The constants may differ with $n$, exactly as required.

The forcing has size below the regular $\lambda$, hence satisfies the $\lambda$-[chain condition for forcing](../../../../../../../chain-condition-for-forcing.md) and preserves its cardinality. The ground-model set $H$ consequently still has size $\lambda$. Since the argument works for every name and condition,

$$
\boxed{\Vdash_{\mathbb P}\lambda\rightarrow(\lambda)^{<\omega}_2.}
$$

This is [small forcing preservation of finite-subset partition properties](../../../../../../../small-forcing-preservation-of-finite-subset-partition-properties.md); no closure assumption on the forcing is required.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Paper 24](../../../../paper-24-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
