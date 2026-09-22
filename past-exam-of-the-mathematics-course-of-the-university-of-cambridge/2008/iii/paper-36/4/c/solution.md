<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Since $\dot u(t)=a_t^2>0$, invert the image clock before exit and put $\widehat\xi_u=W_{t(u)}$. Its [quadratic variation](../../../../../../quadratic-variation.md) is $6u$ and its initial value is zero, because $\Phi(0)=0$. By the [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md), or the localized [Dambis-Dubins-Schwarz theorem](../../../../../../dambis-dubins-schwarz-theorem.md),

$$
\widehat\xi_u=\sqrt6\,\widehat B_u
$$

for a standard [Brownian motion](../../../../../../brownian-motion-split.md) up to the image exit time. If that lifetime is finite, the stopped [Brownian motion](../../../../../../brownian-motion-split.md) can be extended beyond it; only the stopped law is used here.

In this clock the image [mapping-out functions](../../../../../../mapping-out-function-of-a-compact-h-hull.md) obey the ordinary [Chordal Loewner equation](../../../../../../chordal-loewner-equation.md) with driver $\sqrt6\,\widehat B_u$. Their generated trace therefore has the law of [SLE](../../../../../../schramm-loewner-evolution.md) with parameter six, stopped when it leaves $N^*$. Meanwhile the original image segment is exactly $\Phi(\gamma)$ up to exit from $N$. The clock change is increasing, so it disappears after passing to $[\gamma]$. This proves **the local stopped-curve equality required in part (a)**.

For completeness, the original law is scale invariant: the maps $r^{-1}g_{r^2t}(rz)$ have driver $r^{-1}\xi_{r^2t}$, whose law is again $\sqrt6 B_t$ by [Brownian scaling](../../../../../../brownian-scaling.md). Hence $(r^{-1}\gamma_{r^2t})_{t\geq0}$ has the original trace law. Together with the stopped conformal-change argument, this establishes

$$
\boxed{[\gamma]\text{ for SLE}(6)\text{ has the locality property}.}
$$

The conclusion concerns local unparameterized segments up to exit; the capacity parameter itself changes according to $du=h_t'(\xi_t)^2dt$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
