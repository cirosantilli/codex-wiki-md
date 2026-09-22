<h1 id="32d/solution">Solution</h1>

↑ **Parent:** [32D](../32d.md)

In the original eigenbasis, $Q'=\begin{pmatrix}-1&i\epsilon\\-i\epsilon&1\end{pmatrix}$. Insert the proposed first-order state for [eigenvalue](../../../../../eigenvalue.md) near minus one. The first component gives $c_1=0$; the second gives $-ia_1+a_2=-a_2$, hence $a_2=ia_1/2$. Similarly for the [eigenvalue](../../../../../eigenvalue.md) near one, $c_2=0$ and $b_2=ib_1/2$. Normalization gives $|a_1|=|b_1|=1$, with their phases freely selectable. Choosing the original-state phase conventions,

$$
\boxed{a_1=b_1=1,\qquad a_2=b_2=i/2,\qquad c_1=c_2=0.}
$$

The states are orthogonal through first order because the two cross terms cancel.

Exactly, $(Q')^2=(1+\epsilon^2)I$, so putting $R=\sqrt{1+\epsilon^2}$ gives

$$
\boxed{q'_1=-R,\qquad q'_2=R.}
$$

For an [eigenvalue](../../../../../eigenvalue.md) $q'$, the first row requires the component ratio $v_2/v_1=-i(1+q')/\epsilon$, so the coefficient in the printed parametrization is **$\boxed{B=1}$**. With $D=\sqrt{(1+R)^2+\epsilon^2}$, smooth normalized choices are

$$
\boxed{|1'\rangle=\frac1D\binom{1+R}{i\epsilon},\qquad
|2'\rangle=\frac1D\binom{i\epsilon}{1+R}.}
$$

They have unit norm and zero inner product, and direct multiplication gives the two [eigenvalue](../../../../../eigenvalue.md) equations. For $\epsilon\ne0$, the printed scalar factors can be chosen $A_1=(1+R)/D$ and $A_2=i\epsilon/D$; the second is allowed a complex phase. The displayed ratio form is singular at zero, but the normalized vectors have the correct continuous limits there.

Expanding $R=1+\epsilon^2/2+O(\epsilon^4)$ and $D=2+O(\epsilon^2)$ gives $|1'\rangle=|1\rangle+i\epsilon|2\rangle/2+O(\epsilon^2)$ and $|2'\rangle=|2\rangle+i\epsilon|1\rangle/2+O(\epsilon^2)$, while the [eigenvalues](../../../../../eigenvalue.md) have no first-order shift. This recovers all six perturbative coefficients with the same phase convention.

## ↑ Ancestors (10)

1. [32D](../32d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
