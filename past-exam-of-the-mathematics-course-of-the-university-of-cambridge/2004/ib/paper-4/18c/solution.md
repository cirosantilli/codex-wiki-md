<h1 id="18c/solution">Solution</h1>

↑ **Parent:** [18C](../18c.md)

For steady [incompressible flow](../../../../../incompressible-flow.md) of constant density without a body force, the [Euler equation](../../../../../euler-equations-for-an-inviscid-fluid.md) and mass conservation give

$$
\rho u_j\partial_j u_i=-\partial_i p,\qquad \partial_j u_j=0,
\qquad \partial_j(p\delta_{ij}+\rho u_i u_j)=0.
$$

Apply the [divergence theorem](../../../../../divergence-theorem.md) componentwise to a fluid volume. With $\mathbf n$ its outward normal, the integral [momentum flux](../../../../../momentum-flux.md) balance is

$$
\boxed{\int_{\partial V}\left(p\mathbf n+\rho\mathbf u(\mathbf u\cdot\mathbf n)\right)dS=\mathbf0.}
$$

If a solid bounds part of the volume, retain its pressure contribution; that contribution supplies the force on the fluid. This derivation includes pressure as well as transported momentum.

Choose the axis in the incoming jet direction. The printed diagram measures $\alpha$ between that axis and the downstream sheet: it is the cone's half-angle. Along a streamline, the steady Euler equation integrates to the [Bernoulli equation](../../../../../bernoulli-equation.md) $p/\rho+|\mathbf u|^2/2=\text{constant}$. At the incoming free jet and the outgoing free sheet the pressure is atmospheric. With gravity neglected, the outgoing speed is therefore $u$. This argument uses far free surfaces; it does not assert atmospheric pressure on the wetted sphere.

At radial distance $r$, the sheet's circumference is $2\pi r\sin\alpha$. Its cross-section normal to its velocity is this circumference times its small thickness $d$. [Conservation of mass](../../../../../mass-conservation.md) gives $Au=(2\pi r\sin\alpha)du$, hence

$$
\boxed{d=\frac{A}{2\pi r\sin\alpha}.}
$$

For the axial momentum balance, transverse contributions cancel by axial symmetry. The outgoing axial momentum rate is $\rho Au^2\cos\alpha$ and the incoming rate is $\rho Au^2$. Uniform atmospheric pressure cancels on the closed control surface when expressed as gauge pressure. The sphere's force on the fluid is therefore $\rho Au^2(\cos\alpha-1)$ in the axis direction. By action and reaction, **the fluid force on the sphere is downstream**, with magnitude

$$
\boxed{F=\rho Au^2(1-\cos\alpha).}
$$

The downstream direction in the original diagram fixes this sign and the factor $1-\cos\alpha$. If one calls the full cone opening its vertex angle, that full opening is $2\alpha$; using $\alpha$ as the full opening would conflict with the printed thickness formula.

## ↑ Ancestors (10)

1. [18C](../18c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
