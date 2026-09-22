<h1 id="36a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a point charge, the [charge density](../../../../../../charge-density.md) and [current density](../../../../../../current-density.md) are

$$
\rho(x',s)=q\delta^{(3)}(x'-y(s)),
\qquad
J(x',s)=qv(s)\delta^{(3)}(x'-y(s)).
$$

Insert these into the [retarded electromagnetic potential](../../../../../../retarded-potential.md). The argument of the [Dirac delta function](../../../../../../dirac-delta-function.md) depends on $x'$ through

$$
s=t-\frac{|x-x'|}{c}.
$$

At its unique zero $x'=y(t_{\rm ret})$, the [Jacobian determinant](../../../../../../jacobian-determinant.md) contributes the factor

$$
\left|1-\frac{n\cdot v}{c}\right|^{-1}.
$$

Since the source is subluminal, this quantity is positive. Writing $\mathbf R=x-y(t_{\rm ret})$, $R=|\mathbf R|$, and evaluating $\mathbf v$ at $t_{\rm ret}$ gives the [Liénard–Wiechert potentials](../../../../../../lienard-wiechert-potential.md)

$$
\boxed{
\phi(x,t)=\frac{q}{4\pi\epsilon_0}
\frac1{R-\mathbf v\cdot\mathbf R/c},
\qquad
\mathbf A(x,t)=\frac{\mu_0q}{4\pi}
\frac{\mathbf v}{R-\mathbf v\cdot\mathbf R/c}.}
$$

The identity $\mu_0\epsilon_0c^2=1$ equivalently gives $\mathbf A=\mathbf v\phi/c^2$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [36A](../../36a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
