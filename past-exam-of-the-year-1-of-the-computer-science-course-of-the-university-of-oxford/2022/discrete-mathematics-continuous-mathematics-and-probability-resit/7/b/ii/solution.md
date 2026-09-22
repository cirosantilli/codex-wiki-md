<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Equality can occur only at the two pairs $(0,0)$ and $(1,1)$. Their combined [probability](../../../../../../probability.md) is

$$
e^{-p}-p(1-e^{-p})+pe^{-p}=(1+2p)e^{-p}-p.
$$

Taking the complementary [probability](../../../../../../probability.md) gives

$$
\boxed{\mathbb P(X\ne Y)=1+p-(1+2p)e^{-p}.}
$$

Since $1+2p>0$, the supplied exponential bound implies

$$
\mathbb P(X\ne Y)\leqslant1+p-(1+2p)(1-p)=\boxed{2p^2}.
$$

This is a bound on the mismatch [probability](../../../../../../probability.md) for this particular [coupling](../../../../../../coupling.md) of the two [marginal distributions](../../../../../../marginal-distribution.md); the variables are not presumed independent.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Discrete mathematics, continuous mathematics and probability resit](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
