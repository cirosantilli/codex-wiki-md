# Paper 140

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_140.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_140.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 140](paper-140.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use polar coordinates $z_j=r_je^{i\theta_j}$ on each complex coordinate plane. On $S^3$, where $r_1^2+r_2^2=1$,

$$
\alpha_s=\frac12(r_1^2d\theta_1+sr_2^2d\theta_2),
\qquad
d\alpha_s=r_1dr_1\wedge d\theta_1+sr_2dr_2\wedge d\theta_2.
$$

Direct substitution shows that $\alpha_s\wedge d\alpha_s$ is nowhere zero for $s>0$, so $\alpha_s$ is a [contact form](../../../differential-geometry.md#contact-form).

The vector field

$$
R_s=2\frac{\partial}{\partial\theta_1}+\frac2s\frac{\partial}{\partial\theta_2}
$$

satisfies $\alpha_s(R_s)=r_1^2+r_2^2=1$ and $\iota_{R_s}d\alpha_s=0$ on tangent vectors to the sphere. It is therefore the [Reeb vector field](../../../differential-geometry.md#reeb-vector-field). Its flow is

$$
(z_1,z_2)\longmapsto(e^{2it}z_1,e^{2it/s}z_2).
$$

If both coordinates are nonzero, an orbit closes only if the two angular frequencies have rational ratio, equivalently if $s\in\mathbb Q$. For irrational $s$, the only closed orbits are $\{z_2=0\}$ and $\{z_1=0\}$, the two coordinate circles. This is the [irrational contact ellipsoid flow on the three-sphere](../../../differential-geometry.md#irrational-contact-ellipsoid-flow-on-the-three-sphere).

## 2

↑ **Parent:** [Paper 140](paper-140.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [Weinstein neighborhood theorem](../../../symplectic-geometry.md#weinstein-neighborhood-theorem) identifies a neighborhood of $X$ in $M$ with a neighborhood of the zero section in $T^*X$. If $j$ is sufficiently $C^1$-close to the inclusion, projection of its image to $X$ is a diffeomorphism. After reparametrization, $j(X)$ is therefore the graph of a small one-form $\beta$.

The [graph of a closed one-form is Lagrangian](../../../symplectic-geometry.md#graph-of-a-closed-one-form-is-lagrangian) criterion says that $j(X)$ is Lagrangian exactly when $d\beta=0$. Since $H^1(X;\mathbb R)=0$, write $\beta=df$. Intersections of $j(X)$ with $X$ are the critical points of $f$. A smooth function on a compact manifold has a maximum and a minimum; if they coincide as points because $f$ is constant, every point is an intersection. Thus there are at least two intersection points, proving the [nearby exact Lagrangian intersection lemma](../../../symplectic-geometry.md#nearby-exact-lagrangian-intersection-lemma).

The cohomology hypothesis is necessary. Take the zero section in $T^*S^1$ and the graph of the arbitrarily small nowhere-zero closed one-form $\varepsilon,d\theta$. Both are Lagrangian and disjoint.

## 3

↑ **Parent:** [Paper 140](paper-140.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Define the [cotangent lift of a diffeomorphism](../../../symplectic-geometry.md#cotangent-lift-of-a-diffeomorphism)

$$
f_\#(x,\xi)=\left(f(x),(df_x^{-1})^*\xi\right).
$$

If $\alpha$ is the canonical one-form and $W\in T_{(x,\xi)}T^*X$, then

$$
(f_\#^*\alpha)_{(x,\xi)}(W)
=((df_x^{-1})^*\xi)(df_x(d\pi W))
=\xi(d\pi W)=\alpha_{(x,\xi)}(W).
$$

**Hence $f_\#^*\alpha=\alpha$.**

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The area form $\sigma$ on $S^2$ is closed. For any closed two-form $B$ on a base, the [twisted cotangent symplectic form](../../../symplectic-geometry.md#twisted-cotangent-symplectic-form) $\omega+\pi^*B$ is closed and nondegenerate: pairing a putative kernel vector first with vertical vectors kills its horizontal component, and then pairing with horizontal vectors kills its vertical component. Thus both $\omega_+$ and $\omega_-$ are symplectic.

The cotangent bundle deformation-retracts onto its zero section. Their cohomology classes satisfy

$$
[\omega_+]-[\omega_-]=2\pi^*[\sigma]\ne0\in H^2(T^*S^2;\mathbb R).
$$

They are therefore not [strongly isotopic](../../../symplectic-geometry.md#strong-isotopy-of-symplectic-forms).

Let $f:S^2\to S^2$ be an orientation-reversing isometry. Then $f^*\sigma=-\sigma$, while its cotangent lift preserves the canonical form and satisfies $\pi\circ f_\#=f\circ\pi$. Consequently

$$
f_\#^*\omega_+=\omega+\pi^*f^*\sigma=\omega_-,
$$

so the two forms are [symplectomorphic](../../../symplectic-geometry.md#symplectomorphism).

## 4

↑ **Parent:** [Paper 140](paper-140.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

If $H|_L$ is constant, then $dH(v)=0$ for every $v\in TL$. By the definition of the [Hamiltonian vector field](../../../symplectic-geometry.md#hamiltonian-vector-field),

$$
\omega(X_H,v)=-dH(v)=0.
$$

Since $L$ is [Lagrangian](../../../symplectic-geometry.md#lagrangian-submanifold), $(TL)^\omega=TL$, so $X_H$ is tangent to $L$. Its [Hamiltonian flow](../../../symplectic-geometry.md#hamiltonian-isotopy) preserves $L$. This is the [Hamiltonian flow preserves a constant-level Lagrangian](../../../symplectic-geometry.md#hamiltonian-flow-preserves-a-constant-level-lagrangian) principle.

The cotangent lift is functorial:

$$
(f\circ g)_\#=f_\#\circ g_\#.
$$

Since $\phi_{t+s}=\phi_t\circ\phi_s$, it follows that

$$
\psi_{t+s}=(\phi_{t+s})_\#=(\phi_t)_\#\circ(\phi_s)_\#=\psi_t\circ\psi_s.
$$

Thus $(\psi_t)$ is a flow with infinitesimal vector field $V_\#$ as stated in the question.

Finally, a cotangent lift sends the [conormal bundle](../../../symplectic-geometry.md#conormal-bundle) $N^*Y$ to $N^*f(Y)$. Explicitly, if $\xi$ annihilates $T_xY$, then $(df_x^{-1})^*\xi$ annihilates $T_{f(x)}f(Y)$. Since $\phi_t(Y)=Y$, we have

$$
\psi_t(N^*Y)=N^*\phi_t(Y)=N^*Y,
$$

so the conormal bundle is invariant.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
