<h1 id="1f/solution">Solution</h1>

↑ **Parent:** [1F](../1f.md)

A [basis](../../../../../basis.md) of a [vector space](../../../../../vector-space-split.md) $V$ is a family of vectors that is both [linearly independent](../../../../../linear-independence.md) and a [spanning set](../../../../../spanning-set.md) of $V$.

Write the given finite basis as $\mathcal B=\{v_1,\ldots,v_n\}$. First, any other basis $\mathcal B'$ must also be finite. Each $v_i$ is a finite [linear combination](../../../../../linear-combination.md) of elements of $\mathcal B'$, so the union $S$ of the finitely many elements of $\mathcal B'$ occurring in these $n$ expressions is finite. Since $S$ spans every $v_i$, it spans $V$. If some $w\in\mathcal B'\setminus S$ existed, then $w$ would lie in the span of $S$, contradicting the [linear independence](../../../../../linear-independence.md) of $\mathcal B'$. Hence $\mathcal B'=S$; write $|\mathcal B'|=m$.

It remains to prove the elementary [Steinitz exchange lemma](../../../../../steinitz-exchange-lemma.md) directly. If independent vectors $w_1,\ldots,w_r$ lie in the span of $v_1,\ldots,v_n$, express $w_1$ in terms of the $v_i$. Some coefficient is nonzero, so the corresponding $v_i$ can be solved for in terms of $w_1$ and the other $v_i$; replacing it by $w_1$ preserves the span. Inductively, after replacing $k$ of the $v_i$ by $w_1,\ldots,w_k$, the expression for $w_{k+1}$ must have a nonzero coefficient on one of the unreplaced $v_i$, since otherwise $w_{k+1}$ would be a linear combination of $w_1,\ldots,w_k$. That $v_i$ can again be replaced. There are only $n$ original vectors to replace, so $r\leq n$.

Apply this argument first to the independent family $\mathcal B'$ and the spanning family $\mathcal B$ to obtain $m\leq n$, and then with the two bases interchanged to obtain $n\leq m$. Therefore

$$
\boxed{|\mathcal B'|=|\mathcal B|}.
$$

## ↑ Ancestors (10)

1. [1F](../1f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
