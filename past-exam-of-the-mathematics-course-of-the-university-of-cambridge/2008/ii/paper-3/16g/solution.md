<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

A [transitive set](../../../../../transitive-set.md) $x$ satisfies $z\in y\in x\Rightarrow z\in x$, equivalently $\bigcup x\subseteq x$. If $x$ is transitive and $z\in y\in\bigcup x$, choose $w\in x$ with $y\in w$. Transitivity gives $y\in x$, so $z\in\bigcup x$. Thus $\bigcup x$ is transitive. If $z\in y\in\mathcal P(x)$, then $z\in x$ and transitivity implies $z\subseteq x$, whence $z\in\mathcal P(x)$. Thus the [power set](../../../../../power-set.md) is transitive as well.

The converse for the union is false: take $x=\{\{\varnothing\}\}$. Then $\bigcup x=\{\varnothing\}$ is transitive but $x$ is not. The power-set converse is true: if $z\in y\in x$, then $y\in\{y\}\in\mathcal P(x)$ implies $y\in\mathcal P(x)$, so $z\in x$.

Define $x_0=x$, $x_{n+1}=\bigcup x_n$ and $\operatorname{TC}(x)=\bigcup_{n<\omega}x_n$. This is a set by [replacement](../../../../../axiom-schema-of-replacement.md) and [union](../../../../../set-union.md), contains $x$ as a subset, and is transitive because taking a member advances one stage. Induction shows it is contained in every transitive set containing $x$, proving the [transitive closure](../../../../../transitive-closure.md) property.

If the [rank of a set](../../../../../rank-of-a-set.md) $x$ is $\alpha$, then

$$
\boxed{\operatorname{rank}\mathcal P(x)=\alpha+1,\qquad\operatorname{rank}\operatorname{TC}(x)=\alpha.}
$$

Every subset of $x$ has rank at most $\alpha$, and $x$ itself is an element of $\mathcal P(x)$, proving the first formula. The second is [transitive closure preserves set-theoretic rank](../../../../../transitive-closure-preserves-set-theoretic-rank.md). Here the convention is $x\subseteq\operatorname{TC}(x)$, not $x\in\operatorname{TC}(x)$.

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
