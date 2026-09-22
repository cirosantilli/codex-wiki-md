<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a circular mid-plane orbit, radial force balance in the [Newtonian gravitational potential](../../../../../../newtonian-gravitational-potential.md) is $r\Omega^2=\Phi_{,r}$. Hence

$$
\boxed{\Omega^2(r)=\frac1r\Phi_{,r}(r,0)}.
$$

Axisymmetry conserves the [specific angular momentum](../../../../../../specific-angular-momentum.md) $j=r^2\dot\phi$. At fixed $j$, radial motion obeys $\ddot r=-\partial_r\Phi_{\rm eff}$, where the [effective potential](../../../../../../effective-potential.md) is $\Phi_{\rm eff}=\Phi+j^2/(2r^2)$. Linearize around a circular radius $r_0$, writing $r=r_0+\xi$. Since $j^2=r_0^3\Phi_{,r}(r_0,0)$ there,

$$
\ddot\xi+\kappa^2\xi=0,\qquad
\boxed{\kappa^2=\Phi_{,rr}(r_0,0)+\frac3{r_0}\Phi_{,r}(r_0,0)}.
$$

This is the [radial epicyclic frequency](../../../../../../radial-epicyclic-frequency.md); equivalently $\kappa^2=r^{-3}d(r^4\Omega^2)/dr$.

Reflection symmetry gives $\Phi_{,z}(r,0)=0$ and $\Phi_{,rz}(r,0)=0$, so vertical and radial displacements decouple at linear order. The vertical equation is $\ddot z=-\Phi_{,zz}(r_0,0)z$, giving the [vertical epicyclic frequency](../../../../../../vertical-epicyclic-frequency.md)

$$
\boxed{\Omega_z^2(r_0)=\Phi_{,zz}(r_0,0)}.
$$

Positive squared frequencies give oscillatory stability; a negative squared frequency gives exponential instability rather than a real oscillation frequency.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
