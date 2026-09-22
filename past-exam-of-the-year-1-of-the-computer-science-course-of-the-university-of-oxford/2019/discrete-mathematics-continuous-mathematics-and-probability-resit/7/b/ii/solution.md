<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $G(s)=\mathbb E[s^F]$. The initial possibilities are $H$ with probability $1/2$, after which a fresh wait begins; $TH$ with probability $1/4$, after which a fresh wait begins; or $TT$ with probability $1/4$, which ends the experiment. Accounting for the flips already made in each case gives the [probability generating function](../../../../../../probability-generating-function.md) equation

$$
G(s)=\frac s2G(s)+\frac{s^2}4G(s)+\frac{s^2}4=\frac{(2s+s^2)G(s)+s^2}{4}.
$$

Therefore **$\displaystyle G_F(s)=\frac{s^2}{4-2s-s^2}$** for $0\leq s\leq1$. In particular, $G_F(1)=1$ and there is no mass below two flips, as required.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Discrete mathematics, continuous mathematics, and probability resit](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
