<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [matrix exponential](../../../matrix-exponential.md) is the absolutely convergent series $e^{tA}=\sum_{n=0}^\infty t^nA^n/n!$, with derivative $Ae^{tA}$ and inverse $e^{-tA}$. If $K^T=-K$, then $(e^{tK})^Te^{tK}=e^{-tK}e^{tK}=I$. Its [determinant](../../../determinant.md) is [continuous](../../../continuous-function.md) in $t$, is never zero, and starts at one, so it is one throughout: $e^{tK}\in SO(3)$. Conversely, differentiating $(e^{tK})^Te^{tK}=I$ at zero gives $K^T+K=0$. Thus

$$
\boxed{e^{tK}\in SO(3)\text{ for all real }t\iff K^T=-K.}
$$

The quantifier matters: membership at one isolated time alone would not imply skewness.

Write $P(F)=DW(F)$ and $J=\det F>0$. For any skew matrix $K$, differentiate frame indifference along $e^{tK}F$:

$$
0=P(F):(KF)=(P(F)F^T):K.
$$

A matrix orthogonal to every skew matrix is symmetric. Therefore $P(F)F^T$ and the [Cauchy stress tensor](../../../cauchy-stress-tensor.md) $T=J^{-1}P(F)F^T$ are symmetric.

Let $\mathcal C=D^2W(I)$ and assume $P(I)=0$. Differentiating symmetry of $P(F)F^T$ at $I$ in direction $H$ shows $\mathcal C[H]$ is symmetric for every $H$. Hence $c_{ijkl}=c_{jikl}$. As a [Hessian](../../../hessian-matrix.md), $\mathcal C$ also has pair-interchange symmetry $c_{ijkl}=c_{klij}$. Combining the two gives $c_{ijkl}=c_{ijlk}$. Equivalently $\mathcal C$ annihilates [infinitesimal rotations](../../../skew-symmetric-matrix.md). This proves both requested minor symmetries and shows exactly where the stress-free assumption enters. It is [stress-free linearization of an objective energy](../../../stress-free-linearization-of-an-objective-energy.md).

For the particular energy, $\sum_iv_i^2=\operatorname{tr}(F^TF)$ and $\prod_iv_i=J$, so

$$
P(F)=4\alpha F+h'(J)\operatorname{cof}F.
$$

At $I$ this is $[4\alpha+h'(1)]I$. Therefore the reference is stress-free exactly when $\boxed{h'(1)=-4\alpha}$. To differentiate again, use $\operatorname{cof}F=JF^{-T}$. The [determinant](../../../determinant.md) and inverse derivatives at $I$ give

$$
\boxed{D(\operatorname{cof})(I)[H]=(\operatorname{tr}H)I-H^T,}
$$

which also proves the supplied hint. It follows that

$$
\mathcal C[H]=4\alpha H+h''(1)(\operatorname{tr}H)I-4\alpha[(\operatorname{tr}H)I-H^T].
$$

For a symmetric $e$ this becomes

$$
\boxed{\mathcal Ce=8\alpha e+[h''(1)-4\alpha](\operatorname{tr}e)I=2\mu e+\lambda(\operatorname{tr}e)I,\quad\mu=4\alpha,\ \lambda=h''(1)-4\alpha.}
$$

No additional positivity of the [bulk modulus](../../../bulk-modulus.md) follows from the stated smoothness of $h$ alone; this calculation identifies the moduli rather than imposing extra material assumptions.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2009](../../2009-split.md)
3. [Past exam of the solid mechanics course of the University of Oxford](../../split.md)
4. [Solid mechanics course of the University of Oxford](../../../solid-mechanics-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
