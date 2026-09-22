<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the standard [A-stability](../../../../../../a-stability.md) convention including the root condition at $z=h\lambda=0$. The [amplification polynomial of a multistep method](../../../../../../amplification-polynomial-of-a-multistep-method.md) is

$$
P_z(\zeta)=\left(1-\frac{1+a}{2}z\right)\zeta^2
-\left(1+a+\frac{1-3a}{2}z\right)\zeta+a.
$$

[Zero-stability](../../../../../../zero-stability.md) first restricts the possible parameters to $-1\leq a<1$. For $-1<a<0$, as $z$ tends to negative infinity, one amplification root tends to $(3a-1)/(1+a)$, whose modulus exceeds one. For $a=-1$, the characteristic equation is $\zeta^2-2z\zeta-1=0$; large negative real $z$ likewise gives an exterior root. Thus $a\geq0$ is necessary.

For sufficiency take $0\leq a<1$. The leading coefficient cannot vanish in the closed left half-plane. On the unit circle $\zeta=e^{i\theta}$ the [boundary-locus test for multistep A-stability](../../../../../../boundary-locus-test-for-multistep-a-stability.md) uses $z=\rho(\zeta)/\sigma(\zeta)$ and gives

$$
\operatorname{Re}z
=\frac{4a(1+a)(1-\cos\theta)^2}
{|1-3a+(1+a)e^{i\theta}|^2}\geq0
$$

where the denominator is nonzero. When $a=0$, the exceptional zero of $\sigma$ at $\zeta=-1$ is not a zero of $\rho$ and therefore cannot be an amplification root for a finite $z$. Near $z=0$ on the negative real axis, the root issuing from one is $1+z+O(z^2)$ and is strictly inside the disk; the other root is close to $a$ and is also inside. Roots vary continuously, cannot escape through infinity because the leading coefficient is nonzero, and cannot cross the unit circle anywhere in the open left half-plane by the displayed boundary formula. Thus every root remains inside there. Continuity gives the boundary case; for $a>0$ a unit root on the imaginary axis can occur only at $z=0$, where it is simple. For $a=0$, cancellation of the harmless zero root leaves the [trapezoidal rule](../../../../../../trapezoidal-rule.md), whose amplification factor has modulus at most one.

Therefore

$$
\boxed{0\leq a<1\quad\text{for A-stability}.}
$$

The third-order member is convergent but not [A-stable](../../../../../../a-stability.md), consistent with the [Second Dahlquist barrier](../../../../../../second-dahlquist-barrier.md). At $a=1$, $P_z=(\zeta-1)[(1-z)\zeta-1]$ has a permanent unit root and a double root at $z=0$: the unreduced method is not [zero-stable](../../../../../../zero-stability.md) and is not [A-stable](../../../../../../a-stability.md) under the stated convention. Testing only the open half-plane while overlooking its zero-step behavior would give a weaker conclusion.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
