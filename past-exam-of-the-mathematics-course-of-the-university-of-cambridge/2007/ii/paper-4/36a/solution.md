<h1 id="36a/solution">Solution</h1>

↑ **Parent:** [36A](../36a.md)

Vary the curve by $\delta x^c$, fixing endpoints. Integration by parts in the kinetic functional gives its Euler-Lagrange equations

$$
\frac d{d\lambda}(2g_{cb}\dot x^b)-\partial_cg_{ab}\dot x^a\dot x^b=0.
$$

Multiplying by $g^{cd}/2$ and symmetrizing the velocity product gives

$$
\boxed{\ddot x^d+\Gamma^d_{ab}\dot x^a\dot x^b=0,\qquad
\Gamma^d_{ab}=\tfrac12g^{dc}(\partial_ag_{bc}+\partial_bg_{ac}-\partial_cg_{ab}).}
$$

There is no term proportional to $\dot x$ from parameter reparametrization, so this is the affine [geodesic equation](../../../../../geodesic-equation.md).

In units $c=1$, the static spherical vacuum metric is Schwarzschild with $f(r)=1-2GM/r$. For example, starting from $-e^{2\Phi}dt^2+e^{2\Lambda}dr^2+r^2d\Omega^2$, the vacuum radial equations give $[r(1-e^{-2\Lambda})]'=0$ and $\Phi'+\Lambda'=0$. Asymptotic flatness and the Newtonian mass fix $e^{2\Phi}=e^{-2\Lambda}=1-2GM/r$, giving the displayed metric. Time and azimuthal coordinates are cyclic in its [geodesic](../../../../../geodesic.md) Lagrangian, so

$$
\boxed{f\dot t=E,\qquad r^2\dot\phi=h.}
$$

Normalize the velocity norm to $-k$, with $k=1$ for proper-time parametrized massive motion and $k=0$ for null motion. In the equatorial plane this gives $\dot r^2+f(k+h^2/r^2)=E^2$. For a nonradial orbit, $h\ne0$ and $u=1/r$ imply $\dot r=-h\,du/d\phi$. Therefore

$$
\boxed{(u')^2+fu^2=-\frac{k}{h^2}f+\frac{E^2}{h^2}.}
$$

Differentiating with $f=1-2GMu$ yields

$$
\boxed{u''+u=\frac{kGM}{h^2}+3GMu^2.}
$$

It extends across isolated turning points by continuity. The original PDF's later $f=1-GMu$ is inconsistent with this claimed equation: that choice gives $u''+u=kGM/(2h^2)+(3GM/2)u^2$. The intended Schwarzschild factor is **$1-2GMu$**, which we retain.

For massive motion put $\ell=h^2/(GM)$. The Newtonian solution is $u_0=(1+e\cos\phi)/\ell$. The resonant cosine forcing in $3GMu_0^2$ is $6GMe\cos\phi/\ell^2$, producing the secular correction $3GMe\phi\sin\phi/\ell^2$. Resumming it into a shifted phase gives the precessing-ellipse approximation

$$
\boxed{u\approx\ell^{-1}[1+e\cos(\alpha\phi)],\qquad
\alpha=1-3GM/\ell.}
$$

For finite eccentricity there are also bounded corrections of this same small order: one particular correction is $3GM(1+e^2/2)/\ell^2-GMe^2\cos(2\phi)/(2\ell^2)$, besides adjustable homogeneous terms. Thus the simple displayed ellipse captures the secular precession rather than the complete first-order shape correction. Consecutive periapses are separated by $2\pi/\alpha$, so the [Schwarzschild perihelion precession](../../../../../schwarzschild-perihelion-precession.md) per radial orbit is approximately **$6\pi GM/\ell$**, forward in the direction of motion.

## ↑ Ancestors (10)

1. [36A](../36a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
