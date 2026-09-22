<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At $(\sigma,\mu)=(1,0)$ the origin's [matrix](../../../../../../matrix.md) is $\begin{pmatrix}0&0\\2&0\end{pmatrix}$: it has a double zero [eigenvalue](../../../../../../eigenvalue.md) and one [eigenvector](../../../../../../eigenvector.md). [Trace](../../../../../../matrix-trace.md) and [determinant](../../../../../../determinant.md) vary independently with $\mu$ and $\sigma$ there, so two parameters are needed. The symmetry of an [odd function](../../../../../../odd-function.md) removes quadratic terms, giving a [reflection-symmetric cubic double-zero normal form](../../../../../../reflection-symmetric-cubic-double-zero-normal-form.md). The quadratic nonlinearity required for a generic [Bogdanov–Takens bifurcation](../../../../../../bogdanov-takens-bifurcation.md) vanishes.

Use a prime for [differentiation](../../../../../../differentiation.md) with respect to the rescaled time. Direct substitution, with all rescaled variables written without tildes, gives

$$
\begin{aligned}
u'&=-sv+\tfrac12v^3+\varepsilon(\mu-v^2/2)u
+\tfrac12\varepsilon^2u^2v-\tfrac12\varepsilon^3u^3,\\
v'&=2u+\varepsilon(\mu-v^2/2)v
+\varepsilon^2(s-v^2/2)u-\tfrac12\varepsilon^3u^2v-\tfrac12\varepsilon^4u^3.
\end{aligned}
$$

At $\varepsilon=0$, the equations are $u'=-sv+v^3/2$, $v'=2u$. For

$$
\boxed{H=u^2+\frac s2v^2-\frac18v^4,}
$$

[differentiation](../../../../../../differentiation.md) gives $H'=2u(-sv+v^3/2)+(sv-v^3/2)2u=0$. This is the [Hamiltonian blow-up of a reflection-symmetric double-zero point](../../../../../../hamiltonian-blow-up-of-a-reflection-symmetric-double-zero-point.md).

For $s>0$, the [equilibrium points](../../../../../../equilibrium-point-of-a-dynamical-system.md) are a [centre equilibrium](../../../../../../center-equilibrium.md) at $(0,0)$ and saddles at $(0,\pm\sqrt{2s})$. The [centre equilibrium](../../../../../../center-equilibrium.md) has [eigenvalues](../../../../../../eigenvalue.md) $\pm i\sqrt{2s}$; at either [saddle equilibrium](../../../../../../saddle-equilibrium.md) they are $\pm2\sqrt s$. Levels $0<H<s^2/2$ contain closed inner ovals around the [centre equilibrium](../../../../../../center-equilibrium.md). The [saddle equilibrium](../../../../../../saddle-equilibrium.md) level has

$$
\boxed{H_{\rm het}=\frac{s^2}{2},\qquad
u=\pm\frac{2s-v^2}{2\sqrt2},\quad|v|\le\sqrt{2s}.}
$$

These two branches form a [heteroclinic cycle](../../../../../../heteroclinic-cycle.md) connecting the saddles. The branch with $u>0$ runs from the lower [saddle equilibrium](../../../../../../saddle-equilibrium.md) to the upper one because $v'=2u>0$; the other runs back. Outside the potential well, trajectories are open. The right panel of the preceding figure uses the coordinates $(v,u)$ to display the well and these directed connections.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 85](../../../paper-85-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
