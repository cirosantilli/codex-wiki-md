# Paper 308

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_308.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_308.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 308](paper-308.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write

$$
V(\phi)=\frac12(q^2-\phi^2)^2(p^2-\phi^2)^2,
\qquad q>p>0.
$$

The four vacua are $-q,-p,p,q$. Hence there are three adjacent [scalar-field kink](../../../classical-field-theory-soliton.md#scalar-field-kink) sectors, $(-q,-p)$, $(-p,p)$ and $(p,q)$, together with their three reversed antikinks. With

$$
W'(\phi)=(q^2-\phi^2)(p^2-\phi^2),
\qquad
W(\phi)=p^2q^2\phi-\frac{p^2+q^2}{3}\phi^3+\frac15\phi^5,
$$

the [Bogomolny bound](../../../quantum-field-theory.md#bogomolny-bound) gives $E=|W(\phi_+)-W(\phi_-)|$. The central kink obeys $\phi'=W'(\phi)$ and has

$$
E_c=\frac{4p^3}{15}(5q^2-p^2).
$$

The two outer kinks obey $\phi'=-W'(\phi)$ and have equal energy

$$
E_o=\frac{2}{15}(q-p)^3(p^2+3pq+q^2).
$$

For the kink passing through zero, choose $\phi(0)=0$. Its profile is determined implicitly by

$$
\boxed{
\frac1{q^2-p^2}\left[\frac1p\operatorname{artanh}\frac{\phi}{p}-\frac1q\operatorname{artanh}\frac{\phi}{q}\right]=x
}.
$$

If $q=p$, the central equation becomes $\phi'=(p^2-\phi^2)^2$, so

$$
\boxed{
\frac{\phi}{2p^2(p^2-\phi^2)}+\frac1{2p^3}\operatorname{artanh}\frac\phi p=x
}.
$$

For $q=p+\varepsilon$,

$$
E_o=\frac23p^2\varepsilon^3+O(\varepsilon^4),
\qquad
E_c=\frac{16}{15}p^5+O(\varepsilon),
$$

so the leading ratio is

$$
\boxed{E_o:E_c:E_o=1:\frac85(p/\varepsilon)^3:1}.
$$

## 2

↑ **Parent:** [Paper 308](paper-308.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Away from a zero of $\phi$, the first [Bogomolny vortex equation](../../../classical-field-theory-soliton.md#bogomolny-vortex-equation) gives

$$
a_{\bar z}=-i\partial_{\bar z}\log\phi,
\qquad
f_{z\bar z}=-2i\partial_z\partial_{\bar z}\log|\phi|.
$$

Substitution into the second equation, with $\nabla^2=4\partial_z\partial_{\bar z}$, gives

$$
\boxed{-\frac2\Omega\nabla^2\log|\phi|=1-|\phi|^2}.
$$

Now set $\widetilde\Omega=\Omega|\phi|^2$. The [Gaussian curvature](../../../second-fundamental-form.md#gaussian-curvature) formula gives

$$
\widetilde K\widetilde\Omega=K\Omega-\nabla^2\log|\phi|.
$$

Therefore $(\widetilde K+1/2)\widetilde\Omega=(K+1/2)\Omega$ implies

$$
-\nabla^2\log|\phi|=\frac\Omega2(1-|\phi|^2),
$$

which is exactly the vortex equation.

The metric

$$
ds_n^2=\frac{8n^2|z|^{2n-2}}{(1-|z|^{2n})^2}dzd\bar z
$$

is the pullback of the $n=1$ [Poincare disc model](../../../geometry-and-topology.md#poincare-disk-model) metric under $w=z^n$. It consequently has $K=-1/2$ away from the origin. Comparing it with $ds_1^2$ gives the [Witten hyperbolic vortex](../../../classical-field-theory-soliton.md#witten-hyperbolic-vortex)

$$
\boxed{|\phi|=\frac{n|z|^{n-1}(1-|z|^2)}{1-|z|^{2n}}}.
$$

Putting $n=N+1$ gives winding number $N$. A gauge choice with positive radial factor is

$$
\phi=\frac{n z^N(1-|z|^2)}{1-|z|^{2n}},
$$

and then

$$
\boxed{
a_{\bar z}=i\left(\frac{z}{1-|z|^2}-\frac{nz|z|^{2n-2}}{1-|z|^{2n}}\right),
\qquad a_z=\overline{a_{\bar z}}.
}
$$

## 3

↑ **Parent:** [Paper 308](paper-308.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For coprime polynomials $p,q$, the algebraic degree of $R=p/q:S^2\to S^2$ is

$$
\deg R=\max(\deg p,\deg q),
$$

and its Wronskian is $W=p'q-pq'$. Thus

$$
R=z^2:\quad \deg R=2,\quad W=2z,
$$

while for

$$
R=\frac{\sqrt3iz^2-1}{z^3-\sqrt3iz}
$$

one obtains

$$
\boxed{\deg R=3,\qquad W=-\sqrt3iz^4+6z^2-\sqrt3i}.
$$

For $R=z^2$, a domain rotation $z\mapsto e^{i\alpha}z$ is accompanied by a target rotation $R\mapsto e^{2i\alpha}R$. There is also a half-turn about every axis in the equatorial plane, with the corresponding target half-turn. These generate the axial dihedral rotational symmetry: the distinguished spatial axis is the $z$-axis, and the continuous rotations about it are accompanied by twice the angle in target space.

The [rational map approximation for Skyrmions](../../../classical-field-theory-soliton.md#rational-map-approximation-for-skyrmions) uses

$$
U(r,z)=\exp\bigl(if(r)\,\widehat n_R(z)\cdot\boldsymbol\tau\bigr),
\qquad f(0)=\pi,\quad f(\infty)=0.
$$

The rational-map degree is the [Skyrmion](../../../classical-field-theory-soliton.md#skyrmion) baryon number, while zeros of the Wronskian identify directions where the angular baryon density vanishes and therefore influence the shape and energy. For $R=z^2$ the result is the $B=2$ toroidal Skyrmion.

Quantization treats spatial and isospin rotations as collective coordinates and imposes the [Finkelstein-Rubinstein constraints](../../../classical-field-theory-soliton.md#finkelstein-rubinstein-constraints). For even baryon number, spin and isospin are integral. The axial constraint is $2J_3+I_3=0$, and the equatorial half-turn imposes $(-1)^{J+I}=-1$. Restricting to $J,I\leq1$ leaves

$$
\boxed{(J,I)=(1,0)\quad\text{and}\quad(J,I)=(0,1)}.
$$

The $(0,0)$ and $(1,1)$ representations violate the discrete constraint.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
