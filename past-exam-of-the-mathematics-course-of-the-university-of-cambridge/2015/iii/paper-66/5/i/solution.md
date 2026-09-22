<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $t<1$, normalize the remaining probabilities by $q_j=P_X(j)/(1-t)$, $j=2,\ldots,k$. Directly splitting the [Shannon entropy](../../../../../../information-entropy.md) sum gives

$$
H(X)=-t\log_2t-(1-t)\log_2(1-t)+(1-t)H(q)=h(t)+(1-t)H(q).
$$

Here $h$ is the [binary entropy](../../../../../../binary-entropy.md). The [Shannon entropy](../../../../../../information-entropy.md) of a distribution on $k-1$ points is at most $\log_2(k-1)$. For example, nonnegativity of its [Kullback-Leibler divergence](../../../../../../kullback-leibler-divergence.md) from the uniform distribution gives $\log_2(k-1)-H(q)\geq0$. Thus the [entropy bound with one prescribed probability](../../../../../../entropy-bound-with-one-prescribed-probability.md) is

$$
\boxed{H(X)\leq h(t)+(1-t)\log_2(k-1).}
$$

For $t<1$, equality holds precisely when the remaining probabilities are all $(1-t)/(k-1)$. For $t=1$, the distribution is deterministic and both sides are zero. The displayed formula is for $k\geq2$; a one-point alphabet simply has zero [Shannon entropy](../../../../../../information-entropy.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
