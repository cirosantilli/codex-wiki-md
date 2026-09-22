<h1 id="16h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Axiom of foundation](../../../../../../axiom-of-regularity.md) says that every nonempty set $A$ contains an $x$ with $x\cap A=\varnothing$. The principle of [epsilon induction](../../../../../../epsilon-induction.md) says that if a formula $\varphi$ is progressive,

$$
\forall x\left[
(\forall y\in x,\ \varphi(y))\Longrightarrow\varphi(x)
\right],
$$

then $\varphi$ holds for every set.

Assume foundation and let $\varphi$ be progressive. If $\varphi(a)$ failed for some $a$, use [separation](../../../../../../axiom-schema-of-specification.md) to form the nonempty set of failures inside $\operatorname{TC}(\{a\})$. Foundation supplies an $\in$-minimal failure $x$. Every member of $x$ lies in the transitive closure and is not a failure, so progressiveness gives $\varphi(x)$, a contradiction. Hence epsilon induction holds.

Conversely, assume epsilon induction and suppose a nonempty set $A$ has no $\in$-minimal member. Let

$$
\varphi(x)\quad\Longleftrightarrow\quad x\notin A.
$$

If every member of $x$ satisfies $\varphi$ but $x\in A$, then $x\cap A=\varnothing$, making $x$ an $\in$-minimal member of $A$, contrary to the assumption. Thus $\varphi$ is progressive. Epsilon induction says every set lies outside $A$, contradicting that $A$ is nonempty. Foundation follows.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [16H](../../16h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
