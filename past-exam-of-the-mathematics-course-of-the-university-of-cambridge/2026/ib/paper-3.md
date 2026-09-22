# Paper 3

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2026/Paperib_3_2026.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2026/Paperib_3_2026.pdf)

**Table of contents**

- [1E](#1e)
  - [Solution](#1e/solution)
- [2F](#2f)
  - [Solution](#2f/solution)
- [3C](#3c)
  - [Solution](#3c/solution)
- [4B](#4b)
  - [Solution](#4b/solution)
- [5A](#5a)
  - [Solution](#5a/solution)
- [6B](#6b)
  - [Solution](#6b/solution)
- [7A](#7a)
  - [Solution](#7a/solution)
- [8H](#8h)
  - [Solution](#8h/solution)
- [9G](#9g)
  - [Solution](#9g/solution)
- [10E](#10e)
  - [Solution](#10e/solution)
- [11F](#11f)
  - [Solution](#11f/solution)
- [12F](#12f)
  - [Solution](#12f/solution)
- [13G](#13g)
  - [Solution](#13g/solution)
- [14A](#14a)
  - [Solution](#14a/solution)
- [15D](#15d)
  - [Solution](#15d/solution)
- [16A](#16a)
  - [Solution](#16a/solution)
- [17C](#17c)
  - [Solution](#17c/solution)
- [18H](#18h)
  - [Solution](#18h/solution)
- [19H](#19h)
  - [Solution](#19h/solution)

## 1E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="1e/solution">Solution</h3>

↑ **Parent:** [1E](#1e)

$A=\mathbb Z^2/\langle(6,9)\rangle$. The class of $(2,3)$ has order $3$, so $A$ has torsion and is not free. A unimodular change of [basis](../../../vector-space.md#basis) ([Smith normal form](../../../algebra.md#smith-normal-form), using $\gcd(6,9)=3$) gives $A\cong\mathbb Z\oplus\mathbb Z/3\mathbb Z$.

## 2F

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="2f/solution">Solution</h3>

↑ **Parent:** [2F](#2f)

The subspace opens are $A\cap U$; quotient opens are those whose inverse image is open; a homeomorphism is a continuous bijection with continuous inverse. Here $q(x,y)=(|x|,y)$ identifies exactly the required pairs and induces a homeomorphism $Y\to[0,1]\times[-1,1]$. An affine rescaling maps that rectangle homeomorphically onto $S$.

## 3C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="3c/solution">Solution</h3>

↑ **Parent:** [3C](#3c)

Integrate $(1+z^p)^{-1}$ around the wedge $0\le\arg z\le2\pi/p$. The radial [integrals](../../../calculus.md#integral) differ by the factor $e^{2\pi i/p}$, the arc vanishes, and the wedge contains the simple pole $e^{i\pi/p}$ with residue $-[p e^{-i\pi/p}]^{-1}$. Solving the resulting identity gives $I=(\pi/p)\csc(\pi/p)$.

## 4B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="4b/solution">Solution</h3>

↑ **Parent:** [4B](#4b)

For fixed boundary values, integration by parts gives $L_u-\partial_xL_{u_x}-\partial_yL_{u_y}=0$. For $L=u^2+u_xu_y$, this is $2u-2u_{xy}=0$, or $u_{xy}=u$, with the independently prescribed boundary data $u=xy$ on the circle.

## 5A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="5a/solution">Solution</h3>

↑ **Parent:** [5A](#5a)

Integration by parts gives $\tilde g_\sigma\prime(k)=-\sigma^2k\tilde g_\sigma(k)$ and $\tilde g_\sigma(0)=1$, so $\tilde g_\sigma=e^{-\sigma^2k^2/2}$. The convolution theorem says $\widetilde{f*g}=\tilde f\tilde g$; multiplying the two Gaussian transforms and inverting yields $g_{\sqrt{\sigma_1^2+\sigma_2^2}}$.

## 6B

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="6b/solution">Solution</h3>

↑ **Parent:** [6B](#6b)

$L_a=\varepsilon_{abc}x_bp_c$, with $[x_a,p_b]=i\hbar\delta_{ab}$ and position-position and momentum-momentum commutators zero. Expansion gives $[L_a,L_b]=i\hbar\varepsilon_{abc}L_c$ and $[L_a,p_d]=i\hbar\varepsilon_{adc}p_c$. Thus $[L_1,p_2]=i\hbar p_3\ne0$, so they are not simultaneously diagonalisable.

## 7A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="7a/solution">Solution</h3>

↑ **Parent:** [7A](#7a)

Unsteady Bernoulli gives the surface [pressure](../../../thermodynamics.md#pressure) from $p+\rho\partial_t\phi+\rho|\nabla\phi|^2/2=C(t)$. The velocity-squared contribution integrates to zero net force, while the unsteady term gives $F=-m_a\dot V$ with [added mass](../../../physics.md#added-mass) $m_a=\tfrac12(4\pi\rho a^3/3)=2\pi\rho a^3/3$. Hence $(m+m_a)a=G$, so $m^*=m+2\pi\rho a^3/3$: accelerating the bubble also accelerates surrounding fluid.

## 8H

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="8h/solution">Solution</h3>

↑ **Parent:** [8H](#8h)

The communicating classes are $\{1,2,3,6\}$ and $\{4,5\}$; only the latter is closed. Let $h_i=P_i(T_2\lt \infty)$, with $h_2=1$ and $h_4=h_5=0$. The first-step equations give $h_3=1/2$, $h_6=(h_1+h_3)/2$, and $h_1=1/3+h_3/3+h_6/6$, hence $h_1=13/22$.

## 9G

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="9g/solution">Solution</h3>

↑ **Parent:** [9G](#9g)

$V^*$ is the space of linear functionals and the dual [basis](../../../vector-space.md#basis) satisfies $v_i^*(v_j)=\delta_{ij}$. Nondegeneracy and equal finite dimensions make $u\mapsto\langle u,\cdot\rangle$ an isomorphism; evaluation similarly identifies $V$ with $V^{**}$. Riesz representation applied to $v\mapsto\langle Tv,u\rangle$ gives the unique adjoint. If $T$ is diagonalizable, declare an eigenbasis orthonormal to make it self-adjoint. Conversely, for self-adjoint $T$ and invariant $W$, $\langle Tv,w\rangle=\langle v,Tw\rangle=0$ shows $W^\perp$ invariant.

## 10E

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="10e/solution">Solution</h3>

↑ **Parent:** [10E](#10e)

Generators define a surjection $R^k\to M$, and conversely images of the standard [basis](../../../vector-space.md#basis) generate any quotient. Writing $\phi(m_i)=\sum_j a_{ij}m_j$ with $a_{ij}\in I$ and applying the adjugate to $XI-A$ gives a monic annihilating [polynomial](../../../polynomial.md) whose lower coefficients lie in $I$. Taking $\phi=1$ when $IM=M$ yields $xM=0$ with $x-1\in I$; for $M=\mathbb Z/3$ and $I=(2)$ take $x=3$. The Jacobson radical criterion follows by placing a nonunit $1-rs$ in a maximal [ideal](../../../commutative-algebra.md#ideal). It yields Nakayama’s lemma. Applying the [determinant](../../../linear-algebra.md#determinant) trick to preimages of a finite generating set constructs a [polynomial](../../../polynomial.md) right inverse to any surjective endomorphism, proving injectivity.

## 11F

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="11f/solution">Solution</h3>

↑ **Parent:** [11F](#11f)

A norm is positive definite, homogeneous, and subadditive; equivalence means mutual bounds by positive constants. Finite-dimensional norm equivalence gives corresponding constants for operator norms, whose $k$th roots tend to one, so $\rho(A)$ is norm-independent. If $\|A\|\lt 1$, Picard iteration gives $(I-A)^{-1}=\sum_{k\ge0}A^k$. If $\rho(A)\lt 1$, choose $\rho(A)\lt \alpha\lt 1$ and define $\|v\|_\alpha=\sup_{m\ge0}\alpha^{-m}\|A^mv\|$; it is finite, equivalent to the original norm, and $\|Av\|_\alpha\le\alpha\|v\|_\alpha$.

## 12F

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="12f/solution">Solution</h3>

↑ **Parent:** [12F](#12f)

A base covers the space and refines intersections. On $X^k$, products of opens form a base. The weighted metric satisfies the metric axioms and has exactly this topology; convergence is coordinatewise. For $X^{\mathbb N}$ the metric $d(f,g)=\sum_{n\ge1}2^{-n}\min\{1,\rho(f(n),g(n))\}$ induces the stated [product topology](../../../geometry-and-topology.md#product-topology): finitely many coordinates control a basic neighbourhood and the tail is uniformly small. Thus [sequences](../../../real-analysis.md#sequence) converge exactly coordinatewise.

## 13G

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="13g/solution">Solution</h3>

↑ **Parent:** [13G](#13g)

Expanding the [derivative](../../../calculus.md#derivative) [limit](../../../calculus.md#limit-of-a-function) along real and imaginary increments gives $u_x=v_y$ and $u_y=-v_x$. Since $\operatorname{Re}(ze^z)=e^x(x\cos y-y\sin y)$, the required [function](../../../function.md) is $f(z)=ze^z$, and $f(0)=0$. Two such [functions](../../../function.md) differ by a [holomorphic function](../../../complex-analysis.md#holomorphic-function) with zero real part; the open mapping theorem makes it constant, and the value at zero makes that constant zero.

## 14A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="14a/solution">Solution</h3>

↑ **Parent:** [14A](#14a)

Away from $x=y$ the Newton kernel is harmonic, while integrating its normal [derivative](../../../calculus.md#derivative) over a small sphere gives one, proving $\nabla^2\hat G=\delta$. Green’s second identity is $\int_V(u\nabla^2v-v\nabla^2u)=\int_{\partial V}(u\partial_nv-v\partial_nu)$. For the half-space, images give $G(x,y)=-(4\pi|x-y|)^{-1}+(4\pi|x-y^*|)^{-1}$. Substitution in the boundary formula yields the Poisson kernel $z/[2\pi((x_1-y_1)^2+(x_2-y_2)^2+z^2)^{3/2}]$; polar integration against the Gaussian gives exactly the stated one-dimensional [integral](../../../calculus.md#integral).

## 15D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="15d/solution">Solution</h3>

↑ **Parent:** [15D](#15d)

With $P^\mu=mU^\mu$, $U^\mu=dx^\mu/d\tau$, and $F^{\mu\nu}$ the field tensor, separating temporal and spatial components yields the [Lorentz force](../../../electromagnetism.md#lorentz-force) and power equations. The invariants are $E\cdot B$ and $E^2-c^2B^2$. For perpendicular fields with $E\lt cB$, boost with $v=E\times B/B^2$ (here $-E\hat y/B$); then $E\prime=0$ and $B\prime=\sqrt{B^2-E^2/c^2}\,\hat z$. Perpendicular motion is circular with $\omega=|q|B\prime/(\gamma m)$ and radius $p/(|q|B\prime)$. Transforming back adds the frame [velocity](../../../classical-mechanics.md#velocity), giving the nonrelativistic $E\times B/B^2$ drift, independent of $m,q$; a parallel [velocity](../../../classical-mechanics.md#velocity) would additionally produce a helix.

## 16A

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="16a/solution">Solution</h3>

↑ **Parent:** [16A](#16a)

[Momentum](../../../classical-mechanics.md#momentum) balance gives $\rho u_t=-p_x+\mu u_{yy}$. Steadiness forces $p_x=-G$ and no slip gives $u=Gy(H-y)/(2\mu)$, hence $Q=GH^3/(12\mu)$. After removal, separation gives

$$
u(y,t)=\sum_{\substack{n\ge1\\n\text{ odd}}}\frac{4GH^2}{\mu n^3\pi^3}\sin(n\pi y/H)\exp[-(\mu/\rho)(n\pi/H)^2t].
$$

## 17C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="17c/solution">Solution</h3>

↑ **Parent:** [17C](#17c)

Expanding the order condition about $w=1$ yields $\rho(w)=\sigma_s\sum_{l=1}^s w^{s-l}(w-1)^l/l$ and $\sigma_s=(\sum1/l)^{-1}$. Thus BDF2 has $\rho=w^2-4w/3+1/3$, $\sigma_2=2/3$, and BDF3 has $\rho=w^3-18w^2/11+9w/11-2/11$, $\sigma_3=6/11$. Their first characteristic [polynomials](../../../polynomial.md) satisfy the root condition, so consistency plus Dahlquist equivalence gives convergence. For BDF2 the stability boundary $z=\rho(e^{i\theta})/(\sigma_2e^{2i\theta})$ has nonnegative real part; hence the whole left half-plane is stable.

## 18H

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="18h/solution">Solution</h3>

↑ **Parent:** [18H](#18h)

Neyman–Pearson rejects for large $g(X)/f(X)$ and is most powerful at its size. For the normal sample, monotone likelihood ratio makes the UMP test reject when $\sqrt n\bar X\gt \Phi^{-1}(1-\alpha)$; its rejection probability increases in $\mu$, so it also has size $\alpha$ for the composite null $\mu\le0$. A likelihood-ratio test against a mixture null that has size $\alpha$ under each component bounds every competing test’s mixture power and is therefore UMP for the original two-point null. In the drug problem, the symmetric interval test has equal size $\alpha$ at $\mu=\pm\mu_0$ and no larger size farther out; it is the NP test against the equal mixture of those boundary laws, hence is UMP.

## 19H

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="19h/solution">Solution</h3>

↑ **Parent:** [19H](#19h)

[Gradient descent](../../../numerical-analysis.md#gradient-descent) is $x_{t+1}=x_t-\eta\nabla f(x_t)$. Integrating the Hessian along a segment gives the descent lemma. Applying it to the hinted $z$ and convexity yields cocoercivity: $(\nabla f(x)-\nabla f(y))^T(x-y)\ge\|\nabla f(x)-\nabla f(y)\|^2/\beta$. Apply this to $\phi=f-\alpha\|x\|^2/2$, whose Hessian lies between $0$ and $(\beta-\alpha)I$, and rearrange to obtain the displayed strengthened inequality. With $y=x^*$, $\nabla f(x^*)=0$, and $\eta=2/(\alpha+\beta)$, expansion of the squared update gives contraction factor $((\beta-\alpha)/(\beta+\alpha))^2$ per step and the stated bound.

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
