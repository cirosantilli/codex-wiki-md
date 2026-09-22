<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The in-plane [equilibrium](../../../equilibrium-point-of-a-dynamical-system.md) equations are $\tau_{xx,x}+\tau_{xy,y}=0$ and $\tau_{xy,x}+\tau_{yy,y}=0$. On a [simply connected](../../../simply-connected-space.md) patch, each [divergence-free](../../../solenoidal-vector-field.md) row has a [streamfunction](../../../stream-function.md): write $\tau_{xx}=\phi_y$, $\tau_{xy}=-\phi_x=-\psi_y$, $\tau_{yy}=\psi_x$. Symmetry gives $\phi_x=\psi_y$, so another potential exists with $A_y=\phi$, $A_x=\psi$. Hence

$$
\boxed{\tau_{xx}=A_{yy},\qquad\tau_{yy}=A_{xx},\qquad\tau_{xy}=-A_{xy}.}
$$

If two such [Airy stress functions](../../../airy-stress-function.md) give the same [stress](../../../stress.md), their difference has zero [Hessian](../../../hessian-matrix.md) and is therefore an arbitrary [affine function](../../../affine-function.md) $a+bx+cy$ on a connected domain. This is the full nonuniqueness for a fixed [stress](../../../stress.md). The existence argument is local, or global on a [simply connected](../../../simply-connected-space.md) domain; domains that are [multiply connected regions](../../../multiply-connected-region.md) require the associated force and moment period conditions for a single-valued global potential. [Equilibrium](../../../equilibrium-point-of-a-dynamical-system.md) alone should not silently erase that topological qualification.

For [plane strain](../../../plane-strain.md) put $s=e_{xx}+e_{yy}$. The [constitutive equation](../../../constitutive-equation.md) gives $\tau_{xx}+\tau_{yy}=2(\lambda+\mu)s$. Consequently

$$
e_{xx}=\frac{\tau_{xx}-\lambda s}{2\mu},\quad
e_{yy}=\frac{\tau_{yy}-\lambda s}{2\mu},\quad
e_{xy}=\frac{\tau_{xy}}{2\mu},\quad
s=\frac{\Delta A}{2(\lambda+\mu)}.
$$

The [displacement](../../../displacement.md) [Saint-Venant compatibility equations](../../../saint-venant-strain-compatibility-and-differential-identities.md) $e_{xx,yy}+e_{yy,xx}-2e_{xy,xy}=0$ then becomes

$$
0=2\mu(e_{xx,yy}+e_{yy,xx}-2e_{xy,xy})
=\frac{\lambda+2\mu}{2(\lambda+\mu)}\Delta^2A.
$$

For stable elastic moduli the coefficient is nonzero, so $\boxed{\Delta^2A=0}$. If $D$ is bounded and smooth and $A=\partial_nA=0$ on its boundary, integrating twice by parts gives $0=\int_DA\Delta^2A\,dV=\int_D(\Delta A)^2\,dV$. Thus $A$ is harmonic with zero boundary value and $\boxed{A=0}$ by uniqueness of the [Dirichlet problem](../../../dirichlet-problem.md). The normal-[derivative](../../../derivative.md) condition is what removes the extra fourth-order [boundary terms](../../../boundary-term.md).

For the pressurized [annulus](../../../annulus-mathematics.md), substituting the radial [constitutive equations](../../../constitutive-equation.md) into [equilibrium](../../../equilibrium-point-of-a-dynamical-system.md) gives $u''+u'/r-u/r^2=0$, so $u=Cr+D/r$. The stresses are

$$
\tau_{rr}=2(\lambda+\mu)C-\frac{2\mu D}{r^2},\qquad
\tau_{\theta\theta}=2(\lambda+\mu)C+\frac{2\mu D}{r^2}.
$$

Using gauge stresses relative to ambient, the boundaries are $\tau_{rr}(a)=-P$, $\tau_{rr}(b)=0$. Therefore

$$
2(\lambda+\mu)C=\frac{Pa^2}{b^2-a^2},\qquad
2\mu D=\frac{Pa^2b^2}{b^2-a^2},
$$

and

$$
\boxed{|\tau_{rr}-\tau_{\theta\theta}|=\frac{2Pa^2b^2}{(b^2-a^2)r^2},\qquad
\max_{a\leq r\leq b}|\tau_{rr}-\tau_{\theta\theta}|=\frac{2Pb^2}{b^2-a^2}.}
$$

The maximum occurs at the bore. Once the chosen [yield criterion](../../../yield-criterion.md) is reached, [Hooke's law](../../../hooke-s-law.md) cannot describe the total [strain](../../../strain.md) alone: write total [strain](../../../strain.md) as elastic plus [plastic strain](../../../plastic-strain.md) and supplement the elastic [stress](../../../stress.md) law with a yield condition, a [plastic flow rule](../../../plastic-flow-rule.md) and any required [work hardening](../../../work-hardening.md) law. A plastic region starts near the bore and must be matched to the remaining elastic region. The exact conversion between a principal-[stress](../../../stress.md) difference and the quoted [yield stress](../../../yield-stress.md) depends on whether the material criterion is Tresca or von Mises. This is the [elastic stress concentration in a pressurized thick cylinder](../../../elastic-stress-concentration-in-a-pressurized-thick-cylinder.md).

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2007](../../2007-split.md)
3. [Past exam of the elasticity and plasticity course of the University of Oxford](../../split.md)
4. [Elasticity and plasticity course of the University of Oxford](../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
