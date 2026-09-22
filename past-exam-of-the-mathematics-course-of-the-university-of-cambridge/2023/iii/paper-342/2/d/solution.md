<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Under independent physical phase flips, an inner block suffers an effective phase flip of its encoded qubit exactly when it contains an odd number of errors. The binomial parity identity gives

$$
\Pr(\text{even})+\Pr(\text{odd})=1,
\qquad
\Pr(\text{even})-\Pr(\text{odd})=(1-2p)^m,
$$

and hence the effective outer error probability is

$$
\boxed{q_m=\Pr(\text{odd})=\frac{1-(1-2p)^m}{2}.}
$$

For every $p<1/2$ and finite $m$, one has $q_m<1/2$, so outer majority-vote decoding succeeds with probability tending to one as $n\to\infty$. At $p=1/2$, one has $q_m=1/2$. The physical threshold is therefore still

$$
\boxed{p_c=\frac12.}
$$

For fixed $p\in(0,1/2)$, however, $q_m$ increases monotonically to $1/2$ as $m$ grows. Its distance from threshold is

$$
\frac12-q_m=\frac{(1-2p)^m}{2}.
$$

Consequently the majority-vote standardized separation is only of order $(1-2p)^m\sqrt n$, and the [large-deviation](../../../../../../large-deviation-principle.md) exponent is of order $n(1-2p)^{2m}$. Thus larger $m$ leaves the threshold unchanged but makes the logical phase-error probability decay more slowly with $n$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
