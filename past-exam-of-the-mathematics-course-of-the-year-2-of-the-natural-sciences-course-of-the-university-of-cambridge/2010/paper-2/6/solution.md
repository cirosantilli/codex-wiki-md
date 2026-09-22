<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

In Cartesian coordinates a rank-$r$ [tensor](../../../../tensor.md) is an array whose components transform under a change of orthonormal axes by one [rotation matrix](../../../../rotation-matrix.md) factor per index:

$$
T'_{i_1\cdots i_r}=Q_{i_1j_1}\cdots Q_{i_rj_r}T_{j_1\cdots j_r}.
$$

An [isotropic tensor](../../../../isotropic-tensor.md) has unchanged components under every proper [rotation](../../../../rotation-mathematics.md). The [Levi-Civita symbol](../../../../levi-civita-symbol.md) obeys

$$
Q_{ia}Q_{jb}Q_{kc}\epsilon_{abc}=(\det Q)\epsilon_{ijk}=\epsilon_{ijk}
$$

for $Q\in SO(3)$, proving [rotation invariance of the Levi-Civita symbol](../../../../rotation-invariance-of-the-levi-civita-symbol.md). Under an orthogonal transformation of determinant $-1$ its sign reverses; including such transformations requires the [pseudotensor](../../../../pseudotensor.md) distinction. Here isotropy is with respect to proper rotations.

Contract the determinant identity with $\epsilon_{ijk}$. Since $\epsilon_{ijk}\epsilon_{ijk}=3!=6$, one obtains

$$
\boxed{\det A=\frac16\epsilon_{ijk}\epsilon_{lmn}A_{il}A_{jm}A_{kn}.}
$$

Every index on the right is contracted, so the [tensor component transformation law](../../../../tensor-component-transformation-law.md) leaves no free rotation factor: the [determinant](../../../../determinant.md) is a [scalar](../../../../scalar.md). Equivalently, $A'=QAQ^T$ gives $\det A'=(\det Q)^2\det A=\det A$.

For the [matrix inverse](../../../../matrix-inverse-split.md), define

$$
C_{ab}=\frac12\epsilon_{ajk}\epsilon_{bmn}A_{jm}A_{kn}.
$$

This is the [cofactor matrix](../../../../cofactor-matrix.md). To verify the inverse formula rather than just recognize it, contract with $A_{ib}$ and use the determinant identity again:

$$
A_{ib}C_{ab}=\frac12\epsilon_{ajk}(\det A)\epsilon_{ijk}=(\det A)\delta_{ia}.
$$

Here the [contraction of two Levi-Civita symbols](../../../../contraction-of-two-levi-civita-symbols.md) gives $\epsilon_{ajk}\epsilon_{ijk}=2\delta_{ai}$. Therefore $AC^T=(\det A)I$ and, when $\det A\ne0$,

$$
\boxed{(A^{-1})_{ba}=\frac{C_{ab}}{\det A}=\frac1{2\det A}\epsilon_{ajk}\epsilon_{bmn}A_{jm}A_{kn}.}
$$

These are the [Levi-Civita formulas for a three-dimensional determinant and inverse](../../../../levi-civita-formulas-for-a-three-dimensional-determinant-and-inverse.md).

Now differentiate the cubic determinant formula with respect to the individual entry $A_{ab}$. The three differentiated factors give equal contributions: exchanging two paired indices changes the sign of both epsilon symbols, leaving their product unchanged. Thus

$$
\frac{\partial\det A}{\partial A_{ab}}=\frac36\epsilon_{ajk}\epsilon_{bmn}A_{jm}A_{kn}=C_{ab}.
$$

Substituting the inverse expression proves the entrywise [derivative of the determinant](../../../../derivative-of-the-determinant.md):

$$
\boxed{\frac{\partial\det A}{\partial A_{ab}}=(\det A)(A^{-1})_{ba}=(\det A)(A^{-1})^T_{ab}.}
$$

The cofactor version remains valid for singular matrices; only the inverse version requires invertibility.

For the time-dependent [Jacobian matrix](../../../../jacobian-matrix.md), the stated smooth expansion implies

$$
A_{ij}(t,x)=\delta_{ij}+t\partial_i u_j(x)+O(t^2),\qquad A(0,x)=I.
$$

Applying the [chain rule](../../../../chain-rule.md) and the entrywise determinant derivative gives [Jacobi's formula](../../../../jacobi-s-formula.md) near $t=0$:

$$
\frac d{dt}\det A=\sum_{ab}C_{ab}\dot A_{ab}=(\det A)\operatorname{tr}(A^{-1}\dot A).
$$

At zero, $C=I$, so $\left.\partial_t\det A\right|_0=\sum_a\partial_a u_a=\nabla\cdot u$. A [Taylor expansion](../../../../taylor-expansion.md) therefore yields

$$
\boxed{\det A(t,x)=1+t\nabla\cdot u(x)+O(t^2)=1+O(t^2)\quad\text{if }\nabla\cdot u=0.}
$$

The [Jacobian determinant](../../../../jacobian-determinant.md) measures local volume change, so this establishes volume preservation to first order. An arbitrary family specified only through its first-order expansion need not preserve volume exactly at higher orders.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [Paper 2](../../paper-2-split.md)
3. [2010](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
