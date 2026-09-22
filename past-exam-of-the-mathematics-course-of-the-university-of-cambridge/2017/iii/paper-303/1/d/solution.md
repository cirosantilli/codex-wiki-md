<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $\mathcal A_2\ne0$, rescale the [order parameter](../../../../../../order-parameter.md) by $m=(|\mathcal A_2|/\mathcal A_6)^{1/4}\psi$. Write $\sigma=\operatorname{sgn}\mathcal A_2$ and introduce dimensionless scaling variables

$$
X=\frac{\mathcal A_4}{|\mathcal A_2|^{1/2}\mathcal A_6^{1/2}},\qquad Y=\frac{h\mathcal A_6^{1/4}}{|\mathcal A_2|^{5/4}}.
$$

Every term then has the common energy-density factor $|\mathcal A_2|^{3/2}/\mathcal A_6^{1/2}$:

$$
\mathcal A=\frac{|\mathcal A_2|^{3/2}}{\mathcal A_6^{1/2}}\left(\frac\sigma2\psi^2+\frac X4\psi^4+\frac16\psi^6-Y\psi\right).
$$

Minimizing over $\psi$ defines the [tricritical crossover scaling](../../../../../../tricritical-crossover-scaling.md) functions

$$
\Phi_\sigma(X,Y)=\min_{\psi\in\mathbb R}\left(\frac\sigma2\psi^2+\frac X4\psi^4+\frac16\psi^6-Y\psi\right).
$$

For the minimized potential, following the paper's notation $\mathcal F$, this proves

$$
\boxed{(u,v,w,x,y,z)=\left(\frac32,\frac12,\frac12,\frac12,\frac14,\frac54\right).}
$$

The exponent names $x,y$ here are unrelated to the couplings in question 2. The expression concerns the specified order-parameter [polynomial](../../../../../../polynomial-split.md); a general material can also have a smooth, field-independent background [free-energy density](../../../../../../free-energy-density.md). Such a background should be separated before writing a homogeneous singular scaling form. A potential at prescribed [magnetization](../../../../../../magnetization.md), instead of prescribed field, is a different [Legendre transform](../../../../../../convex-conjugate.md) and is not obtained by this minimization.

There is a needed qualification to the printed single $\Phi$ and nonzero-value condition. At $(X,Y)=(0,0)$, the ordered branch has minimizers $\psi=\pm1$ and $\Phi_-(0,0)=-1/3$, whereas the disordered branch has minimizer zero and $\Phi_+(0,0)=0$. Thus

$$
\boxed{\Phi_-(0,0)=-\frac13,\qquad \Phi_+(0,0)=0.}
$$

For example, $\mathcal A_2>0$, $\mathcal A_4=h=0$ gives an identically zero minimized [polynomial](../../../../../../polynomial-split.md), contradicting a nonzero $\Phi(0,0)$ on that side. The valid scaling statement uses separate sign branches, or restricts the asserted nonzero value to approach from the ordered side. At $\mathcal A_2=0$ the displayed coordinates are singular; the critical isotherm is obtained as a limit or directly from the equation of state.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 303](../../../paper-303-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
