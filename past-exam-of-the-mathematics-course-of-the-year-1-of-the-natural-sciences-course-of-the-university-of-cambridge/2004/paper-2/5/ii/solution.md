<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Each additional pair of independent shots resolves the tie with probability $r=2p(1-p)$, since exactly one team must score. It preserves the tie with probability $q=p^2+(1-p)^2=1-r$. Finishing after $10+2k+2$ shots means an initial tie, then $k$ tied pairs, then a decisive pair. Independence and [geometric continuation after an initial tie](../../../../../geometric-continuation-after-an-initial-tie.md) give

$$
\boxed{\Pr(N=12+2k)=\alpha\,[p^2+(1-p)^2]^k\,2p(1-p),\qquad k=0,1,\ldots.}
$$

Because $0<p<1$, $r>0$ and $q<1$. The total eventual winning probability is the sum of winning in the first ten shots and winning later:

$$
(1-\alpha)+\sum_{k=0}^\infty\alpha q^kr=1-\alpha+\frac{\alpha r}{1-q}=1.
$$

Equivalently, conditional on the initial tie, the probability of still being tied after $m$ further pairs is $q^m\to0$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
