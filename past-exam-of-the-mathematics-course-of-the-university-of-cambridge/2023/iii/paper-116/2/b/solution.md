<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\mathrm{IC}$ be the sentence asserting that a [strongly inaccessible cardinal](../../../../../../strongly-inaccessible-cardinal.md) exists, and begin with

$$
T_0=\mathrm{ZFC}+\mathrm{IC}.
$$

Define the [iterated consistency progression](../../../../../../iterated-consistency-progression.md)

$$
T_{n+1}=T_n+\operatorname{Con}(T_n),
\qquad
T_\infty=\bigcup_{n<\omega}T_n.
$$

The construction is effective, so every $T_n$ and $T_\infty$ is a recursively axiomatized [first-order theory](../../../../../../first-order-theory.md) extending ZFC.

Because $T_{n+1}$ extends $T_n$, every theorem of $T_n$, including every [formal consistency statement](../../../../../../formal-consistency-statement.md) it proves, is a theorem of $T_{n+1}$; hence $T_n\leq_{\mathrm{Cons}}T_{n+1}$. The theory $T_{n+1}$ proves $\operatorname{Con}(T_n)$ by construction, whereas a consistent $T_n$ cannot prove its own consistency by [Gödel second incompleteness theorem](../../../../../../godel-second-incompleteness-theorem.md). Therefore

$$
T_n<_{\mathrm{Cons}}T_{n+1}.
$$

Likewise $T_\infty$ extends every $T_n$ and contains $\operatorname{Con}(T_n)$ as an axiom already at stage $n+1$, while $T_n$ does not prove it. Consequently

$$
T_0<_{\mathrm{Cons}}T_1<_{\mathrm{Cons}}T_2<_{\mathrm{Cons}}\cdots<_{\mathrm{Cons}}T_\infty,
$$

assuming the stated consistency hypotheses.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 116](../../../paper-116-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
