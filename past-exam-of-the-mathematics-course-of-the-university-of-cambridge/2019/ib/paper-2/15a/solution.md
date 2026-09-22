<h1 id="15a/solution">Solution</h1>

↑ **Parent:** [15A](../15a.md)

The two [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) are

$$
\frac d{dx}\frac{\partial f}{\partial u'}-\frac{\partial f}{\partial u}=0,
\qquad
\frac d{dx}\frac{\partial f}{\partial w'}-\frac{\partial f}{\partial w}=0.
$$

Differentiating $\kappa=f-u'f_{u'}-w'f_{w'}$ along an extremal and using these equations gives $d\kappa/dx=f_x$. Hence the [Beltrami identity](../../../../../beltrami-identity.md) makes $\kappa$ constant when $f$ has no explicit dependence on $x$. If $f$ omits $u$ or $w$, that variable is a [cyclic coordinate](../../../../../cyclic-coordinate.md) and the corresponding momentum $f_{u'}$ or $f_{w'}$ is an additional [first integral](../../../../../first-integral.md); continuous symmetries give the analogous conserved quantities through [Noether's theorem](../../../../../noether-conserved-quantity-for-a-mechanical-point-symmetry.md).

Put $A=1-m/u$. Since $w$ is cyclic,

$$
2Aw'=2\lambda,
\qquad Aw'=\lambda
$$

for a constant $\lambda$. The Beltrami integral is

$$
\kappa=f-u'f_{u'}-w'f_{w'}
=A^{-1}u'^2-Aw'^2
=A^{-1}(u'^2-\lambda^2).
$$

Therefore

$$
\boxed{u'^2=\lambda^2+\kappa\left(1-\frac mu\right)}.
$$

If $\kappa=-\lambda^2$, then $u'^2=\lambda^2m/u$ and

$$
\frac{dw}{du}=\pm\frac{(u/m)^{3/2}}{u/m-1}.
$$

For $z>1$, define

$$
F(z)=\frac23z^{3/2}+2z^{1/2}
+\log\frac{\sqrt z-1}{\sqrt z+1};
$$

the hinted identity gives $F'(z)=z^{3/2}/(z-1)$. Hence $w=C\pm mF(u/m)$. Because $F(z)\to+\infty$ as $z\to\infty$, the prescribed limit selects the minus sign:

$$
\boxed{w(u)=C-m\left[
\frac23\left(\frac um\right)^{3/2}
+2\sqrt{\frac um}
+\log\frac{\sqrt{u/m}-1}{\sqrt{u/m}+1}
\right]}.
$$

As $u\downarrow m$, the logarithm tends to $-\infty$, so every such solution satisfies $\boxed{w\to+\infty}$.

## ↑ Ancestors (10)

1. [15A](../15a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
