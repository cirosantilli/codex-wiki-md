<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

Let $D=Q/V_0$ be the [dilution rate](../../../../../dilution-rate.md). Population loss is $DN$, and nutrient loss by consumption is $NK(C)/V_0$, so [mass conservation](../../../../../mass-conservation.md) gives

$$
\dot N=\gamma NK(C)-DN,\qquad \dot C=D(C_0-C)-\frac{NK(C)}{V_0}.
$$

Use the dimensionless variables $\tau=Dt$, $c=C/K_0$, and $n=NK_{\max}/(QK_0)$. Substitution into the [Monod equation](../../../../../monod-equation.md) gives the stated system with

$$
\boxed{\alpha=\frac{\gamma K_{\max}V_0}{Q},\qquad\beta=\frac{C_0}{K_0}.}
$$

For a positive [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md), the first equation requires $\alpha c/(1+c)=1$. Hence $c_*=1/(\alpha-1)$ and $n_*=\alpha(\beta-c_*)$, both positive exactly under the specified inequalities.

Writing $A=\alpha n_* /(1+c_*)^2>0$, the [Jacobian matrix](../../../../../jacobian-matrix.md) at this [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) is

$$
J=\begin{pmatrix}0&A\\-1/\alpha&-1-A/\alpha\end{pmatrix},\qquad
\boxed{\operatorname{spec}J=\{-1,-A/\alpha\}.}
$$

Both [eigenvalues](../../../../../eigenvalue.md) are negative, so the state is [locally asymptotically stable](../../../../../asymptotic-stability.md). The [Monod chemostat equilibrium and relaxation](../../../../../monod-chemostat-equilibrium-and-relaxation.md) also makes one decay rate transparent: $z=c+n/\alpha$ satisfies $z'=\beta-z$, independently of the uptake kinetics.

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
