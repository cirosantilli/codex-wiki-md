<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The nonlinear velocity term is a divergence componentwise: $v_j\partial_jv_i=\partial_j(v_jv_i)$ because $\nabla\cdot\mathbf v=0$. Likewise $B_j\partial_jB_i=\partial_j(B_jB_i)$; their [volume averages](../../../../../../volume-average.md) vanish. Pressure gradients, spatial Laplacians and the background-advection term $x\partial_y$ also average to zero by the boundary identities. The mean momentum equation is therefore

$$
\boxed{\frac{d\langle\mathbf v\rangle}{dt}-2A\langle v_x\rangle\mathbf e_y
+2\Omega\mathbf e_z\times\langle\mathbf v\rangle=0}.
$$

In induction, the two nonlinear terms are divergences, $v_j\partial_jB_i=\partial_j(v_jB_i)$ and $B_j\partial_jv_i=\partial_j(B_jv_i)$. Averaging consequently gives

$$
\boxed{\frac{d\langle\mathbf B\rangle}{dt}+2A\langle B_x\rangle\mathbf e_y=0}.
$$

The radial and vertical mean magnetic fields stay constant, and $\langle B_y\rangle(t)=\langle B_y\rangle(0)-2At\langle B_x\rangle(0)$. In particular an initially zero mean magnetic field stays zero.

Writing $V_i=\langle v_i\rangle$, the horizontal mean motion satisfies

$$
\dot V_x=2\Omega V_y,\qquad \dot V_y=-2(\Omega-A)V_x,
\qquad \boxed{\ddot V_x+\kappa^2V_x=0,\quad\kappa^2=4\Omega(\Omega-A)}.
$$

This is the local [radial epicyclic frequency](../../../../../../radial-epicyclic-frequency.md). When the background is centrifugally stable, $\Omega(\Omega-A)>0$, the whole box supports epicyclic mean-velocity oscillations. For example,

$$
V_x=C\cos\kappa t+D\sin\kappa t,\qquad
V_y=\frac{\kappa}{2\Omega}[-C\sin\kappa t+D\cos\kappa t],
$$

while $V_z$ is constant. A [Keplerian shearing sheet](../../../../../../keplerian-shearing-sheet.md) has $\kappa=\Omega$. For a centrifugally unstable rotation law the same mean equations instead give exponential growth, so an oscillation interpretation requires the positive squared frequency.

No divergence of turbulent stress survives the box average, and a zero initial mean radial velocity cannot acquire a secular accretion drift from internal stresses. More generally, a steady horizontal mean flow has $V_x=V_y=0$ for the usual nondegenerate rotating disk. The epicycle has zero time-averaged radial velocity. Opposite radial faces are identified rather than connected to a central sink and an outer mass reservoir: material crossing a face re-enters the opposite one after an azimuthal shift. Thus **the shearing box can model angular-momentum transport and its local stresses, but not develop a global disk accretion flow**. Such accretion needs radial gradients, boundaries and mass exchange omitted from the homogeneous local model.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
