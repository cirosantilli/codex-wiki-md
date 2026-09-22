<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $S=R\setminus P$. If $Q\subseteq P$ is a [prime ideal](../../../../../../prime-ideal.md), then $Q\cap S=\varnothing$. Its extension is

$$
QR_P=\{q/s:q\in Q,\ s\in S\}.
$$

It is proper: $1=q/s$ would give $u(s-q)=0$ for some $u\in S$, and hence $us=uq\in Q$, impossible because $u,s\notin Q$. If a product $(a/s)(b/t)$ lies in $QR_P$, clearing a denominator gives $uab\in Q$ for some $u\in S$. Primeness and $u\notin Q$ imply $a\in Q$ or $b\in Q$. Thus $QR_P$ is prime. Its contraction is $Q$, since $r/1\in QR_P$ implies $ur\in Q$ for some $u\in S$, forcing $r\in Q$.

Conversely, contract a [prime ideal](../../../../../../prime-ideal.md) $\mathfrak q$ of $R_P$ to $Q=\{r:r/1\in\mathfrak q\}$. This is a [prime ideal](../../../../../../prime-ideal.md) of $R$. It contains no element of $S$, since such an element becomes a [unit](../../../../../../unit-in-a-ring.md) and cannot belong to the proper [ideal](../../../../../../ideal.md) $\mathfrak q$. Hence $Q\subseteq P$. Also $r/s\in\mathfrak q$ exactly when $r/1\in\mathfrak q$, because $s/1$ is a [unit](../../../../../../unit-in-a-ring.md), so $\mathfrak q=QR_P$. These extension and contraction operations are inverse, giving the [prime ideal correspondence for localization](../../../../../../prime-ideal-correspondence-for-localization.md):

$$
\boxed{\operatorname{Spec}(R_P)\longleftrightarrow\{Q\in\operatorname{Spec}R:Q\subseteq P\},\qquad Q\mapsto QR_P.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
