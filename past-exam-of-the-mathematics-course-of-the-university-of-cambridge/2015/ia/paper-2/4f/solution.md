<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

Put $a=P(A)$, $b=P(B)$ and $j=P(A\cap B)$. Because $a,b>0$, the [conditional probability](../../../../../conditional-probability.md) inequality $P(A\mid B)>P(A)$ is equivalent to $j>ab$. But that same inequality gives $j/a>b$, or **$\boxed{P(B\mid A)>P(B)}$**. Thus [positive association of two events](../../../../../positive-association-of-two-events.md) is symmetric.

For the [complement of an event](../../../../../complement-of-an-event.md), $P(B^c)=1-b>0$, and

$$
P(A\mid B^c)=\frac{a-j}{1-b}<\frac{a-ab}{1-b}=a.
$$

Therefore **$B^c$ strictly repels $A$**; equivalently $P(B^c\mid A)=1-j/a<1-b=P(B^c)$. Both directions are stated because the wording switches the grammatical roles of attraction and repulsion. The substantive conclusion is the same: the conditional probabilities involving the complement are strictly smaller than their unconditional counterparts.

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
