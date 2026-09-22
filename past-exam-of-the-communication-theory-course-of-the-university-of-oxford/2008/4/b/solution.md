<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [redundancy](../../../../redundancy-of-a-binary-prefix-code.md) is $R=\bar\ell-H(X)$, measured in bits per source symbol. Write $s_v=\sigma_0(v)+\sigma_1(v)$ for the total mass passing through interior node $v$. Counting each [codeword](../../../../codeword.md)'s length as one for each interior node its route visits gives

$$
\bar\ell=\sum_xp_x\sum_{v\text{ on its route}}1=\sum_{v\in N}s_v.
$$

The [entropy](../../../../information-entropy-split.md) can be split into the conditional binary decisions along that route. Algebraically each node contributes

$$
s_v h(\sigma_0(v)/s_v)=s_v\log_2s_v-\sigma_0(v)\log_2\sigma_0(v)-\sigma_1(v)\log_2\sigma_1(v).
$$

Summing telescopes: each non-root interior mass appears once positively as a parent and once negatively as a child. The root term is $1\log_21=0$ and the remaining leaf terms sum to $-\sum_xp_x\log_2p_x=H(X)$. Hence

$$
H(X)=\sum_{v\in N}s_vh(\sigma_0(v)/s_v).
$$

Subtracting this identity from the expected-length identity proves

$$
\boxed{R=\sum_{v\in N}(\sigma_0(v)+\sigma_1(v))\left[1-h\!\left(\frac{\sigma_0(v)}{\sigma_0(v)+\sigma_1(v)}\right)\right]}.
$$

Thus [redundancy](../../../../redundancy-of-a-binary-prefix-code.md) is the sum of the probability-weighted imbalances of the binary branch decisions. Nodes with no mass contribute zero by [continuity](../../../../continuous-function.md). The formula holds for every full prefix tree, even without optimality.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the communication Theory course of the University of Oxford](../../../split.md)
5. [Communication Theory course of the University of Oxford](../../../../communication-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
