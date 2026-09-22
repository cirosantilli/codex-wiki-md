<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Adjoin $\dot p=0$ and use an [extended centre manifold](../../../../../../extended-centre-manifold-for-a-parameter.md) with local coordinates $(x,p)$. Count $p$ as order $x^2$, as appropriate to a steady-state fold, and write

$$
y=a_1p+a_2x^2+O(x^3,xp,p^2),\qquad
z=b_1p+b_2x^2+O(x^3,xp,p^2).
$$

The [centre-manifold invariance equation](../../../../../../centre-manifold-invariance-equation.md) differentiates these graphs along $\dot x=y$. The derivatives $y_x y$ and $z_x y$ first contribute at weighted order three. Comparing the coefficients of $p$ and $x^2$ in the right sides therefore gives

$$
-qa_1-b_1=0,\quad 1-qa_2-b_2=0,\qquad
a_1+1-b_1=0,\quad a_2-b_2=0.
$$

Since $q+1\ne0$, their solution is

$$
a_1=-\frac1{q+1},\quad a_2=\frac1{q+1},\qquad
b_1=\frac q{q+1},\quad b_2=\frac1{q+1}.
$$

Hence the reduced [normal form](../../../../../../normal-form-dynamical-systems.md) is

$$
\boxed{\dot x=\frac{x^2-p}{q+1}+O(x^3,xp,p^2).}
$$

Both the quadratic and unfolding coefficients are nonzero, so **the steady-state bifurcation is a saddle-node**, with [equilibria](../../../../../../equilibrium-point-of-a-dynamical-system.md) on the $p>0$ side. The exact steady equations confirm this: $y=0$, $z=x^2$, and $p=z+z^3=x^2+x^6$, giving two nearby [equilibria](../../../../../../equilibrium-point-of-a-dynamical-system.md) for $p>0$ and none for $p<0$.

For $q>-1$ the transverse modes are attracting; the negative-$x$ branch is locally attracting and the positive-$x$ branch has one unstable direction. For $q<-1$, one transverse [eigenvalue](../../../../../../eigenvalue.md) is already positive, so neither full [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) is [asymptotically stable](../../../../../../asymptotic-stability.md), although the reduced fold is still present with reversed flow orientation. The parameter $q=-1$ requires a higher-dimensional degeneracy analysis and is outside the stated assumption.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
