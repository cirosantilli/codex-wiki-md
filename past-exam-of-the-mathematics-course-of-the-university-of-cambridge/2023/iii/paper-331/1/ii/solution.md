<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Away from $z=0,\pm1$, the base profile is linear or constant, so $U''=0$ and $\phi''-\alpha^2\phi=0$. Across a corner $z=z_0$, integration of the Rayleigh equation gives the jump condition

$$
(U(z_0)-c)[\phi']=[U']\phi.
$$

For the even mode, at $z=0$ this gives

$$
\phi'(0^+)=-\frac{\phi(0)}{1-c}.
$$

For $0<z<1$, therefore,

$$
\phi(z)=A\left[
\cosh(\alpha z)-
\frac{\sinh(\alpha z)}{\alpha(1-c)}
\right].
$$

For $z>1$, decay requires $\phi\propto e^{-\alpha(z-1)}$. The jump at $z=1$, where $[U']=1$, gives

$$
\phi'(1^-)=\left(\frac1c-\alpha\right)\phi(1).
$$

Substitution and elementary simplification yield

$$
\boxed{
2\alpha^2c^2+\alpha(1-2\alpha-e^{-2\alpha})c
-[1-\alpha-(1+\alpha)e^{-2\alpha}]=0}.
$$

The coefficients are real, so instability occurs when the quadratic discriminant is negative. At $\alpha=1$ it is

$$
(1+e^{-2})^2-16e^{-2}<0,
$$

whereas at $\alpha=2$, using $e^{-4}\simeq1/55$, it is positive. By continuity there is a first threshold $1<\alpha_s<2$ at which the discriminant vanishes. Hence one conjugate root has $c_i>0$ for

$$
\boxed{1\leq\alpha<\alpha_s<2}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 331](../../../paper-331-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
