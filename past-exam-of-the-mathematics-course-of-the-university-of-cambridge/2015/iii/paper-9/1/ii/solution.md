<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $M=\operatorname*{ess\,sup}_{\Omega}u$. The standard [local boundedness of weak elliptic subsolutions](../../../../../../local-boundedness-of-weak-elliptic-subsolutions.md) gives a finite upper bound on every [relatively compact](../../../../../../relatively-compact-subset.md) ball. In particular, the assumed equality of [essential suprema](../../../../../../essential-supremum.md) makes $M$ finite. Equivalently, when using the maximum principle for an upper-bounded [weak subsolution](../../../../../../weak-subsolution-of-a-divergence-form-elliptic-equation.md), this preliminary fact is already part of the hypothesis.

Set $v=M-u$. Because the [divergence-form elliptic operator](../../../../../../divergence-form-elliptic-operator.md) here annihilates constants, $v\geq0$ and $Lv=-Lu\leq0$. The hypothesis says $\operatorname*{ess\,inf}_Bv=0$. Cover the compact closure of $B$ by finitely many balls $D_j$ whose doubled balls lie in $\Omega$. At least one $D_j$ has [essential infimum](../../../../../../essential-infimum.md) zero: otherwise the minimum of their finitely many positive lower bounds would be a positive lower bound on $B$. The [Weak Harnack inequality](../../../../../../weak-harnack-inequality.md) with zero forcing now gives

$$
\left(\frac{1}{|D_j|}\int_{D_j}v^p\right)^{1/p}\leq C\operatorname*{ess\,inf}_{D_j}v=0.
$$

Consequently $v=0$ almost everywhere on $D_j$. If another admissible ball overlaps $D_j$ in an open set, its [essential infimum](../../../../../../essential-infimum.md) of $v$ is also zero, and the same argument makes $v$ vanish there. Since a domain is [connected](../../../../../../connected-space.md), a chain of overlapping interior balls reaches every point of $\Omega$. This [propagation of zeros by the weak Harnack inequality](../../../../../../propagation-of-zeros-by-the-weak-harnack-inequality.md) proves **$u=M$ almost everywhere on $\Omega$**, which is the claimed [strong maximum principle](../../../../../../strong-maximum-principle-for-elliptic-operators.md). Notice why the absence of the $b,d$ terms matters: it is precisely what makes $L(M-u)=-Lu$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
