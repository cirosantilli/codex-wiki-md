<h1 id="section-c/c12/solution">Solution</h1>

↑ **Parent:** [C12](../c12.md)

**Normal-mode idea.** Near a stable equilibrium, expand the [potential energy](../../../../../potential-energy.md) to quadratic order and the [kinetic energy](../../../../../kinetic-energy.md) as a quadratic form in generalized velocities. The [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) then take the linear form $\mathsf M\ddot{\mathbf x}+\mathsf K\mathbf x=0$. A [normal mode](../../../../../normal-mode.md) has fixed displacement ratios, $\mathbf x=\mathbf q\cos(\omega t+\varphi)$, with $\mathsf K\mathbf q=\omega^2\mathsf M\mathbf q$. Real systems admit this description for sufficiently small motion, before higher-order nonlinearities or strong damping matter. [Superposition](../../../../../superposition-principle.md) permits a general motion to be assembled from the modes. A free symmetry direction may instead be a [zero mode](../../../../../zero-mode.md), with constant or linearly changing coordinate.

**Lagrangian and bead equations.** Take each $x_i$ as an arc-length displacement positive in the same sense around the fixed circular wire. Spring length changes are $x_2-x_1$, $x_3-x_2$ and $x_1-x_3$. Equal equilibrium spring tensions give no net tangential [force](../../../../../force-split.md); their linear energy terms sum to zero. Dropping an irrelevant constant, the [Lagrangian](../../../../../lagrangian.md) is

$$
\boxed{\mathcal L=\frac m2(\dot x_1^2+\dot x_2^2+\dot x_3^2)
-\frac k2\left[(x_2-x_1)^2+(x_3-x_2)^2+(x_1-x_3)^2\right].}
$$

For example, differentiating the potential with respect to $x_1$ gives $k(2x_1-x_2-x_3)$. The three [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) therefore are

$$
\boxed{\begin{aligned}
m\ddot x_1&=-k(2x_1-x_2-x_3),\\
m\ddot x_2&=-k(2x_2-x_3-x_1),\\
m\ddot x_3&=-k(2x_3-x_1-x_2).
\end{aligned}}
$$

The wire supplies normal constraint forces but does no tangential work. These are the equal-mass case of the [normal modes of three beads connected by springs on a circular hoop](../../../../../normal-modes-of-three-beads-connected-by-springs-on-a-circular-hoop.md).

**Frequencies.** The stiffness matrix divided by $k$ is

$$
\mathsf K/k=\begin{pmatrix}2&-1&-1\\-1&2&-1\\-1&-1&2\end{pmatrix}
=3\mathsf I-\mathbf 1\mathbf 1^{\mathsf T},\qquad
\mathbf 1=(1,1,1)^{\mathsf T}.
$$

It annihilates $\mathbf 1$. On the two-dimensional subspace $q_1+q_2+q_3=0$, its action is multiplication by three. Thus the [angular frequencies](../../../../../angular-frequency.md) of the [normal modes](../../../../../normal-mode.md) are

$$
\boxed{\omega_0=0,\qquad\omega_1=\omega_2=\sqrt{\frac{3k}{m}}.}
$$

The repeated [frequency](../../../../../frequency.md) is a [degeneracy of normal modes](../../../../../degeneracy-of-normal-modes.md), while the zero [frequency](../../../../../frequency.md) expresses free rigid [rotation](../../../../../rotation-mathematics.md) of all beads along the wire.

**General solution.** Two independent vectors spanning the vibrating subspace are $\mathbf q_A=(1,-1,0)^{\mathsf T}$ and $\mathbf q_B=(1,0,-1)^{\mathsf T}$. Each amplitude satisfies $\ddot Q+\omega^2Q=0$, with $\omega=\sqrt{3k/m}$. The uniform coordinate satisfies $\ddot Q_0=0$. Hence

$$
\boxed{\mathbf x(t)=\mathbf q_A A\cos(\omega t+\phi)
+\mathbf q_B B\cos(\omega t+\psi)
+\mathbf 1(Ct+D).}
$$

The six freely specifiable real constants $A,\phi,B,\psi,C,D$ give the six initial data; $\omega$ is fixed by $k,m$ and is not an additional independent integration constant. The linear zero-mode term must be included to allow nonzero total tangential momentum.

**Shapes and uniqueness.** In the first term beads 1 and 2 have opposite equal displacements and bead 3 remains at its equilibrium position. In the second term beads 1 and 3 do this while bead 2 stays fixed. The last term moves all three identically, leaving spring extensions unchanged: $D$ is a rigid phase shift and $C$ a uniform drift around the wire. The sketches show positive modal amplitudes; all arrows reverse half a vibration period later.

<a id="section-c/c12/image-original-displacement-sketches-for-two-independent-equal-frequency-bead-modes-and-the-rigid-rotation-zero-mode-arrows-indicate-displacement-along-the-ring-rather-than-its-radius"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-1-c12-ring-mode-shapes.png)

**[Figure 4](#section-c/c12/image-original-displacement-sketches-for-two-independent-equal-frequency-bead-modes-and-the-rigid-rotation-zero-mode-arrows-indicate-displacement-along-the-ring-rather-than-its-radius). Original displacement sketches for two independent equal-frequency bead modes and the rigid-rotation zero mode; arrows indicate displacement along the ring rather than its radius**.

The two nonzero-[frequency](../../../../../frequency.md) [eigenvectors](../../../../../eigenvector.md) are not unique, because any independent linear combinations in their degenerate two-dimensional [eigenspace](../../../../../eigenspace.md) form an equally valid basis. In particular the displayed pair is independent but not orthogonal; one could use $(1,-1,0)$ and $(1,1,-2)$ instead. The zero [eigenspace](../../../../../eigenspace.md) is one-dimensional, so its vector is fixed up to scale and sign.

**Specified release.** Zero initial velocities permit $\phi=\psi=0$ and require $C=0$. At $t=0$, the three displacement conditions become $A+B+D=a$, $-A+D=0$, $-B+D=0$. Therefore one convenient set of constants is

$$
\boxed{A=B=D=\frac a3,\quad C=0,\quad\phi=\psi=0,
\quad\omega=\sqrt{3k/m}.}
$$

Equivalently,

$$
\boxed{x_1(t)=\frac a3[1+2\cos(\omega t)],\qquad
x_2(t)=x_3(t)=\frac a3[1-\cos(\omega t)].}
$$

Their sum remains $a$, as required by zero initial total tangential momentum. Alternative amplitude signs with compensating phase shifts represent the same motion.

## ↑ Ancestors (14)

1. [C12](../c12.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
