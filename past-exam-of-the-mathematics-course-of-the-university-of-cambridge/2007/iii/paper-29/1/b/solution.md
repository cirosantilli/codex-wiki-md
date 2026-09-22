<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the normalized [Eisenstein series](../../../../../../eisenstein-series.md) $E_4=1+240q+O(q^2)$ and $E_6=1-504q+O(q^2)$, and put

$$
\Delta=\frac{E_4^3-E_6^2}{1728}=q+O(q^2),\qquad j=\frac{E_4^3}{\Delta}.
$$

The [valence formula for the modular group](../../../../../../valence-formula-for-the-modular-group.md) applied to this nonzero weight-twelve [cusp form](../../../../../../cusp-form.md) gives weighted zero order one. Its order at infinity is already one, so $\Delta$ has no zeros in $\mathbb H$. Consequently the [Klein j-invariant](../../../../../../klein-j-invariant.md) is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) there and invariant under $SL_2(\mathbb Z)$.

Set $\rho=e^{2\pi i/3}$. The [stabilizer](../../../../../../stabilizer-subgroup.md) of $\rho$ forces $E_4(\rho)=0$, since the weight-four [automorphy factor](../../../../../../automorphy-factor.md) for $\begin{pmatrix}0&-1\\1&1\end{pmatrix}$ is $(\rho+1)^4\ne1$. The [stabilizer](../../../../../../stabilizer-subgroup.md) of $i$ forces $E_6(i)=0$, since $i^6=-1$. The [valence formula for the modular group](../../../../../../valence-formula-for-the-modular-group.md) gives

$$
v_\rho(E_4)=1,\qquad v_i(E_6)=1,
$$

with no other zero orbits for either form. In particular $j(\rho)=0$ and $j(i)=1728$.

For any $A\in\mathbb C$, the weight-twelve form

$$
h_A=E_4^3-A\Delta
$$

is nonzero, with constant [Fourier coefficient](../../../../../../fourier-coefficient.md) one and hence order zero at infinity. Its total weighted zero order is one. If $A=0$, the triple zero at $\rho$ accounts for this entire order. If $A=1728$, then $h_A=E_6^2$, and the double zero at $i$ accounts for it. For all other $A$, neither elliptic [orbit](../../../../../../orbit-dynamical-system.md) is a zero: $E_4(\rho)=0$ and $\Delta(\rho)\ne0$ exclude $\rho$, while $E_6(i)=0$ gives $E_4(i)^3=1728\Delta(i)$ and excludes $i$. Therefore there is precisely one ordinary zero [orbit](../../../../../../orbit-dynamical-system.md), of multiplicity one. Since $h_A(\tau)=0$ is exactly $j(\tau)=A$, every complex number occurs at exactly one modular [orbit](../../../../../../orbit-dynamical-system.md). Thus

$$
\boxed{SL_2(\mathbb Z)\backslash\mathbb H\xrightarrow{\;j\;}\mathbb C\text{ is a bijection}.}
$$

This proves [Klein j-invariant classifies complex lattice homothety](../../../../../../klein-j-invariant-classifies-complex-lattice-homothety.md) using the weighted zeros, including the two exceptional stabilizers.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
