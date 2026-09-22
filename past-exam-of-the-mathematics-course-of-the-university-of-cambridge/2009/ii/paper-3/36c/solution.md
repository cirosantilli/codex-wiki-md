<h1 id="36c/solution">Solution</h1>

↑ **Parent:** [36C](../36c.md)

Use $c=1$ and metric signature $(-,+,+,+)$, consistent with the supplied rest potential. In the [Lorenz gauge](../../../../../lorenz-gauge-condition.md), the Maxwell equations reduce to wave equations for the four-potential. A point worldline has current $j^a(x)=q\int u^a(s)\delta^{(4)}(x-y(s))ds$, where $u^a=dy^a/ds$. Convolution with the retarded wave Green function $\theta(R^0)\delta(R^2)/(2\pi)$ gives the stated integral: its support is the future light cone of each source point and it excludes incoming advanced signals.

For uniform motion $y^a(s)=(\gamma s,0,0,\gamma vs)$, $u^a=\gamma(1,0,0,v)$. Let $R=x-y(s)$. The delta-function argument has derivative $d(R^2)/ds=-2R\cdot u$. Only the retarded root survives the step function, so

$$
A^a(x)=\frac{\mu_0q}{4\pi}\left.\frac{u^a}{-R\cdot u}\right|_{\mathrm{ret}}.
$$

Put $Z=z-vt$, $r_\perp^2=x^2+y^2$, and $\Delta=t-t_{\mathrm{ret}}>0$. The light-cone condition is $\Delta^2=r_\perp^2+(Z+v\Delta)^2$, whence

$$
\Delta=\frac{vZ+\sqrt{Z^2+(1-v^2)r_\perp^2}}{1-v^2},\qquad
-R\cdot u=\gamma[(1-v^2)\Delta-vZ]=\gamma\sqrt{Z^2+(1-v^2)r_\perp^2}.
$$

Therefore, away from the worldline,

$$
\boxed{\phi=\frac{\mu_0q}{4\pi\sqrt{(z-vt)^2+(1-v^2)(x^2+y^2)}},\qquad A_z=v\phi,\quad A_x=A_y=0.}
$$

As an independent check, in the rest frame $z'=\gamma(z-vt)$ and $r'=\sqrt{x^2+y^2+\gamma^2Z^2}$. Its potential is $A'^a=(\mu_0q/(4\pi r'),0,0,0)$. A [Lorentz transformation](../../../../../lorentz-transformation.md) gives $A^0=\gamma A'^0$, $A^z=\gamma vA'^0$, exactly the expression above because $r'=\gamma\sqrt{Z^2+(1-v^2)r_\perp^2}$. Restoring SI units would require restoring the factors of $c$ in both the four-potential convention and the supplied electrostatic normalization.

## ↑ Ancestors (10)

1. [36C](../36c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
