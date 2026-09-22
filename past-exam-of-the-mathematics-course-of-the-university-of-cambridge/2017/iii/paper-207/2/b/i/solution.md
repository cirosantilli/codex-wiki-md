<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Reading the arrows in the original diagram gives parents $\operatorname{pa}(A)=\operatorname{pa}(B)=\varnothing$, $\operatorname{pa}(C)=\{A,B\}$ and $\operatorname{pa}(D)=\{B\}$. The [Bayesian network](../../../../../../../bayesian-network.md) factorization is

$$
\boxed{P(a,b,c,d)=P(a)P(b)P(c\mid a,b)P(d\mid b).}
$$

For binary variables, each [conditional probability](../../../../../../../conditional-probability.md) table has one free [probability](../../../../../../../probability.md) per parent configuration, since its two entries sum to one. There are one each for $A$ and $B$, four for $C$, and two for $D$, giving

$$
\boxed{1+1+4+2=8\text{ free parameters}.}
$$

This is the dimension of the unrestricted binary [Bayesian network](../../../../../../../bayesian-network.md) family; extra [statistical parameter](../../../../../../../statistical-parameter.md) equalities or deterministic relationships would describe a smaller model and are not imposed by the diagram.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
