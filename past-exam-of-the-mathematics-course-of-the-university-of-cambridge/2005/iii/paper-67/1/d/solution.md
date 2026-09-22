<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The rotated [global relations](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) form a square system for the three missing [boundary traces](../../../../../../boundary-trace-of-a-function.md). Solve this system and substitute the resulting [finite-time spectral boundary transforms](../../../../../../finite-time-spectral-boundary-transform.md) into the [integral representation](../../../../../../integral-representation.md). The pieces containing $Q(k_j,T)$ have zero contour contribution by analyticity, rotation of the relevant sectors and the [Cauchy integral theorem](../../../../../../cauchy-s-integral-theorem.md). The remaining expression involves only $Q_0,F_0,G_0,G_1$. The [finite-interval Airy spectral determinant](../../../../../../finite-interval-airy-spectral-determinant.md) has no nonremovable zeros in the contour domains, as established below, so this elimination introduces no extra spectral data there. Differentiating the representation, and using temporal inversion and compatibility at the corners, verifies the [partial differential equation](../../../../../../partial-differential-equation-split.md), initial value and the three prescribed boundary values.

For a direct [Hadamard well-posedness](../../../../../../well-posed-problem.md) check, the homogeneous difference satisfies

$$
\frac d{dt}\frac12\int_0^L|q|^2dx=-\frac12|q_x(0,t)|^2\leq0.
$$

This proves uniqueness and continuous dependence for homogeneous boundary data. More generally subtract a smooth quadratic boundary lift $b(x,t)$ satisfying the three prescribed endpoint conditions. The remaining problem has homogeneous boundary conditions and forcing $-b_t-b_{xxx}$. Its [semigroup generator](../../../../../../infinitesimal-generator-of-a-semigroup.md) is $A=-d^3/dx^3$ on $H^3(0,L)$ with $v(0)=v(L)=v'(L)=0$. It is a [dissipative operator](../../../../../../dissipative-operator.md); for every real $\zeta>0$ the equation $(\zeta-A)v=h$ has a unique solution, since the homogeneous third-order boundary system is injective by the same energy identity and therefore invertible. Thus $A$ is [maximal dissipative](../../../../../../maximal-dissipative-operator.md) and generates a [contraction semigroup](../../../../../../contraction-semigroup.md). This gives existence and continuous dependence on the lifted data and forcing. **Smooth compatible data therefore define a well-posed problem.** This operator argument and the spectral elimination describe the same evolution.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
