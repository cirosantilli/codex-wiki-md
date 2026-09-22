<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The high-contact assumptions give $A>D$ away from a degeneracy. Since $C(p)=Bp+O(p^2)$, perturbing the larger [eigenvalue](../../../../../../eigenvalue.md) in the [assortatively mixed two-risk-group SIS model](../../../../../../assortatively-mixed-two-risk-group-sis-model.md) gives

$$
\boxed{R_0=\frac A\gamma+
\frac{B^2}{\gamma(A-D)}p+O(p^2).}
$$

For the biologically useful high-risk-core regime $A>\gamma>D$, put $x_0=1-\gamma/A$. Substituting $x=x_0+px_1+O(p^2)$ and $y=py_1+O(p^2)$ into the two [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) equations gives

$$
0=Bx_0+(D-\gamma)y_1,
\qquad
0=-(A-\gamma)x_1+\frac{\gamma B}{A}y_1.
$$

Thus the group susceptible fractions and their population-weighted total are

$$
\boxed{\begin{aligned}
s_H&=\frac\gamma A-\frac{B^2\gamma}{A^2(\gamma-D)}p+O(p^2),\\
s_L&=1-\frac{Bx_0}{\gamma-D}p+O(p^2),\\
s_{\rm total}&=1-px_0\left(1+\frac B{\gamma-D}\right)+O(p^2).
\end{aligned}}
$$

The [small-core SIS endemic expansion](../../../../../../small-core-sis-endemic-expansion.md) shows why the [homogeneous SIS susceptible fraction](../../../../../../homogeneous-sis-susceptible-fraction.md) relation fails for a mixed population: as the high-risk fraction tends to zero, $s_{\rm total}\to1$ while $R_0\to A/\gamma>1$. A small high-risk core sustains infection even though almost everyone in the population remains susceptible. Even $s_H$ need not equal $1/R_0$ at first order.

For completeness, if $A,D<\gamma$ with a fixed gap from threshold, small $p$ gives disease-free [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) and total susceptibility one. If $D>\gamma$, the low-risk group already sustains infection. Put $y_0=1-\gamma/D$ and let $x_0\in(0,1)$ be the positive root of $(1-x_0)(Ax_0+By_0)=\gamma x_0$. The first-order coefficients are

$$
y_1=\frac{B\gamma(x_0-y_0)}{D(D-\gamma)},\quad
x_1=\frac{B(1-x_0)y_1}{\gamma-A(1-2x_0)+By_0},\quad
s_{\rm total}=1-y_0+p(y_0-x_0-y_1)+O(p^2).
$$

Again it tends to $\gamma/D$ rather than $\gamma/A=1/R_0(0)$. These regular expansions require fixed nonzero gaps. At $A=D$ the spectral splitting is generally order $\sqrt p$; at $D=\gamma<A$, low-risk infection is also order $\sqrt p$, so a regular first-order Taylor expansion is inappropriate. An exact endemic replacement for the scalar identity is that the [susceptible-weighted next-generation matrix](../../../../../../susceptible-weighted-next-generation-matrix.md) has [spectral radius](../../../../../../spectral-radius.md) one.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
