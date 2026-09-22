<h1 id="3h/solution">Solution</h1>

↑ **Parent:** [3H](../3h.md)

Let a memoryless source have probabilities $p_1,\ldots,p_m$, and let a uniquely decodable $D$-ary code have word lengths $\ell_i$ and mean length $L=\sum_i p_i\ell_i$. The [Shannon source coding theorem](../../../../../shannon-s-source-coding-theorem.md) states

$$
H_D(p)\leq L,
\qquad
H_D(p)=-\sum_i p_i\log_Dp_i,
$$

and that some [prefix code](../../../../../prefix-code.md) satisfies

$$
H_D(p)\leq L<H_D(p)+1.
$$

For the lower bound, the [Kraft inequality](../../../../../kraft-mcmillan-inequality.md) gives $K=\sum_iD^{-\ell_i}\leq1$. Set $q_i=D^{-\ell_i}/K$. The [Gibbs inequality](../../../../../gibbs-inequality.md), or nonnegativity of [relative entropy](../../../../../kullback-leibler-divergence.md), gives

$$
0\leq\sum_i p_i\log_D\frac{p_i}{q_i}
=-H_D(p)+L+\log_DK.
$$

Therefore $L\geq H_D(p)-\log_DK\geq H_D(p)$.

For achievability choose $\ell_i=\lceil-\log_Dp_i\rceil$. Then $\sum_iD^{-\ell_i}\leq\sum_ip_i=1$, so the converse part of the Kraft theorem supplies a prefix code with these lengths, and

$$
L<\sum_i p_i(-\log_Dp_i+1)=H_D(p)+1.
$$

**Hence the entropy is the optimal mean code length up to less than one code symbol.**

## ↑ Ancestors (10)

1. [3H](../3h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
