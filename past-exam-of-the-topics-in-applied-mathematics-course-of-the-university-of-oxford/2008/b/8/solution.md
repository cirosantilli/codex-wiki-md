<h1 id="b/8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

Let $S(x,y,z)=(-x,-y,z)$. In the first two components of the [vector field](../../../../vector-field.md), replacing $x,y$ by their negatives changes the sign of the whole component; in the third, the product $xy$ is unchanged. Thus $F(Sv)=SF(v)$, establishing the [symmetry](../../../../symmetry-physics.md), with solutions mapped to solutions by $S$.

At an [equilibrium point](../../../../equilibrium-point-of-a-dynamical-system.md), positivity of $a$ makes $y=x$. The remaining equations give $x(2c-a-z)=0$ and $z=x^2/b$. Hence

$$
\boxed{O=(0,0,0),\qquad P_\pm=(\pm\sqrt{b(2c-a)},\ \pm\sqrt{b(2c-a)},\ 2c-a),}
$$

where the two nonzero [equilibrium points](../../../../equilibrium-point-of-a-dynamical-system.md) exist when $0<a<2c$. They merge with the origin at $a_p=2c$, in a [pitchfork bifurcation](../../../../pitchfork-bifurcation-normal-form.md).

At the origin the [Jacobian matrix](../../../../jacobian-matrix.md) and its [eigenvalues](../../../../eigenvalue.md) are

$$
J_O=\begin{pmatrix}-a&a&0\\c-a&c&0\\0&0&-b\end{pmatrix},\qquad
\lambda_z=-b,\quad\lambda_\pm=\frac{c-a\pm\sqrt{c^2+6ac-3a^2}}2.
$$

At $a=2c$ these are $0,-c,-b$. To see the local [pitchfork bifurcation](../../../../pitchfork-bifurcation-normal-form.md) dynamics more explicitly put $\delta=2c-a$, $y=x+v$, and use $z=x^2/b+\cdots$ on the [center manifold](../../../../center-manifold.md). The equations become

$$
\dot x=av,\qquad \dot v=\delta x+(c-a)v-xz,\qquad
\dot z=x^2+xv-bz.
$$

At $\delta=0$, invariance at cubic order gives $v=-x^3/(bc)+\cdots$, hence the reduced equation is

$$
\dot x=2\delta x-\frac2b x^3+\text{higher-order terms}.
$$

It has the supercritical [pitchfork bifurcation](../../../../pitchfork-bifurcation-normal-form.md) form as $\delta$ increases, with the two branches $x\simeq\pm\sqrt{b\delta}$ [attracting](../../../../attraction-in-a-dynamical-system.md) near onset while the origin becomes [unstable](../../../../instability.md).

For $0<a<2c$, the [determinant](../../../../determinant.md) of the planar block is $a(a-2c)<0$, so the origin has one positive and two negative [eigenvalues](../../../../eigenvalue.md) and is a [saddle equilibrium](../../../../saddle-equilibrium.md). At $a=c$, the planar [eigenvalues](../../../../eigenvalue.md) are explicitly $\pm c$. For $a>2c$, the planar [trace](../../../../matrix-trace.md) $c-a$ is negative and its [determinant](../../../../determinant.md) positive, so the origin is [asymptotically stable](../../../../asymptotic-stability.md). To distinguish its type put

$$
a_*=c\left(1+\frac{2\sqrt3}{3}\right).
$$

For $2c<a<a_*$ both planar [eigenvalues](../../../../eigenvalue.md) are real negative, giving a [stable node](../../../../stable-node.md). At $a=a_*$ they coincide at $-c/\sqrt3$; the planar block is not a scalar [matrix](../../../../matrix.md), so it is a defective [stable node](../../../../stable-node.md). For $a>a_*$ they are [nonreal](../../../../nonreal-complex-number.md) with negative [real part](../../../../real-part.md), giving a [stable](../../../../lyapunov-stability.md) spiral in the planar block together with the [stable](../../../../lyapunov-stability.md) third direction. This refines the requested node-versus-saddle classification.

The origin cannot have a [Hopf bifurcation](../../../../hopf-bifurcation.md): a planar imaginary pair would require [trace](../../../../matrix-trace.md) zero, namely $a=c$, but the [determinant](../../../../determinant.md) there is $-c^2<0$, so the pair is real and of opposite signs.

For either nonzero [equilibrium point](../../../../equilibrium-point-of-a-dynamical-system.md) put $s=\pm\sqrt{b(2c-a)}$. The [Jacobian matrix](../../../../jacobian-matrix.md) is

$$
J_\pm=\begin{pmatrix}-a&a&0\\-c&c&-s\\s&s&-b\end{pmatrix}.
$$

Its [characteristic polynomial](../../../../characteristic-polynomial.md) is

$$
p(\lambda)=\lambda^3+A\lambda^2+B\lambda+C,\qquad
A=a+b-c,\quad B=bc,\quad C=2ab(2c-a).
$$

A nonzero imaginary [root of an equation](../../../../root-of-an-equation.md) $i\omega$ requires, by separating real and imaginary parts, $\omega^2=B$ and $AB=C$. Equivalently

$$
2a^2-3ac+bc-c^2=0,
$$

so the candidate [Hopf bifurcation](../../../../hopf-bifurcation.md) values are

$$
\boxed{a_h=\frac{3c\pm\sqrt{17c^2-8bc}}4.}
$$

At such an admissible value the factorization is $p(\lambda)=(\lambda+A)(\lambda^2+bc)$, giving the pair $\pm i\sqrt{bc}$ and a negative third [eigenvalue](../../../../eigenvalue.md) $-A$, since $A=C/B>0$ on the nonzero branches.

The [mathematical model parameter](../../../../mathematical-model-parameter.md) restrictions matter. A real candidate requires $b/c\le17/8$, and the nonzero [equilibrium points](../../../../equilibrium-point-of-a-dynamical-system.md) also require $0<a_h<2c$. The upper-sign value is admissible for $0<b/c<17/8$; the lower-sign value additionally requires $b/c>1$. For fixed $b,c$, [differentiation](../../../../differentiation.md) of the characteristic equation at the imaginary [root of an equation](../../../../root-of-an-equation.md) gives the [eigenvalue crossing speed](../../../../eigenvalue-crossing-speed.md)

$$
\left.\frac{d\operatorname{Re}\lambda}{da}\right|_{a_h}
=-\frac{b(4a_h-3c)}{2\{bc+(a_h+b-c)^2\}}.
$$

Thus the [transverse eigenvalue crossing](../../../../transverse-eigenvalue-crossing.md) condition holds except at the coincident-root case $b/c=17/8$, $a_h=3c/4$. At a [transverse eigenvalue crossing](../../../../transverse-eigenvalue-crossing.md), a generic nonzero [first Lyapunov coefficient](../../../../first-lyapunov-coefficient.md) gives a [Hopf bifurcation](../../../../hopf-bifurcation.md). The displayed radical is the spectral threshold; it does not justify an unconditional generic-Hopf claim for all positive [mathematical model parameters](../../../../mathematical-model-parameter.md), nor does it by itself exclude a degenerate [Hopf bifurcation](../../../../hopf-bifurcation.md) point. For example $b>17c/8$ yields no real candidate at all. The cubic [Routh-Hurwitz stability criterion](../../../../routh-hurwitz-stability-criterion.md) gives local [Lyapunov stability](../../../../lyapunov-stability.md) on the side with $A>0$ and $AB-C>0$, where

$$
AB-C=b(2a^2-3ac+bc-c^2).
$$

For the modified equation, the planar block at the origin is $\begin{pmatrix}-a&a\\c&c\end{pmatrix}$, with [determinant](../../../../determinant.md) $-2ac<0$ for the stipulated positive [mathematical model parameters](../../../../mathematical-model-parameter.md). Thus the origin is always a [saddle equilibrium](../../../../saddle-equilibrium.md) for nonzero $a,c$ in that [mathematical model parameter](../../../../mathematical-model-parameter.md) range. The nonzero [equilibrium points](../../../../equilibrium-point-of-a-dynamical-system.md) now satisfy $y=x$, $z=2c$ and $x^2=2bc$, so they are

$$
(\pm\sqrt{2bc},\ \pm\sqrt{2bc},\ 2c).
$$

For $b,c>0$ these branches stay a positive distance from the origin and do not merge with it as $a$ varies. The origin also has no zero [eigenvalue](../../../../eigenvalue.md) for $a,c>0$. Therefore **the [pitchfork bifurcation](../../../../pitchfork-bifurcation-normal-form.md) is absent in the modified system**.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../split.md)
5. [Topics in applied mathematics course of the University of Oxford](../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
