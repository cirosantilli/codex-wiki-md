<h1 id="4b/solution">Solution</h1>

↑ **Parent:** [4B](../4b.md)

Use the inverse [Lorentz transformation](../../../../../lorentz-transformation.md)

$$
x=\gamma_v(x'+vt'),\qquad
t=\gamma_v(t'+vx'/c^2).
$$

Along the particle's worldline $dx'=u'\,dt'$, so the [relativistic velocity-addition formula](../../../../../velocity-addition-formula.md) is

$$
\boxed{u=\frac{u'+v}{1+u'v/c^2}.}
$$

For subluminal collinear [velocities](../../../../../velocity.md), put $u/c=\tanh\varphi_u$, $u'/c=\tanh\varphi_{u'}$ and $v/c=\tanh\varphi_v$. The [hyperbolic tangent](../../../../../hyperbolic-tangent.md) addition formula, obtained by dividing the supplied sine/cosine addition formulas, gives

$$
\tanh\varphi_u=\tanh(\varphi_{u'}+\varphi_v).
$$

Because [hyperbolic tangent](../../../../../hyperbolic-tangent.md) is [injective](../../../../../injective-function.md) on the real line,

$$
\boxed{\varphi_u=\varphi_{u'}+\varphi_v.}
$$

Thus [rapidity](../../../../../rapidity.md) is additive even though [velocity](../../../../../velocity.md) is not.

Each positive increment in the instantaneous rest frame adds the same [rapidity](../../../../../rapidity.md) $\alpha=\operatorname{artanh}(1/2)=\tfrac12\log3$. Starting from zero [rapidity](../../../../../rapidity.md), [iterated collinear boosts with equal rapidity](../../../../../iterated-collinear-boosts-with-equal-rapidity.md) give

$$
\boxed{u_n=c\tanh(n\alpha)
=c\frac{e^{2n\alpha}-1}{e^{2n\alpha}+1}
=c\frac{3^n-1}{3^n+1}.}
$$

Every finite number of increments leaves $u_n<c$; the [speed of light](../../../../../speed-of-light.md) is approached as $n\to\infty$.

## ↑ Ancestors (10)

1. [4B](../4b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
