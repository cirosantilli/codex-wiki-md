<h1 id="5/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Starting from $X$ at time $n$, the [markov property](../../../../../../../markov-property.md) and the time-independent transition rules give $\mathbb P(M_{2n}=X\mid M_n=X)=p_n$. Therefore

$$
\boxed{\mathbb P(M_n=X\mid M_{2n}=X)=\frac{\mathbb P(M_n=X,M_{2n}=X)}{p_{2n}}=\frac{p_n^2}{p_{2n}}.}
$$

Write $p_n=\frac34(\frac34)^n\left(1+\frac13(-\frac13)^n\right)$. The [conditional probability](../../../../../../../conditional-probability.md) becomes

$$
\frac34\frac{\left(1+\frac13(-\frac13)^n\right)^2}{1+\frac13(\frac19)^n}
\longrightarrow\boxed{\frac34}.
$$

The conditioning selects paths which have avoided the [absorbing state](../../../../../../../absorbing-state.md) up to time $2n$; it is therefore quite different from the unconditioned [probability](../../../../../../../probability.md) $p_n$, which tends to zero.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
