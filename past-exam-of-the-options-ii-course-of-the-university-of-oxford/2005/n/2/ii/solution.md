<h1 id="n/2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume $N\ge2$, as required by the source's selection probabilities, and put $q=(1-p)/(N-1)$. Conditional on the red book's current position, the next independent selection determines its move without needing its earlier history. Selecting the red book moves it left, unless already leftmost. Selecting the plain book immediately to its right moves it right. Every other selection leaves its position unchanged. Thus this position process is a [Markov chain](../../../../../markov-chain-split.md) on $\{1,\ldots,N\}$, with

$$
P_{i,i-1}=p\ (i>1),\quad P_{i,i+1}=q\ (i<N),\quad
P_{i,i}=1-p-q\ (1<i<N),
$$

and boundary self-loop probabilities $P_{11}=1-q$, $P_{NN}=1-p$. These account for every selection and each row sums to one.

Stationarity at the first state gives $\pi_1=(1-q)\pi_1+p\pi_2$, hence $p\pi_2=q\pi_1$. When $N\ge3$, for the second state substitution of this identity into its stationarity equation gives $p\pi_3=q\pi_2$. More generally, summing stationarity over the [initial segment](../../../../../initial-segment.md) $\{1,\ldots,i\}$ equates its sole outward and inward [probability](../../../../../probability.md) flows:

$$
q\pi_i=p\pi_{i+1}\qquad(1\le i<N).
$$

Write $r=q/p$. Then $\pi_i=\pi_1r^{i-1}$. Normalization gives

$$
\boxed{\pi_i=\frac{(1-r)r^{i-1}}{1-r^N}\quad(r\ne1),\qquad
\pi_i=\frac1N\quad(r=1),\qquad r=\frac{1-p}{p(N-1)}.}
$$

The expression is positive also for $r>1$, since both numerator prefactor and denominator are negative. The uniform case is exactly $p=1/N$, when all books are equally likely to be selected. Since both neighboring transition probabilities are positive, the finite chain is irreducible; the displayed [stationary distribution](../../../../../stationary-distribution.md) is therefore unique.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [N](../../../n.md)
4. [2005](../../../../2005-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
