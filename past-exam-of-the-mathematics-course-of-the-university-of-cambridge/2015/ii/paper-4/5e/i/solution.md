<h1 id="5e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $x=1+y$ and retain linear terms. The [delay differential equation](../../../../../../delay-differential-equation.md) is $\dot y(t)=-\alpha y(t-T)$, with [characteristic equation of a delay differential equation](../../../../../../characteristic-equation-of-a-delay-differential-equation.md) $\lambda+\alpha e^{-\lambda T}=0$. Write $z=\lambda T$ and $q=\alpha T$. If a root has $\operatorname{Re}z\geq0$, then $|z|=q e^{-\operatorname{Re}z}\leq q$. Writing $z=a+ib$ gives $a=-q e^{-a}\cos b$. For $q<\pi/2$, $|b|<\pi/2$ and the right side is negative, contradicting $a\geq0$. All characteristic roots therefore lie in the left half-plane.

An imaginary root $z=ib$ requires $\cos b=0$ and $b=q\sin b$. The first crossing is $q=\pi/2$, $z=\pm i\pi/2$. Implicit differentiation gives $dz/dq=-e^{-z}/(1+z)$, whose real part at the positive crossing is $(\pi/2)/(1+\pi^2/4)>0$. The later imaginary crossings occur at $q=\pi/2+2\pi k$ and also enter the right half-plane. Thus the equilibrium is **locally exponentially asymptotically stable when**

$$
\boxed{\alpha T<\pi/2,}
$$

and unstable when $\alpha T>\pi/2$. At equality the [linearized equation](../../../../../../linearized-equation.md) has neutral oscillatory modes; it is the [Hopf bifurcation](../../../../../../hopf-bifurcation.md) threshold. If stability is meant for the nonlinear equation itself, the borderline can also be resolved. In dimensionless time $s=t/T$, let $q_0=\pi/2$. A small center oscillation has the form $y=R\cos\theta+R^2(\cos2\theta/5+\sin2\theta/10)+O(R^3)$. Substitution at quadratic order gives these second-harmonic coefficients. At cubic order the fundamental forcing is $q_0R^3(\cos\theta/20+3\sin\theta/20)$. Projection onto the center mode divides the complex forcing by the characteristic derivative $1+iq_0$, yielding the [Hopf normal form](../../../../../../hopf-normal-form.md) amplitude equation

$$
\frac{dR}{ds}=-\frac{q_0(3q_0-1)}{20(1+q_0^2)}R^3+O(R^5).
$$

Its cubic coefficient is negative, so the equilibrium at equality is locally asymptotically stable, with algebraic rather than exponential decay. Thus the usual strictly decaying linear condition is $\alpha T<\pi/2$, while **nonlinear local asymptotic stability includes $\alpha T=\pi/2$**. The purely imaginary linear modes alone would not justify that borderline conclusion.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5E](../../5e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
