<h1 id="15b/solution">Solution</h1>

↑ **Parent:** [15B](../15b.md)

For a stationary spherically symmetric state, set $u(r)=r\psi(r)$. The [Schrödinger equation](../../../../../schrodinger-equation.md) becomes

$$
-\frac{\hbar^2}{2m}u''+V(r)u=Eu.
$$

A [bound state](../../../../../bound-state.md) must have $E<0$, while the well's lower bound gives $E>-U$ for a nonzero square-integrable eigenstate. Define $k=\sqrt{2m(U+E)}/\hbar$ and $\kappa=\sqrt{-2mE}/\hbar$. Regularity at the origin requires $u(0)=0$, so the interior cosine solution is excluded; square integrability at infinity excludes the growing exterior exponential. Matching $u$ and $u'$ at $r=a$ therefore gives

$$
\boxed{\psi(r)=C\begin{cases}
\sin(kr)/r,&0<r\leq a,\\
\sin(ka)e^{-\kappa(r-a)}/r,&r\geq a,
\end{cases}\qquad k\cot(ka)=-\kappa.}
$$

The limit at the origin is the finite value $Ck$. Continuity of $u,u'$ is equivalent here to continuity of $\psi,\psi'$ at the finite potential jump. If desired, the normalized state has

$$
|C|^{-2}=4\pi\left[\frac a2-\frac{\sin(2ka)}{4k}+\frac{\sin^2(ka)}{2\kappa}\right].
$$

The equation for $k$ implicitly determines the energy, with $k^2+\kappa^2=2mU/\hbar^2$.

Write $K=a\sqrt{2mU}/\hbar$ and $z=ka$. The matching condition is $z\cot z=-\sqrt{K^2-z^2}$. The first possible solution has $\pi/2<z<\pi$. If $K\leq\pi/2$, every permitted interior $z<K$ has nonnegative cotangent and cannot match a negative exterior logarithmic [derivative](../../../../../derivative.md). If $K>\pi/2$, at $z\downarrow\pi/2$ the sum $z\cot z+\sqrt{K^2-z^2}$ is positive; it is negative either at $z\uparrow K$ when $K<\pi$, or at $z\uparrow\pi$ when $K\geq\pi$. Continuity supplies a first bound-state solution. Thus **at least one spherically symmetric [bound state](../../../../../bound-state.md) exists exactly when**

$$
\boxed{U>\frac{\pi^2\hbar^2}{8ma^2}.}
$$

At equality the limiting energy is zero and the exterior wave is proportional to $1/r$, whose norm diverges. Hence the inequality is strict. Deeper wells can support additional radial states; their negative-energy matching solutions have the same displayed form. This is the [spherically symmetric bound state of a finite well](../../../../../spherically-symmetric-bound-state-of-a-finite-well.md).

## ↑ Ancestors (10)

1. [15B](../15b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
