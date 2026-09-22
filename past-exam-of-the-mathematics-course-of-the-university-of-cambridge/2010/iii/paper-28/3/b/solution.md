<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $T$ swap coordinate blocks $0,\ldots,n$ and $n+1,\ldots,2n+1$, fixing all other coordinates. The symmetric law makes $T$ measure preserving, and invariance of the event $A$ gives $F\circ T=F$ pointwise. Put $\mathcal B_n=\sigma(X_{n+1},\ldots,X_{2n+1})$.

Conditional expectation transforms covariantly under this block swap:

$$
\mathbb E[F\mid\mathcal E_n]\circ T=\mathbb E[F\mid\mathcal B_n]\quad\text{almost surely}.
$$

To check it, the left side is $\mathcal B_n$-measurable, and for $C\in\mathcal B_n$ the change of variables by $T$ sends its defining integral to the conditional-expectation identity on $T(C)\in\mathcal E_n$, with $F\circ T=F$. Thus the two versions agree. Measure preservation now gives

$$
\boxed{\|F-\mathbb E[F\mid\mathcal B_n]\|_1
=\|F-\mathbb E[F\mid\mathcal E_n]\|_1\leq\varepsilon.}
$$

This is the first requested estimate.

The [L1 contraction of conditional expectation](../../../../../../l1-contraction-of-conditional-expectation.md) follows from the pointwise bound $|\mathbb E[Z\mid\mathcal H]|\leq\mathbb E[|Z|\mid\mathcal H]$: take expectations to get $\|\mathbb E[Z\mid\mathcal H]\|_1\leq\|Z\|_1$. Applied to a difference, it makes conditional expectation a contraction between any two integrable inputs.

Let $U_n=\mathbb E[F\mid\mathcal B_n]$. Since $\mathcal B_n\subseteq\mathcal G_n$, $U_n$ is $\mathcal G_n$-measurable. Hence

$$
\|F-\mathbb E[F\mid\mathcal G_n]\|_1
\leq\|F-U_n\|_1+\|\mathbb E[U_n-F\mid\mathcal G_n]\|_1
\leq2\varepsilon.
$$

Combining this with the other given approximation bound yields

$$
\|F-\mathbb E[F\mid\mathcal G]\|_1\leq3\varepsilon.
$$

The left side does not depend on $n$, and $\varepsilon>0$ was arbitrary. It is therefore zero. For a $\mathcal G$-measurable version $Y=\mathbb E[F\mid\mathcal G]$, the event $C=\{Y>1/2\}$ belongs to $\mathcal G$ and satisfies

$$
\boxed{\mathbb P(A\mathbin{\triangle}C)=0.}
$$

This proves that [exchangeable invariant events are tail events modulo null sets](../../../../../../exchangeable-invariant-events-are-tail-events-modulo-null-sets.md). It does not assert literal pointwise equality of the two events or sigma-algebras before completing them with null sets.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
