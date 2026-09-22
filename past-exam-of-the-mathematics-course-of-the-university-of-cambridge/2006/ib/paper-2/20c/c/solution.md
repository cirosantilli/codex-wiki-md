<h1 id="20c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

One excursion from zero escapes forever on the positive branch with probability $a_+=\tfrac12(1-\tfrac12)=1/4$, and on the negative branch with probability $a_-=\tfrac12(1-\tfrac13)=1/3$. The remaining probability is the return probability $r=5/12$. By the [last-excursion direction law at a transient junction](../../../../../../last-excursion-direction-law-at-a-transient-junction.md), the eventual positive escape probability is

$$
\boxed{\sum_{m=0}^\infty r^m a_+=\frac{1/4}{1-5/12}=\frac37.}
$$

Equivalently, if $p$ denotes the desired probability, the [Strong Markov property](../../../../../../strong-markov-property.md) gives $p=1/4+(5/12)p$. The negative escape probability is $4/7$, and their sum is one, as independently established in part (b).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [20C](../../20c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
