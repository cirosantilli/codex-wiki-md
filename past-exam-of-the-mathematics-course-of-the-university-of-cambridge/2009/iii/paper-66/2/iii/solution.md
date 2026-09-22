<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The stated real trigonometric substitution applies to the closed case $q_0>1/2$. Set $A=2q_0-1$, so $x=q_0(1-\cos\theta)/A$, $dx=q_0\sin\theta\,d\theta/A$, and

$$
1-2q_0+\frac{2q_0}{x}=A\frac{1+\cos\theta}{1-\cos\theta}.
$$

The upper limit obeys $1-\cos\theta_*=A/q_0$, with $0<\theta_*<\pi$ on the expanding branch. Substitution into the [age of a dust universe without a cosmological constant](../../../../../../age-of-a-dust-universe-without-a-cosmological-constant.md) yields

$$
\boxed{H_0t_0=\frac{q_0}{(2q_0-1)^{3/2}}\int_0^{\theta_*}\frac{\sin\theta\sqrt{1-\cos\theta}}{\sqrt{1+\cos\theta}}\,d\theta.}
$$

On this interval, the integrand equals $1-\cos\theta$, so it can also be evaluated:

$$
H_0t_0=\frac{q_0(\theta_*-\sin\theta_*)}{(2q_0-1)^{3/2}},\qquad\cos\theta_*=\frac{1-q_0}{q_0}.
$$

For $q_0=1/2$, the original integral instead gives $H_0t_0=2/3$. For $0<q_0<1/2$, use a hyperbolic substitution to obtain $H_0t_0=q_0(\sinh\eta_*-\eta_*)/(1-2q_0)^{3/2}$, where $\cosh\eta_*=(1-q_0)/q_0$. A real $\theta$ cannot implement the printed substitution in that open case.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
