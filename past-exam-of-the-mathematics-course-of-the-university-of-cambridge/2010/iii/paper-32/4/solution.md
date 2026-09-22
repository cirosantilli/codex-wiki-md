<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $R$ be the total number of rejected [null hypotheses](../../../../../null-hypothesis.md), and let $V$ count rejected null hypotheses that are in fact true. The [false discovery proportion](../../../../../false-discovery-proportion.md) and [false discovery rate](../../../../../false-discovery-rate.md) are

$$
\boxed{\operatorname{FDP}=\frac{V}{R\vee1},\qquad \operatorname{FDR}=\mathbb E\left[\frac{V}{R\vee1}\right].}
$$

Thus the [false discovery proportion](../../../../../false-discovery-proportion.md) is zero when there are no rejections, and the [false discovery rate](../../../../../false-discovery-rate.md) averages the realized proportion of erroneous rejections.

For the [Benjamini-Hochberg procedure](../../../../../benjamini-hochberg-procedure.md), order the [p-values](../../../../../p-value.md) as $P_{(1)}\le\cdots\le P_{(m)}$ and define

$$
R=\max\bigl(\{k\in\{1,\ldots,m\}:P_{(k)}\le\alpha k/m\}\cup\{0\}\bigr).
$$

Reject every hypothesis whose [p-value](../../../../../p-value.md) satisfies $P_i\le\alpha R/m$ when $R>0$, and reject none otherwise. There are exactly $R$ such hypotheses: if a further [p-value](../../../../../p-value.md) also met the threshold, its larger rank would satisfy its own, still larger, threshold, contradicting maximality. Under the stated [independence](../../../../../independent-random-variables.md) and uniform true-null [p-values](../../../../../p-value.md), this procedure has [false discovery rate](../../../../../false-discovery-rate.md) $\alpha m_0/m\le\alpha$.

For the first modified [Benjamini-Hochberg procedure](../../../../../benjamini-hochberg-procedure.md), remove $P_1$, order the remaining $m-1$ [p-values](../../../../../p-value.md) as $Q_{(1)},\ldots,Q_{(m-1)}$, and use the shifted critical values $\alpha(j+1)/m$. Define its rejection count by

$$
R_{-1}=\max\bigl(\{j\in\{1,\ldots,m-1\}:Q_{(j)}\le\alpha(j+1)/m\}\cup\{0\}\bigr).
$$

Equivalently, insert a zero in place of $P_1$ and run the ordinary [Benjamini-Hochberg procedure](../../../../../benjamini-hochberg-procedure.md) on $m$ values; its total rejection count is $R^{(1)}=R_{-1}+1$. For $r=1,\ldots,m$, the [Benjamini-Hochberg leave-one-out identity](../../../../../benjamini-hochberg-leave-one-out-identity.md) in event form is

$$
\boxed{\{P_1\le\alpha r/m,\ R=r\}=\{P_1\le\alpha r/m,\ R_{-1}=r-1\}.}
$$

To prove it, suppose first that the left event holds. Then $P_1$ is among the rejected values. Lowering it to zero leaves all ordered [p-values](../../../../../p-value.md) at ranks greater than $r$ unchanged, so no new rank can meet its threshold. Rank $r$ still meets its threshold, giving $R^{(1)}=r$. Conversely, if $R^{(1)}=r$ and $P_1\le\alpha r/m$, the $r-1$ rejected remaining values and $P_1$ all meet the original rank-$r$ threshold. Hence the original count is at least $r$. Lowering a [p-value](../../../../../p-value.md) cannot decrease the rejection count, so the original count is also at most $R^{(1)}=r$. This proves equality of the events, including possible ties.

For the second modified [Benjamini-Hochberg procedure](../../../../../benjamini-hochberg-procedure.md), remove both $P_1,P_2$, order the remaining [p-values](../../../../../p-value.md) as $T_{(j)}$, and use shifted critical values $\alpha(j+2)/m$. Its count is

$$
R_{-12}=\max\bigl(\{j\in\{1,\ldots,m-2\}:T_{(j)}\le\alpha(j+2)/m\}\cup\{0\}\bigr).
$$

Replacing $P_1,P_2$ by zeros in the full procedure gives a total of $R^{(12)}=R_{-12}+2$ rejections. The same argument gives the [Benjamini-Hochberg leave-two-out identity](../../../../../benjamini-hochberg-leave-two-out-identity.md), for $r=2,\ldots,m$:

$$
\boxed{\{P_1\le\alpha r/m,\ P_2\le\alpha r/m,\ R=r\}
=\{P_1\le\alpha r/m,\ P_2\le\alpha r/m,\ R_{-12}=r-2\}.}
$$

In the forward direction both replaced values already lie among the first $r$, so ordered ranks greater than $r$ remain unchanged. In the reverse direction reinserting the two values below the rank-$r$ threshold still leaves at least $r$ qualifying values, while monotonicity under lowering bounds the original count above by $r$. For $r=1$, the event of two [p-values](../../../../../p-value.md) meeting the displayed threshold while only one is rejected is empty. For $m=1$ only the first modification is needed.

To calculate the second moment, write $I_i=\mathbf1\{i\text{ rejected}\}$ for a true null. Expanding the square gives

$$
V^2=\sum_{i=1}^{m_0}I_i+\sum_{\substack{1\le i,j\le m_0\\i\ne j}}I_iI_j.
$$

For a true-null index $i$, let $R_{-i}$ denote the first modified count after removing $P_i$. It is a function only of the remaining [p-values](../../../../../p-value.md), and so is independent of the uniform variable $P_i$. The first event identity therefore yields

$$
\mathbb E\frac{I_i}{(R\vee1)^2}
=\sum_{r=1}^m\frac1{r^2}\mathbb P(P_i\le\alpha r/m,\ R_{-i}=r-1)
=\frac\alpha m\sum_{r=1}^m\frac{\mathbb P(R_{-i}=r-1)}r
=\frac\alpha m\mathbb E\frac1{R_{-i}+1}.
$$

For distinct true-null indices $i,j$, the two independent uniform [p-values](../../../../../p-value.md) are independent of the second modified count $R_{-ij}$. The second event identity gives

$$
\mathbb E\frac{I_iI_j}{(R\vee1)^2}
=\sum_{r=2}^m\frac1{r^2}\left(\frac{\alpha r}{m}\right)^2\mathbb P(R_{-ij}=r-2)
=\frac{\alpha^2}{m^2}.
$$

The last sum is one because $R_{-ij}$ always takes a value in $\{0,\ldots,m-2\}$. The ordered pairs in the expansion of $V^2$ number $m_0(m_0-1)$, with no factor of one half.

The true-null [p-values](../../../../../p-value.md) are identically distributed and independent, so permutations among their indices leave the law of the full collection unchanged. Thus every $R_{-i}$ with $i\le m_0$ has the same distribution as $R_{-1}$, even though the false-null [p-values](../../../../../p-value.md) need not be identically distributed. Combining the diagonal and off-diagonal contributions proves the [second moment of the Benjamini-Hochberg false discovery proportion](../../../../../second-moment-of-the-benjamini-hochberg-false-discovery-proportion.md):

$$
\boxed{\mathbb E(\operatorname{FDP}^2)=\frac{\alpha m_0}{m}\mathbb E(A)+\frac{\alpha^2m_0(m_0-1)}{m^2},\qquad A=\frac1{R_{-1}+1}.}
$$

If the first modified count is instead defined to include the inserted zero, the same answer is $A=1/R^{(1)}$. When $m_0=0$, both sides are zero; when $m_0=1$, there are no off-diagonal terms. Finally, repeating the first calculation with denominator $R\vee1$ rather than its square gives $\mathbb E[I_i/(R\vee1)]=\alpha/m$, which verifies the claimed exact [false discovery rate](../../../../../false-discovery-rate.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
