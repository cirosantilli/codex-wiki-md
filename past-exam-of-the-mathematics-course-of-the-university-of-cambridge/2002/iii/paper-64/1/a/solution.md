<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [order parameter](../../../../../../order-parameter.md) distinguishes thermodynamic phases. For a ferromagnet it is the [magnetization](../../../../../../magnetization.md); for a fluid near its [liquid-gas critical point](../../../../../../liquid-gas-critical-point.md) it can be the density relative to its critical value. In a system with a scalar [order parameter](../../../../../../order-parameter.md), introduce a slowly varying real [scalar field](../../../../../../scalar-field.md) $\phi(x)$ whose spatial average represents that [order parameter](../../../../../../order-parameter.md). The [Landau-Ginzburg theory](../../../../../../landau-ginzburg-theory.md) organizes the effective [free energy](../../../../../../thermodynamic-free-energy.md) as a local expansion consistent with the symmetry:

$$
\mathcal F[\phi]=\int d^dx\left\{\frac K2(\nabla\phi)^2+\frac r2\phi^2+\frac u4\phi^4+\frac v6\phi^6-H\phi\right\}.
$$

Here $K>0$ is the stiffness in the [gradient energy](../../../../../../gradient-energy.md), and $H$ is the [field conjugate to an order parameter](../../../../../../field-conjugate-to-an-order-parameter.md). The even powers assume a symmetry $\phi\mapsto-\phi$ at $H=0$. Without that symmetry further terms, including a cubic term, may be allowed. The coefficients are smooth functions of temperature and other controls; near a mean-field transition one usually writes $r=a(T-T_0)$ with $a>0$. A positive highest retained even coefficient makes the local potential bounded below.

The [partition function](../../../../../../canonical-partition-function.md) is obtained by weighting configurations with $\exp[-\mathcal F/(k_BT)]$. The [Landau approximation](../../../../../../landau-approximation.md) replaces this functional average by minimization, taking a uniform $\phi=M$ in a homogeneous phase. In a symmetric finite system the zero-field average can vanish even below the transition because it averages both signs of $M$. The spontaneous [order parameter](../../../../../../order-parameter.md) selects a [pure thermodynamic phase](../../../../../../pure-thermodynamic-phase.md) by taking the [thermodynamic limit](../../../../../../thermodynamic-limit.md) before removing the conjugate field:

$$
M=\lim_{H\downarrow0}\lim_{V\to\infty}
\left\langle V^{-1}\int_V\phi(x)\,d^dx\right\rangle_H.
$$

Thus **the order parameter measures the ordering of a selected thermodynamic phase**, rather than the average over all symmetry-related phases.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
