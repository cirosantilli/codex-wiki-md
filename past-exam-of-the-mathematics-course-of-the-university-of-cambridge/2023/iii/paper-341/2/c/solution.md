<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Second Dahlquist barrier](../../../../../../second-dahlquist-barrier.md) states that an [A-stable](../../../../../../a-stability.md) linear [multistep method](../../../../../../linear-multistep-method.md) has order at most two. Part a shows that every method in this family has order at least three, so no member can be A-stable.

The exceptional reducible case does not evade the conclusion. At $a=1$,

$$
\rho(\zeta)-z\sigma(\zeta)
=(\zeta-1)\left[(\zeta-1)-\frac z2(\zeta+1)\right].
$$

Thus $\zeta=1$ is an amplification root for every $z=h\lambda$ with $\operatorname{Re}z<0$, whereas the multistep A-stability criterion requires all such roots to lie strictly inside the unit disk. Hence

$$
\boxed{\text{there is no real value of }a\text{ for which the method is A-stable}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
