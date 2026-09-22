<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Write $H=H(\alpha)$. Since $\alpha$ has degree at least two and lies in $(0,1)$, $H>1$. Put

$$
x=\frac{\log(nh)}{d\log H}>1,
\qquad
k=\lfloor x\rfloor+1.
$$

Then $H^{kd}>nh$ and

$$
k+1\leq x+2\leq3x.
$$

Let

$$
m=\left\lceil\frac n{k+1}\right\rceil.
$$

Part (d), applied with $m$ in place of its polynomial-degree parameter, supplies $\ell\in\{k,k+1\}$ such that no nonzero integer polynomial of degree at most $m-1$ and with coefficients of absolute value less than $h$ vanishes at $\beta=\alpha^\ell$.

It follows that the $h^m$ sums

$$
\sum_{j=0}^{m-1}a_j\beta^j,
\qquad 0\leq a_j<h,
$$

are distinct. Since

$$
(m-1)\ell\leq(m-1)(k+1)\leq n-1,
$$

they form a subset of $A_n$. Hence

$$
|A_n|\geq h^m
\geq h^{\,n/(k+1)}
\geq h^{\,dn\log H/(3\log(nh))}
=H^{\,dn\log h/(3\log(nh))},
$$

as required.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 166](../../../paper-166-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
