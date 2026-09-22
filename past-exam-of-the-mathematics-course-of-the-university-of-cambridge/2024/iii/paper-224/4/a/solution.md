<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an IID finite-alphabet source $Q$ and a fixed rate $H(Q)<R<\log_2|\mathcal A|$, let $P_e^*(n,R)$ be the smallest probability that a block is not represented by a fixed-to-fixed code having at most $2^{nR}$ codewords. The [fixed-rate source-coding error exponent](../../../../../../fixed-rate-source-coding-error-exponent.md) theorem states

$$
\lim_{n\to\infty}-\frac1n\log_2P_e^*(n,R)
=D^*(R,Q),
\qquad
D^*(R,Q)=\min_{P:H(P)\geq R}D(P\|Q).
$$

For the direct part, encode all type classes whose empirical entropy is at most $R-\delta_n$, where $\delta_n\downarrow0$ and $n\delta_n-|\mathcal A|\log_2(n+1)\to\infty$. Since a type class has at most $2^{nH(P)}$ sequences and there are at most $(n+1)^{|\mathcal A|}$ types, this codebook has at most $2^{nR}$ entries for large $n$. An error can occur only when $H(\widehat P_n)>R-\delta_n$. The [method of types](../../../../../../method-of-types.md) bounds its probability by

$$
(n+1)^{|\mathcal A|}
2^{-n\inf_{P:H(P)>R-\delta_n}D(P\|Q)}.
$$

Taking the lower limit of the exponent and using compactness and continuity gives at least $D^*(R,Q)$, proving achievability.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
