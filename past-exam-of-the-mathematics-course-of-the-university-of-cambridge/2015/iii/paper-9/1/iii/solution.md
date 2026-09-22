<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $\alpha=1-n/q>0$ and

$$
A=\operatorname*{ess\,sup}_{\Omega}|u|,\qquad N=A+\|F\|_{L^q(\Omega)}+\|g\|_{L^{q/2}(\Omega)}.
$$

First suppose $A<\infty$. For an interior ball $B_R$, with $R\leq1$, write $M_R=\operatorname*{ess\,sup}_{B_R}u$, $m_R=\operatorname*{ess\,inf}_{B_R}u$, and $\omega(R)=M_R-m_R$. Constant shifts of a [divergence-form elliptic operator](../../../../../../divergence-form-elliptic-operator.md) change its forcing. The two nonnegative [weak supersolutions](../../../../../../weak-supersolution-of-a-divergence-form-elliptic-equation.md) $v=M_R-u$ and $w=u-m_R$ satisfy, respectively,

$$
Lv=\operatorname{div}(M_Rb-F)+(M_Rd-g),\qquad Lw=\operatorname{div}(F-m_Rb)+(g-m_Rd).
$$

Their [Weak Harnack inequalities](../../../../../../weak-harnack-inequality.md) on $B_{R/2}$ therefore have forcing errors bounded by $CNR^\alpha$. Indeed $|M_R|,|m_R|\leq A$, the new divergence forcing is bounded by $\|F\|_q+A\|b\|_q$, and the scalar forcing by $\|g\|_{q/2}+A\|d\|_{q/2}$; also $R^{2\alpha}\leq R^\alpha$.

On $B_{R/2}$ we have $v+w=\omega(R)$. Even if $p<1$, the elementary inequality $(s+t)^p\leq C_p(s^p+t^p)$ implies

$$
\omega(R)\leq C_p\left(\left(\frac{1}{|B_{R/2}|}\int_{B_{R/2}}v^p\right)^{1/p}+\left(\frac{1}{|B_{R/2}|}\int_{B_{R/2}}w^p\right)^{1/p}\right).
$$

The sum of the two [essential infima](../../../../../../essential-infimum.md) is $\omega(R)-\omega(R/2)$. Enlarging a uniform constant $C_0>1$ gives

$$
\omega(R)\leq C_0\bigl(\omega(R)-\omega(R/2)+CNR^\alpha\bigr),\qquad \omega(R/2)\leq\theta\omega(R)+CNR^\alpha,
$$

where $\theta=1-C_0^{-1}\in(0,1)$. This is an [oscillation decay estimate](../../../../../../oscillation-decay-estimate.md); [inhomogeneous oscillation decay implies Hölder continuity](../../../../../../inhomogeneous-oscillation-decay-implies-holder-continuity.md). Choose

$$
0<\mu<\min\{\alpha,-\log_2\theta,1\}.
$$

Iterating on concentric balls, starting at a fixed admissible radius $R_*\leq1$, yields

$$
\omega(2^{-k}R_*)\leq\theta^k\omega(R_*)+CN R_*^\alpha\sum_{j=0}^{k-1}\theta^j2^{-\alpha(k-1-j)}\leq C N2^{-k\mu}.
$$

The strict choice of $\mu$ bounds the [geometric series](../../../../../../geometric-series.md), including the case in which the two original decay rates coincide. Monotonicity of oscillation extends this bound to intermediate radii.

Take $R_*$ uniformly smaller than the distance of $\Omega'$ from the boundary of $\Omega$. The vanishing essential oscillation produces a continuous representative of $u$. A ball centred at either of two sufficiently close points of $\Omega'$ contains both, so its oscillation bounds their difference by $CN|x-y|^\mu$. For separated points use $|u(x)-u(y)|\leq2A$. Thus the [Hölder seminorm](../../../../../../holder-seminorm.md) satisfies

$$
\boxed{[u]_{\mu;\Omega'}\leq C\left(\operatorname*{ess\,sup}_{\Omega}|u|+\|F\|_{L^q(\Omega)}+\|g\|_{L^{q/2}(\Omega)}\right).}
$$

The constants depend only on the indicated domain separation, dimension, coefficient norms, [uniform ellipticity](../../../../../../uniformly-elliptic-operator.md) bounds and $q$. If the global [essential supremum](../../../../../../essential-supremum.md) is infinite, the displayed global estimate is vacuous; [local boundedness of weak elliptic subsolutions](../../../../../../local-boundedness-of-weak-elliptic-subsolutions.md) on slightly larger compact subsets still makes the same argument prove interior [Hölder continuity](../../../../../../holder-condition.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
