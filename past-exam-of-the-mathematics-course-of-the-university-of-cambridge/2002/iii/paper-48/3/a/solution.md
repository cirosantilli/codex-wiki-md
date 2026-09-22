<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Putting $\varepsilon=0$ gives the local [regular perturbation](../../../../../../regular-perturbation.md) result $y_0=(x^2+1)/2$. It cannot describe the whole half-line: its [derivative](../../../../../../derivative.md) grows like $x$, making $\varepsilon y'$ order one at $x=O(\varepsilon^{-1})$.

The useful exact [change of variables](../../../../../../change-of-variables-formula.md) is

$$
r=\log x,\qquad z(r)=\frac{\varepsilon y(x)}x,\qquad
w(r)=\varepsilon y'(x).
$$

Direct substitution turns the equation into two [autonomous differential equations](../../../../../../autonomous-system-mathematics.md),

$$
\boxed{z_r=w-z,\qquad w_r=(1-\varepsilon-w)w+2\varepsilon z}.
$$

The initial values here are $z(0)=w(0)=\varepsilon$. Near the origin, linearizing this system gives [eigenvalues](../../../../../../eigenvalue.md) $1$ and $-1-\varepsilon$. Equivalently, neglecting only the [derivative](../../../../../../derivative.md)-square nonlinearity in the original equation gives the two modes $x^2$ and $x^{-\varepsilon}$. Their matching coefficients are

$$
A=\frac{1+\varepsilon}{2+\varepsilon},\qquad
B=\frac1{2+\varepsilon},\qquad
C=2\varepsilon A=\frac{2\varepsilon(1+\varepsilon)}{2+\varepsilon}.
$$

Thus the growing [derivative](../../../../../../derivative.md) has $w\sim Cx$. Keeping these unexpanded linear-mode coefficients is convenient for matching; it does not assert that the linearized solution is the exact nonlinear one.

At the [distinguished limit](../../../../../../distinguished-limit.md) $X=Cx=O(1)$, set $R=\log X$. To leading order the [derivative](../../../../../../derivative.md) equation becomes $w_R=w(1-w)$, the [logistic differential equation](../../../../../../logistic-differential-equation.md). Matching $w\sim e^R$ as $R\to-\infty$ selects

$$
w=\frac{X}{1+X}.
$$

Then $z_R+z=w$, and the growing-mode matching $z\sim X/2$ gives

$$
z=\frac1X\int_0^X\frac{s}{1+s}\,ds
=\frac{H(X)}X,\qquad H(X)=X-\log(1+X).
$$

This proves the [logistic crossover in a weakly nonlinear Euler equation](../../../../../../logistic-crossover-in-a-weakly-nonlinear-euler-equation.md). In particular the nonlinear-region leading solution is $y\sim H(Cx)/(\varepsilon C)$, or $\varepsilon^{-2}H(\varepsilon x)$ with the constants taken at their lowest order.

A [composite asymptotic expansion](../../../../../../additive-composite-expansion.md) retaining the small-distance stable mode and satisfying the initial value exactly is

$$
\boxed{y_{\rm comp}(x)=A+B x^{-\varepsilon}
+\frac{H(Cx)-H(C)}{\varepsilon C},\qquad
A=\frac{1+\varepsilon}{2+\varepsilon},\ B=\frac1{2+\varepsilon},\ C=2\varepsilon A}.
$$

Since $H(X)=X^2/2+O(X^3)$, this matches $Ax^2+Bx^{-\varepsilon}$ when $Cx\ll1$ and hence $(x^2+1)/2$ at fixed $x$ as $\varepsilon\to0$. Its [derivative](../../../../../../derivative.md) at one differs from the prescribed value only by $O(\varepsilon)$, within leading-order accuracy. For $Cx\gg1$ it gives $y\sim x/\varepsilon$. Thus the composite covers the initial region, the nonlinear transition and the arbitrarily large-$x$ regime; uniform leading accuracy is understood relative to the growing solution, not as an absolute error independent of unbounded $x$.

There is no later hidden growth regime. The exact positive system keeps $z,w$ in $[0,1+\varepsilon]^2$, because its vector field points inward at every boundary. Its positive [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md) is $z=w=1+\varepsilon$, with [Jacobian matrix](../../../../../../jacobian-matrix.md) having trace $-2-3\varepsilon$ and determinant $1+\varepsilon$. The origin has no attracting direction inside the positive quadrant, while the divergence $-\varepsilon-2w<0$ excludes cycles by the [Bendixson-Dulac theorem](../../../../../../bendixson-dulac-theorem.md). The [Poincaré-Bendixson theorem](../../../../../../poincare-bendixson-theorem.md) therefore gives convergence to the positive [stable equilibrium](../../../../../../stable-equilibrium.md). At fixed small positive $\varepsilon$, the exact far-field slope is $y/x\to(1+\varepsilon)/\varepsilon$, whose difference from $1/\varepsilon$ is only relative $O(\varepsilon)$, consistent with the global leading composite.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
