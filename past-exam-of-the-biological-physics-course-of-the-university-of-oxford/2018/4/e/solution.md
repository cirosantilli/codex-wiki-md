<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [quadratic-Hill mutual repression switch](../../../../quadratic-hill-mutual-repression-switch.md) is explicit: for $n=2$, [steady state](../../../../steady-state.md) requires $Y(1+Z^2)=\gamma$ and $Z(1+Y^2)=\gamma$. Subtraction gives

$$
(Y-Z)(1-YZ)=0.
$$

Thus either $Y=Z=x$, giving the unique positive cubic root $x^3+x-\gamma=0$, or $YZ=1$. In the latter case, $Y+1/Y=\gamma$, hence

$$
\boxed{Y_\pm=\frac{\gamma\pm\sqrt{\gamma^2-4}}2,\qquad
Z_\pm=\frac1{Y_\pm}=Y_\mp.}
$$

The non-symmetric pair is real, positive and distinct exactly when $\gamma>2$. For $0<\gamma<2$ only the symmetric solution exists. Eliminating one variable gives the source's hinted factorization,

$$
(Y^3+Y-\gamma)(Y^2-\gamma Y+1)=0,
$$

with no singular denominator for real [concentrations](../../../../concentration.md). The cubic is strictly increasing since $3Y^2+1>0$, so it contributes only the symmetric state.

One can verify the switch interpretation without a lengthy [stability](../../../../stability-of-a-numerical-method.md) analysis. At symmetry the [Jacobian matrix](../../../../jacobian-matrix.md) [eigenvalues](../../../../eigenvalue.md) are $-1\pm2x^2/(1+x^2)$: symmetry is stable for $x<1$ and becomes a saddle for $x>1$, corresponding to $\gamma<2$ and $\gamma>2$. At either asymmetric [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) the [eigenvalues](../../../../eigenvalue.md) are $-1\pm2/\gamma$, both negative when $\gamma>2$. Therefore

$$
\boxed{\gamma>2:\ \text{two attracting alternatives and a separating saddle};\qquad
0<\gamma<2:\ \text{one attracting symmetric state}.}
$$

At $\gamma=2$, all three branches meet at $(1,1)$ with a zero linear [eigenvalue](../../../../eigenvalue.md), the switching threshold rather than two distinct robust memory states. The lower panels of the original figure in [solution](../a/solution.md) show representative [nullclines](../../../../nullcline.md) on either side.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [4](../../4.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
