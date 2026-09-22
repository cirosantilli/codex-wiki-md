<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume the two response labels are distinct and the error probability is the same for each stimulus. Then the stimulus-response map is a [binary symmetric channel](../../../../../../binary-symmetric-channel.md):

$$
\mathbb P(R=r_+\mid S=+)=\mathbb P(R=r_-\mid S=-)=1-P_x,
$$

with the two incorrect conditional probabilities equal to $P_x$. Equal stimulus probabilities give $\mathbb P(R=r_+)=\mathbb P(R=r_-)=1/2$. In bits, the [Shannon entropy](../../../../../../information-entropy.md) of the response is therefore $H(R)=1$. For either stimulus the response entropy is the [binary entropy](../../../../../../binary-entropy.md)

$$
h_2(P_x)=-P_x\log_2P_x-(1-P_x)\log_2(1-P_x),
$$

with $0\log0=0$. Thus $H_{\mathrm{noise}}=H(R\mid S)=h_2(P_x)$, and the [mutual information](../../../../../../mutual-information.md) is

$$
\boxed{I(S;R)=1-h_2(P_x)quad\text{bits per presentation}.}
$$

It is maximal, equal to one bit, at $P_x=0$ and also at $P_x=1$. The latter response is always opposite to the ideal label but still specifies the stimulus perfectly after relabelling. It is minimal, equal to zero, at $P_x=1/2$, when both response distributions are identical and the response is independent of the stimulus. If error is conventionally restricted to $0\leq P_x\leq1/2$, the maximum occurs only at zero.

The symmetric-error assumption matters. A single overall error probability would not determine this information if the two stimuli had different conditional error rates or if the response included additional outcomes.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
