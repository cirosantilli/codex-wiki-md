<h1 id="5/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use logarithms to base two, so [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) and [quantum relative entropy](../../../../../../quantum-relative-entropy.md) are measured in bits. For [density operators](../../../../../../density-matrix.md) $\rho,\sigma$,

$$
\boxed{S(\rho)=-\operatorname{Tr}(\rho\log_2\rho),\qquad
D(\rho\|\sigma)=\operatorname{Tr}[\rho(\log_2\rho-\log_2\sigma)].}
$$

The [quantum relative entropy](../../../../../../quantum-relative-entropy.md) formula applies when the [support of a positive operator](../../../../../../support-of-a-positive-operator.md) $\rho$ is contained in that of $\sigma$; otherwise $D(\rho\|\sigma)=+\infty$. Use $0\log_2 0=0$ in the [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) formula.

The binary [density operator](../../../../../../density-matrix.md) $\omega[p]$ is diagonal with [eigenvalues](../../../../../../eigenvalue.md) $1-p,p$. Its [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) is the [binary entropy](../../../../../../binary-entropy.md):

$$
\boxed{S(\omega[p])=h_2(p)=-(1-p)\log_2(1-p)-p\log_2p.}
$$

The two diagonal [density operators](../../../../../../density-matrix.md) commute, so their [quantum relative entropy](../../../../../../quantum-relative-entropy.md) is

$$
\boxed{D(\omega[p]\|\omega[q])=(1-p)\log_2\frac{1-p}{1-q}+p\log_2\frac pq.}
$$

A term with zero numerator has value zero; a positive numerator and zero denominator give $+\infty$. In particular, $D(\omega[0]\|\omega[0])=D(\omega[1]\|\omega[1])=0$, whereas $q=0,p>0$ or $q=1,p<1$ gives $+\infty$.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [5](../../5.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
