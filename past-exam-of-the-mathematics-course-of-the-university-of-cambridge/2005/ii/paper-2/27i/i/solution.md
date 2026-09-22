<h1 id="27i/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $Q=P_1-P_0$ and $R=I-P_1$. For nested subspaces these are orthogonal [projections](../../../../../../projection-linear-algebra.md) onto $\Theta_1\cap\Theta_0^\perp$ and $\Theta_1^\perp$, of ranks $d_1-d_0$ and $d-d_1$. Under the null, both annihilate $\mu$. In an [orthonormal basis](../../../../../../orthonormal-basis.md) adapted to $\Theta_0$, these two spaces and their complement, the coordinates of $X-\mu$ are [independent](../../../../../../independent-random-variables.md) $N(0,\sigma^2)$. Consequently

$$
\boxed{\frac{\|X-P_1X\|^2}{\sigma^2}\sim\chi^2_{d-d_1},\qquad
\frac{\|P_1X-P_0X\|^2}{\sigma^2}\sim\chi^2_{d_1-d_0},}
$$

and the two variables are [independent](../../../../../../independent-random-variables.md). Equivalently the [joint probability density](../../../../../../joint-probability-density.md) of the two unscaled sums $a,b>0$ factors into gamma [densities](../../../../../../density.md) of respective shapes $(d-d_1)/2,(d_1-d_0)/2$ and common scale $2\sigma^2$.

The nuisance [variance](../../../../../../variance-split.md) cancels in

$$
\boxed{F=\frac{\|P_1X-P_0X\|^2/(d_1-d_0)}{\|X-P_1X\|^2/(d-d_1)}
\sim F_{d_1-d_0,d-d_1}\quad\text{under }H_0.}
$$

Reject for a value above the upper $\alpha$ critical quantile to obtain a level-$\alpha$ test. Under a genuine alternative the numerator is noncentral chi-square with noncentrality $\|Q\mu\|^2/\sigma^2$, while the denominator retains its central law, explaining the upper-tail choice.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [27I](../../27i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
