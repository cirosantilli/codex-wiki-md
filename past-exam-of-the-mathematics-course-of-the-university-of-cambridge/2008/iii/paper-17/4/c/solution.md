<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $H$ be the horizontal lift of $iv$ supplied by the [canonical coframe of a surface unit tangent bundle](../../../../../../canonical-coframe-of-a-surface-unit-tangent-bundle.md). The frame $(X,H,V)$ has commutators

$$
[V,X]=H,\qquad [V,H]=-X,\qquad [X,H]=KV.
$$

Since $F=X+\lambda V$, the [Lie bracket](../../../../../../lie-bracket.md) product rule gives

$$
[F,V]=-H-(V\lambda)V,\qquad
[F,H]=-\lambda F+(K-H\lambda+\lambda^2)V.
$$

These formulas hold for every smooth $\lambda$, with no curvature or Anosov assumption.

Follow a tangent variation $\xi(t)=D\phi_t\xi(0)$ and express it in the moving frame as

$$
\xi(t)=a(t)F+y(t)H+z(t)V.
$$

Pulling this identity back by $D\phi_{-t}$ makes its left side constant. The derivative of the pulled-back frame vector $B$ is the pulled-back bracket $[F,B]$, so the coefficients satisfy

$$
\dot a=\lambda y,\qquad
\dot y=z,\qquad
\dot z=-(K-H\lambda+\lambda^2)y+(V\lambda)z.
$$

This derives the [linearized transverse equation for a surface thermostat](../../../../../../linearized-transverse-equation-for-a-surface-thermostat.md); its first equation in $a$ disappears on the quotient by $F$.

Near a vertical plane, $z\ne0$, and the smooth projective coordinate $r=y/z$ describes the plane as

$$
L=\mathbb RF+\mathbb R(V+rH).
$$

The [vertical Maslov cycle of a surface thermostat](../../../../../../vertical-maslov-cycle-of-a-surface-thermostat.md) is exactly $r=0$. Differentiating the quotient with the derived equations yields

$$
\dot r=1-(V\lambda)r+(K-H\lambda+\lambda^2)r^2.
$$

Consequently

$$
\boxed{F^*r=1\quad\text{on }\Lambda_V.}
$$

Since $r$ is a local defining function for the hypersurface, the nonzero normal derivative proves that **the lifted vector field is transverse to the Maslov cycle everywhere**. In particular, the sign follows from the forward derivative lift and the positive vertical-rotation convention, rather than from an unspecified projective orientation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
