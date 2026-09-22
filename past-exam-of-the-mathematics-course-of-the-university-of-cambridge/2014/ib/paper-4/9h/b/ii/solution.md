<h1 id="9h/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Starting from $Y_{n-2}=0$ forces $X_{n-2}=0$. The first nonzero value is consequently $X_{n-1}=-1$. Remaining nonzero at the next step forces $X_n=1$, because $p_{-1,-1}=0$. Hence, on an event of positive probability,

$$
 \boxed{\mathbb P(Y_{n+1}=0\mid Y_n=1,Y_{n-1}=1,Y_{n-2}=0)=p_{1,0}.}
$$

The two values are unequal by assumption. They expose memory of the hidden sign: immediately after leaving zero the sign is negative, whereas after two consecutive nonzero observations it is positive. Whenever the relevant observed histories coexist with positive probability, the [Markov property](../../../../../../../markov-property.md) for $Y$ fails, since its next-step law is not determined by its present value alone. In particular, the absolute-value projection does not preserve the [Markov property](../../../../../../../markov-property.md) for all initial laws; the [strong lumpability](../../../../../../../strong-lumpability.md) condition would require $p_{-1,0}=p_{1,0}$.

There is a small qualification to a blanket conclusion about an unspecified initial law. The printed assumptions do not ensure that either conditioning event is possible, and a degenerate initial law may never reach the hidden states that cause the failure. For example, in the order $-1,0,1$, take

$$
 P=\begin{pmatrix}0&1&0\\0&1&0\\0&0&1\end{pmatrix},\qquad X_0=0.
$$

All printed constraints hold, yet $Y_n=0$ always and is a [Markov chain](../../../../../../../markov-chain.md). Thus the correct general conclusion is **the transformed process is not necessarily Markov**; the two computed probabilities give the intended failure when their histories are available.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [9H](../../../9h.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ib](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
