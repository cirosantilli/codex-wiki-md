<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use base-two logarithms and put $H=H(U_1)=-\sum_i p_i\log_2p_i$, with $0\log_2 0=0$. Zero-probability letters can be omitted. The random variables $I_j=-\log_2p_{U_j}$ are [self-information](../../../../../information-content.md) values, are IID, and have finite mean $H$ because the alphabet is finite. Independence gives

$$
-\log_2 P(U_1=u_1,\ldots,U_n=u_n)=\sum_{j=1}^n-\log_2p_{u_j}.
$$

For an arbitrary $\delta>0$, define the [typical set](../../../../../typical-set.md)

$$
T_{n,\delta}=\left\{u^{(n)}:P(u^{(n)})>0,\ \left|-\frac1n\log_2P(u^{(n)})-H\right|\le\delta\right\}.
$$

The [weak law of large numbers](../../../../../weak-law-of-large-numbers.md) implies $P(T_{n,\delta})\to1$. Every string in this set satisfies

$$
2^{-n(H+\delta)}\le P(u^{(n)})\le2^{-n(H-\delta)}.
$$

This is the [asymptotic equipartition property](../../../../../asymptotic-equipartition-property.md) for the given finite IID source, here obtained directly from the [weak law of large numbers](../../../../../weak-law-of-large-numbers.md).

For the upper bound, summing the lower bound on typical-string probabilities yields $|T_{n,\delta}|\le2^{n(H+\delta)}$. For sufficiently large $n$, its probability is at least $1-\varepsilon$, so it is an admissible set in the definition of $M(n,\varepsilon)$. Hence

$$
\limsup_{n\to\infty}\frac1n\log_2M(n,\varepsilon)\le H+\delta.
$$

For the lower bound, let $A$ be any admissible set and write $\eta_n=P(T_{n,\delta}^c)\to0$. Then

$$
P(A\cap T_{n,\delta})\ge1-\varepsilon-\eta_n.
$$

Each member of this intersection has probability at most $2^{-n(H-\delta)}$. Therefore, for all sufficiently large $n$,

$$
|A|\ge(1-\varepsilon-\eta_n)2^{n(H-\delta)}\ge\frac{1-\varepsilon}{2}\,2^{n(H-\delta)}.
$$

This applies in particular to a minimum-size admissible set, giving a liminf at least $H-\delta$. Letting $\delta\downarrow0$ proves both existence and the value of the [minimal high-probability source-set exponent](../../../../../minimal-high-probability-source-set-exponent.md):

$$
\boxed{\lim_{n\to\infty}\frac1n\log_2M(n,\varepsilon)=H(U_1)\qquad(0<\varepsilon<1).}
$$

For a deterministic source, $H=0$ and $M(n,\varepsilon)=1$, consistent with the formula.

For coding, label the strings in an admissible set with distinct binary indices of length $\lceil\log_2M(n,\varepsilon)\rceil$. A decoder reconstructs those strings exactly and may fail outside the set. Thus asymptotically $H$ bits per source symbol describe any fixed fraction $1-\varepsilon$ of the probability mass. More strongly, every rate $R>H$ permits block codes with error tending to zero: choose $\delta<R-H$, encode the typical strings individually and reserve one index for all other strings. The required number of indices is at most $2^{n(H+\delta)}+1\le2^{nR}$ for large $n$.

Conversely, a block encoder with at most $2^{nR}$ outputs can reconstruct at most that many distinct input strings correctly. If $R<H$, choose $0<\delta<H-R$. Its success probability is at most

$$
\eta_n+2^{nR}2^{-n(H-\delta)}\longrightarrow0.
$$

This gives the [strong converse for fixed-rate source coding](../../../../../strong-converse-for-fixed-rate-source-coding.md). It is the operational significance of the [information entropy](../../../../../information-entropy.md) limit for [reliable source encoding at a rate](../../../../../reliable-source-encoding-at-a-rate.md). The allowance of a small reconstruction error matters: a fixed-length code that must encode every possible string without error generally needs the larger rate $\log_2|\{i:p_i>0\}|$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
