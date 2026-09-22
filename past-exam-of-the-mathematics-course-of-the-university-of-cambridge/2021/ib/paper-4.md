# Paper 4

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2021/paperib_4_2021.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2021/paperib_4_2021.pdf)

**Table of contents**

- [1E](#1e)
  - [i](#1e/i)
    - [Solution](#1e/i/solution)
  - [ii](#1e/ii)
    - [Solution](#1e/ii/solution)
- [2F](#2f)
  - [a](#2f/a)
    - [Solution](#2f/a/solution)
  - [b](#2f/b)
    - [Solution](#2f/b/solution)
  - [c](#2f/c)
    - [Solution](#2f/c/solution)
- [3G](#3g)
  - [Solution](#3g/solution)
- [4C](#4c)
  - [Solution](#4c/solution)
- [5D](#5d)
  - [Solution](#5d/solution)
- [6B](#6b)
  - [a](#6b/a)
    - [Solution](#6b/a/solution)
  - [b](#6b/b)
    - [Solution](#6b/b/solution)
- [7H](#7h)
  - [Solution](#7h/solution)
- [8E](#8e)
  - [a](#8e/a)
    - [Solution](#8e/a/solution)
  - [b](#8e/b)
    - [Solution](#8e/b/solution)
  - [c](#8e/c)
    - [Solution](#8e/c/solution)
- [9G](#9g)
  - [Solution](#9g/solution)
- [10F](#10f)
  - [a](#10f/a)
    - [Solution](#10f/a/solution)
  - [b](#10f/b)
    - [Solution](#10f/b/solution)
- [11F](#11f)
  - [Solution](#11f/solution)
- [12B](#12b)
  - [Solution](#12b/solution)
- [13D](#13d)
  - [a](#13d/a)
    - [Solution](#13d/a/solution)
  - [b](#13d/b)
    - [Solution](#13d/b/solution)
  - [c](#13d/c)
    - [Solution](#13d/c/solution)
- [14C](#14c)
  - [Solution](#14c/solution)
- [15C](#15c)
  - [a](#15c/a)
    - [Solution](#15c/a/solution)
  - [b](#15c/b)
    - [Solution](#15c/b/solution)
- [16A](#16a)
  - [a](#16a/a)
    - [Solution](#16a/a/solution)
  - [b](#16a/b)
    - [Solution](#16a/b/solution)
  - [c](#16a/c)
    - [Solution](#16a/c/solution)
  - [d](#16a/d)
    - [Solution](#16a/d/solution)
- [17H](#17h)
  - [a](#17h/a)
    - [Solution](#17h/a/solution)
  - [b](#17h/b)
    - [Solution](#17h/b/solution)
  - [c](#17h/c)
    - [Solution](#17h/c/solution)
  - [d](#17h/d)
    - [Solution](#17h/d/solution)
  - [e](#17h/e)
    - [Solution](#17h/e/solution)
  - [f](#17h/f)
    - [Solution](#17h/f/solution)
- [18H](#18h)
  - [a](#18h/a)
    - [Solution](#18h/a/solution)
  - [b](#18h/b)
    - [Solution](#18h/b/solution)
  - [c](#18h/c)
    - [i](#18h/c/i)
      - [Solution](#18h/c/i/solution)
    - [ii](#18h/c/ii)
      - [Solution](#18h/c/ii/solution)
    - [iii](#18h/c/iii)
      - [Solution](#18h/c/iii/solution)

## 1E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1e/i">i</h3>

↑ **Parent:** [1E](#1e)

<h4 id="1e/i/solution">Solution</h4>

↑ **Parent:** [I](#1e/i)

Let $E_{rs}$ be the [matrix unit](../../../vector-space.md#matrix-unit) with its only nonzero entry in row $r$, column $s$. For

$$
A=\operatorname{diag}(1,2,\ldots,n),
$$

one has

$$
AE_{rs}=rE_{rs},
\qquad
E_{rs}A=sE_{rs}.
$$

Therefore

$$
\boxed{\phi_A(E_{rs})=(r-s)E_{rs}}.
$$

The $n^2$ matrix units form an [eigenbasis](../../../linear-operator-theory.md#eigenbasis), with $E_{rs}$ having eigenvalue $r-s$. The zero eigenspace consists exactly of the diagonal matrices and has dimension $n$. The [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem) now gives

$$
\boxed{\operatorname{rank}\phi_A=n^2-n}.
$$

<h3 id="1e/ii">ii</h3>

↑ **Parent:** [1E](#1e)

<h4 id="1e/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1e/ii)

For

$$
X=\begin{pmatrix}a&b\\c&d\end{pmatrix},
$$

direct multiplication gives

$$
\phi_A(X)=AX-XA
=\begin{pmatrix}c&d-a\\0&-c\end{pmatrix}.
$$

With respect to the ordered standard basis $(E_{11},E_{12},E_{21},E_{22})$, its matrix is therefore

$$
\boxed{
[\phi_A]=
\begin{pmatrix}
0&0&1&0\\
-1&0&0&1\\
0&0&0&0\\
0&0&-1&0
\end{pmatrix}
}.
$$

This [nilpotent operator](../../../linear-operator-theory.md#nilpotent-linear-map) satisfies $\phi_A^3=0$, while $\phi_A^2\ne0$. Moreover,

$$
\operatorname{rank}\phi_A=2,
\qquad
\operatorname{rank}\phi_A^2=1.
$$

These ranks determine one nilpotent block of size three and one of size one. Hence its [Jordan normal form](../../../linear-operator-theory.md#jordan-normal-form) is

$$
\boxed{J_3(0)\oplus J_1(0)}.
$$

## 2F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2f/a">a</h3>

↑ **Parent:** [2F](#2f)

<h4 id="2f/a/solution">Solution</h4>

↑ **Parent:** [A](#2f/a)

The [quotient topology](../../../topology.md#quotient-topology) on $\widetilde X$ is

$$
\mathcal T_{\widetilde X}
=\{U\subseteq\widetilde X:\pi^{-1}(U)\text{ is open in }X\}.
$$

Since inverse images preserve arbitrary unions and finite intersections,

$$
\pi^{-1}\!\left(\bigcup_\alpha U_\alpha\right)
=\bigcup_\alpha\pi^{-1}(U_\alpha),
\qquad
\pi^{-1}(U\cap V)=\pi^{-1}(U)\cap\pi^{-1}(V).
$$

Also $\pi^{-1}(\varnothing)=\varnothing$ and $\pi^{-1}(\widetilde X)=X$. The displayed collection therefore satisfies all the [topology axioms](../../../topology.md#topology-axiom).

<h3 id="2f/b">b</h3>

↑ **Parent:** [2F](#2f)

<h4 id="2f/b/solution">Solution</h4>

↑ **Parent:** [B](#2f/b)

If $f:\widetilde X\to Y$ is continuous, then $f\circ\pi$ is continuous because the quotient map $\pi$ is continuous by definition.

Conversely, suppose $f\circ\pi$ is continuous. For every open set $V\subseteq Y$,

$$
\pi^{-1}(f^{-1}(V))
=(f\circ\pi)^{-1}(V)
$$

is open in $X$. The definition of the quotient topology then says that $f^{-1}(V)$ is open in $\widetilde X$. Hence

$$
\boxed{f\text{ is continuous}\iff f\circ\pi\text{ is continuous}}.
$$

This is the [universal property of the quotient topology](../../../topology.md#universal-property-of-the-quotient-topology).

<h3 id="2f/c">c</h3>

↑ **Parent:** [2F](#2f)

<h4 id="2f/c/solution">Solution</h4>

↑ **Parent:** [C](#2f/c)

**No.** Take the [Hausdorff space](../../../topology.md#hausdorff-space) $X=\mathbb R$ and declare all nonzero points equivalent, leaving $0$ in its own class. The quotient has two points,

$$
\{[0],[\mathbb R\setminus\{0\}]\}.
$$

The nonzero class is open because its inverse image $\mathbb R\setminus\{0\}$ is open. However, the only saturated set containing $0$ but not the other class is $\{0\}$, which is not open. Thus every neighbourhood of $[0]$ is the whole quotient, so the two quotient points cannot have disjoint neighbourhoods. Therefore $\widetilde X$ need not be Hausdorff.

## 3G

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3g/solution">Solution</h3>

↑ **Parent:** [3G](#3g)

The hypothesis says that $f$ has a zero of [order](../../../complex-analysis.md#order-of-a-zero-of-a-holomorphic-function) $k$ at $a$, so write

$$
f(z)=(z-a)^kg(z),
\qquad
g(a)\ne0,
$$

with $g$ holomorphic near $a$. Differentiating gives

$$
f'(z)=(z-a)^{k-1}\bigl(kg(z)+(z-a)g'(z)\bigr).
$$

Choose $\delta>0$ so small that the closed disc $\overline D(a,\delta)$ lies in the domain, $g$ never vanishes there, and the parenthesized factor never vanishes there. Thus $a$ is the only critical point of $f$ in that disc.

On the boundary circle, $f$ is nonzero. Set

$$
\varepsilon=\min_{|z-a|=\delta}|f(z)|>0.
$$

If $0<|b|<\varepsilon$, then $|b|<|f(z)|$ on the boundary. [Rouché's theorem](../../../complex-analysis.md#rouche-s-theorem) applied to $f$ and $f-b$ says that $f-b$ has the same number of zeros in $D(a,\delta)$ as $f$, namely $k$, counted with multiplicity.

None of these zeros is $a$ because $b\ne0$, and none is a critical point because $f'$ has no other zero in the disc. Every zero of $f-b$ is therefore simple. Hence there are exactly

$$
\boxed{k\text{ distinct }z\in D(a,\delta)\text{ with }f(z)=b}.
$$

## 4C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4c/solution">Solution</h3>

↑ **Parent:** [4C](#4c)

The one-dimensional [Time-dependent Schrödinger equation](../../../physics.md#time-dependent-schrodinger-equation) for a [wavefunction](../../../quantum-mechanics.md#wave-function) in a real potential is

$$
i\hbar\frac{\partial\Psi}{\partial t}
=-\frac{\hbar^2}{2m}\frac{\partial^2\Psi}{\partial x^2}+U\Psi.
$$

Multiplying this equation by $\Psi^*$, multiplying its [complex conjugate](../../../complex-analysis.md#complex-conjugate) by $\Psi$, and subtracting gives the [probability continuity equation](../../../quantum-mechanics.md#probability-continuity-equation)

$$
\frac{\partial |\Psi|^2}{\partial t}+\frac{\partial j}{\partial x}=0,
\qquad
j=\frac{\hbar}{2mi}\left(\Psi^*\frac{\partial\Psi}{\partial x}
-\Psi\frac{\partial\Psi^*}{\partial x}\right).
$$

If $\Psi$ and its first [derivative](../../../calculus.md#derivative) decay sufficiently rapidly as $x\to\pm\infty$, then the [probability current](../../../quantum-mechanics.md#probability-current) $j$ vanishes at both ends. Integrating the continuity equation and using the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) yields

$$
\frac d{dt}\int_{-\infty}^{\infty}|\Psi(x,t)|^2\,dx
=-j(\infty,t)+j(-\infty,t)=0.
$$

This [conservation of quantum probability](../../../quantum-mechanics.md#conservation-of-quantum-probability) is required by the [Born rule](../../../quantum-mechanics.md#born-rule): once a [normalizable wavefunction](../../../quantum-mechanics.md#normalizable-wavefunction) has total probability one, its time evolution must preserve that normalization.

For the stated [Gaussian wave packet](../../../quantum-mechanics.md#gaussian-wave-packet), put $\beta=\hbar t/m$. Since

$$
f(t)=\frac1{\alpha+i\beta},
\qquad
|f(t)|=\frac1{\sqrt{\alpha^2+\beta^2}},
\qquad
\operatorname{Re}f(t)=\frac{\alpha}{\alpha^2+\beta^2},
$$

its squared [modulus](../../../complex-analysis.md#modulus) is

$$
|\Psi(x,t)|^2
=\frac{C^2}{\sqrt{\alpha^2+\beta^2}}
\exp\left(-\frac{\alpha x^2}{\alpha^2+\beta^2}\right).
$$

The [Gaussian integral](../../../calculus.md#gaussian-integral) then gives

$$
\int_{-\infty}^{\infty}|\Psi(x,t)|^2\,dx
=\frac{C^2}{\sqrt{\alpha^2+\beta^2}}
\sqrt{\frac{\pi(\alpha^2+\beta^2)}{\alpha}}
=\boxed{C^2\sqrt{\frac\pi\alpha}},
$$

which is independent of time, as required.

## 5D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5d/solution">Solution</h3>

↑ **Parent:** [5D](#5d)

In a vacuum with no charge or current, the [Maxwell equations](../../../electromagnetism.md#maxwell-equations) are

$$
\nabla\cdot E=0,
\qquad
\nabla\cdot B=0,
\qquad
\nabla\times E=-\frac{\partial B}{\partial t},
\qquad
\nabla\times B=\frac1{c^2}\frac{\partial E}{\partial t}.
$$

For the proposed [plane electromagnetic wave](../../../electromagnetism.md#plane-electromagnetic-wave), $\nabla\cdot B=0$ gives

$$
k\cdot B_0=0.
$$

The [Ampère-Maxwell equation](../../../electromagnetism.md#ampere-s-circuital-law) gives

$$
E_0=-\frac{c^2}{\omega}\,k\times B_0,
$$

and substituting this into [Faraday's law](../../../electromagnetism.md#faraday-s-law-of-induction) gives the [dispersion relation](../../../wave-equation.md#dispersion-relation)

$$
\omega^2=c^2|k|^2.
$$

Thus both fields have [transverse polarization](../../../wave-equation.md#transverse-polarization) relative to $k$, and the corresponding real electric field is

$$
\boxed{E(x,t)=\operatorname{Re}\left[-\frac{c^2}{\omega}
(k\times B_0)e^{i(k\cdot x-\omega t)}\right]}.
$$

For incidence in the positive $x$-direction, choose the incident fields

$$
B_i=B_0\cos(kx-\omega t)e_z,
\qquad
E_i=cB_0\cos(kx-\omega t)e_y.
$$

The [perfect conductor](../../../electromagnetism.md#perfect-conductor) requires the tangential electric field to vanish at $x=0$. The reflected wave therefore has

$$
B_r=B_0\cos(kx+\omega t)e_z,
\qquad
E_r=-cB_0\cos(kx+\omega t)e_y.
$$

This is [normal reflection of an electromagnetic wave from a perfect conductor](../../../electromagnetism.md#normal-reflection-of-an-electromagnetic-wave-from-a-perfect-conductor). The magnetic field in $x\leq0$ is

$$
B=B_i+B_r
=2B_0\cos(kx)\cos(\omega t)e_z,
$$

so its tangential value at the surface is

$$
\boxed{B_{\rm tangential}(0,t)=2B_0\cos(\omega t)e_z}.
$$

## 6B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="6b/a">a</h3>

↑ **Parent:** [6B](#6b)

<h4 id="6b/a/solution">Solution</h4>

↑ **Parent:** [A](#6b/a)

Use the nodes in the order $0,1,2,3$. Their first [divided differences](../../../numerical-analysis.md#divided-difference) are $4,-2,6$, their second divided differences are $-3,4$, and their third divided difference is $7/3$. The [Newton interpolation polynomial](../../../numerical-analysis.md#newton-polynomial) is therefore

$$
\boxed{
p_3(x)=4x-3x(x-1)+\frac73x(x-1)(x-2)
}.
$$

This is the unique [interpolating polynomial](../../../numerical-analysis.md#polynomial-interpolation) of degree at most three through the four data points.

<h3 id="6b/b">b</h3>

↑ **Parent:** [6B](#6b)

<h4 id="6b/b/solution">Solution</h4>

↑ **Parent:** [B](#6b/b)

Appending the node $-2$ to the existing [Newton interpolation polynomial](../../../numerical-analysis.md#newton-polynomial) gives

$$
p_4(x)=p_3(x)+a_4x(x-1)(x-2)(x-3).
$$

At the new node,

$$
p_3(-2)=-82,
\qquad
(-2)(-3)(-4)(-5)=120.
$$

The condition $p_4(-2)=10$ therefore gives

$$
a_4=\frac{10-(-82)}{120}=\frac{23}{30}.
$$

Hence

$$
\boxed{
p_4(x)=4x-3x(x-1)+\frac73x(x-1)(x-2)
+\frac{23}{30}x(x-1)(x-2)(x-3)
}.
$$

## 7H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="7h/solution">Solution</h3>

↑ **Parent:** [7H](#7h)

For the [simple random walk on the integer line](../../../markov-process.md#simple-random-walk-on-the-integer-line), a return to the origin is possible only at an [even](../../../number-theory.md#even-number) time. At time $2n$, exactly $n$ of the increments must be $+1$, so the return probability is

$$
p_{2n}=\frac1{2^{2n}}\binom{2n}{n}.
$$

The supplied factorial bounds, equivalently the order estimate in the [Stirling formula](../../../real-analysis.md#stirling-formula), give

$$
p_{2n}\asymp n^{-1/2}.
$$

Consequently $\sum_np_{2n}$ diverges. By the [recurrence criterion by return probabilities](../../../markov-process.md#recurrence-criterion-by-return-probabilities), the origin is a [recurrent state](../../../markov-process.md#recurrent-state); translation invariance then makes the whole walk recurrent.

For three [independent](../../../random-variable.md#independent-random-variables) walks, the probability that all three are at the origin at time $2n$ is

$$
p_{2n}^3
=\left(\frac{\binom{2n}{n}}{4^n}\right)^3
\asymp n^{-3/2}.
$$

This [P-series](../../../real-analysis.md#p-series) is convergent, so the first of the [Borel-Cantelli lemmas](../../../probability-theory.md#borel-cantelli-lemmas) says that simultaneous returns occur only finitely often with probability one. Therefore the requested probability is

$$
\boxed{0}.
$$

## 8E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="8e/a">a</h3>

↑ **Parent:** [8E](#8e)

<h4 id="8e/a/solution">Solution</h4>

↑ **Parent:** [A](#8e/a)

A [Hermitian form](../../../linear-algebra.md#hermitian-form) is a [sesquilinear form](../../../linear-algebra.md#sesquilinear-form) $H:V\times V\to\mathbb C$ such that

$$
H(v,w)=\overline{H(w,v)}.
$$

Use the convention that $H$ is linear in its first argument and conjugate-linear in its second. Its [matrix](../../../linear-algebra.md#matrix-of-a-hermitian-form) in the basis $(v_1,\ldots,v_n)$ is

$$
A_{ij}=H(v_i,v_j).
$$

If $v=\sum_i x_iv_i$ and $w=\sum_jy_jv_j$, then

$$
H(v,w)=x^TA\overline y.
$$

Since $w_i=\sum_jp_{ij}v_j$, the coordinate row of each new basis vector is a row of $P$. Direct substitution gives

$$
H(w_i,w_k)=\sum_{j,l}p_{ij}A_{jl}\overline{p_{kl}},
$$

so the new matrix is

$$
\boxed{P A\overline P^{\,T}}.
$$

The subspace $N=V^\perp$ is the [radical](../../../linear-algebra.md#radical-of-a-bilinear-form) of $H$. In coordinates it is the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) of $A$, and the [rank-nullity theorem](../../../linear-algebra.md#rank-nullity-theorem) gives

$$
\boxed{\dim N=n-\operatorname{rank}A}.
$$

<h3 id="8e/b">b</h3>

↑ **Parent:** [8E](#8e)

<h4 id="8e/b/solution">Solution</h4>

↑ **Parent:** [B](#8e/b)

The [symmetric matrix](../../../linear-algebra.md#symmetric-matrix) of the [quadratic form](../../../linear-algebra.md#quadratic-form) in the standard basis is

$$
A=\begin{pmatrix}
1&1&1\\
1&1&-1\\
1&-1&2
\end{pmatrix},
$$

because the off-diagonal entries contribute twice to $x^TAx$.

Apply [Gram-Schmidt orthogonalization for a symmetric bilinear form](../../../linear-algebra.md#gram-schmidt-orthogonalization-for-a-symmetric-bilinear-form) to

$$
u_1=e_1,
\qquad
u_2=e_3-e_1,
\qquad
u_3=e_2-e_1+2u_2=-3e_1+e_2+2e_3.
$$

These vectors are pairwise orthogonal for $B(u,v)=u^TAv$, and

$$
B(u_1,u_1)=1,
\qquad
B(u_2,u_2)=1,
\qquad
B(u_3,u_3)=-4.
$$

Thus the form is diagonal in the basis $(u_1,u_2,u_3)$, with matrix

$$
\operatorname{diag}(1,1,-4).
$$

It follows that its [rank](../../../linear-algebra.md#rank-of-a-quadratic-form) is $3$ and its [signature](../../../linear-algebra.md#signature-of-a-quadratic-form) is

$$
\boxed{2-1=1}.
$$

<h3 id="8e/c">c</h3>

↑ **Parent:** [8E](#8e)

<h4 id="8e/c/solution">Solution</h4>

↑ **Parent:** [C](#8e/c)

By the [real spectral theorem](../../../linear-operator-theory.md#real-spectral-theorem), the real [symmetric matrix](../../../linear-algebra.md#symmetric-matrix) $A$ has an orthonormal basis of [eigenvectors](../../../linear-operator-theory.md#eigenvector). In that basis the associated [quadratic form](../../../linear-algebra.md#quadratic-form) is

$$
q(x)=\lambda_1x_1^2+\cdots+\lambda_nx_n^2.
$$

Rescaling the coordinates belonging to nonzero [eigenvalues](../../../linear-operator-theory.md#eigenvalue) changes every positive coefficient to $+1$ and every negative coefficient to $-1$. Hence the diagonal normal form has one positive square for each positive eigenvalue and one negative square for each negative eigenvalue. By [Sylvester's law of inertia](../../../linear-algebra.md#sylvester-s-law-of-inertia), these counts do not depend on the diagonalizing basis, so

$$
\boxed{\operatorname{signature}H
=\#\{\lambda_i>0\}-\#\{\lambda_i<0\}}.
$$

The numerical eigenvalues are not invariant under a general [change of basis](../../../linear-algebra.md#change-of-basis), because the matrix changes by congruence rather than similarity. For example, on a one-dimensional space let $q(e)=1$. Its matrix in the basis $(e)$ is $(1)$, whereas in the basis $(2e)$ it is $(4)$. The eigenvalue changes from $1$ to $4$, although its sign, and therefore the signature, is unchanged.

## 9G

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="9g/solution">Solution</h3>

↑ **Parent:** [9G](#9g)

For subgroups $H,P\leq G$, define $x\sim y$ when $y\in HxP$. The identity elements show reflexivity, inverses show symmetry, and multiplication shows transitivity. Thus the [double cosets](../../../group-theory.md#double-coset) $HxP$ partition $G$.

Let $H$ act by left multiplication on the set of left [cosets](../../../group-theory.md#coset) $G/P$. The orbit of $xP$ consists of the cosets contained in $HxP$, so its size is $|HxP|/|P|$. Its stabilizer is

$$
\begin{aligned}
\operatorname{Stab}_H(xP)
&=\{h\in H:hxP=xP\}\\
&=H\cap xPx^{-1}.
\end{aligned}
$$

The [orbit-stabilizer theorem](../../../group-theory.md#orbit-stabilizer-theorem) therefore gives

$$
\boxed{\frac{|HxP|}{|P|}
=\frac{|H|}{|H\cap xPx^{-1}|}}.
$$

Suppose $P$ is a [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) of $G$, with $|P|=p^a$, and write the largest power of $p$ dividing $|H|$ as $p^b$. If every $H\cap xPx^{-1}$ had order at most $p^{b-1}$, the displayed formula would make every double-coset size divisible by $p^{a+1}$. Their sum $|G|$ would then also be divisible by $p^{a+1}$, contradicting the choice of $P$. Hence some $H\cap xPx^{-1}$ has order $p^b$ and is a Sylow $p$-subgroup of $H$. This is the [Sylow subgroup of a subgroup from double cosets](../../../group-theory.md#sylow-subgroup-of-a-subgroup-from-double-cosets) argument.

To count the [general linear group over a finite field](../../../finite-group-theory.md#general-linear-group-over-a-finite-field) $GL_n(\mathbb F_p)$, choose its columns successively. There are $p^n-1$ choices for the first, $p^n-p$ for the second, and $p^n-p^k$ for column $k+1$. Consequently

$$
\boxed{|GL_n(\mathbb F_p)|
=\prod_{k=0}^{n-1}(p^n-p^k)
=p^{n(n-1)/2}\prod_{j=1}^n(p^j-1)}.
$$

None of the factors $p^j-1$ is divisible by $p$, so the [upper unitriangular group](../../../finite-group-theory.md#upper-unitriangular-group) is a Sylow $p$-subgroup: it has one arbitrary field entry in each of the $n(n-1)/2$ positions above the diagonal and hence order $p^{n(n-1)/2}$. The [permutation matrices](../../../vector-space.md#permutation-matrix) form a subgroup isomorphic to the [symmetric group](../../../finite-group-theory.md#symmetric-group) $S_n$.

By [Cayley theorem](../../../group-theory.md#cayley-s-theorem), every finite group $G$ embeds in $S_{|G|}$, and permutation matrices embed this symmetric group in $GL_{|G|}(\mathbb F_p)$. The latter has the explicit Sylow $p$-subgroup just described, so the result proved in the first part, applied to the embedded copy of $G$, proves that every finite group has a Sylow $p$-subgroup.

The counting part of the [Sylow theorems](../../../finite-group-theory.md#sylow-theorems) says that if $p^a$ is the largest power of $p$ dividing $|G|$, then the number $n_p$ of Sylow $p$-subgroups satisfies

$$
\boxed{n_p\equiv1\pmod p,\qquad n_p\mid |G|/p^a}.
$$

Finally, let $|G|=pq$ with prime numbers $p>q$. The Sylow counts give

$$
n_p\mid q,\quad n_p\equiv1\pmod p,
$$

so $n_p=1$ and the Sylow $p$-subgroup is a [normal subgroup](../../../group-theory.md#normal-subgroup). Also $n_q\mid p$ and $n_q\equiv1\pmod q$. If $n_q=1$, both Sylow subgroups are normal; their elements commute, so $G$ is their [direct product](../../../group-theory.md#direct-product-of-groups) and is [abelian](../../../group.md#abelian-group). In the nonabelian case one must therefore have $n_q=p$, whence

$$
\boxed{p\equiv1\pmod q},
$$

or equivalently $q\mid p-1$, as recorded by [nonabelian group of order pq](../../../finite-group-theory.md#nonabelian-group-of-order-pq).

## 10F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="10f/a">a</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/a/solution">Solution</h4>

↑ **Parent:** [A](#10f/a)

Fix $x\in\mathbb R^n$ and a coordinate direction $e_i$. The [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) gives

$$
\frac{g(t,x+he_i)-g(t,x)}h
=\int_0^1D_i g(t,x+she_i)\,ds.
$$

For sufficiently small $h$, the points $(t,x+she_i)$ lie in a fixed compact set. The continuity of $D_i g$ makes it [uniformly continuous](../../../topological-analysis.md#uniform-continuity) there, so the right-hand side converges to $D_i g(t,x)$ uniformly in $t$. We may consequently pass the limit through the finite [integral](../../../calculus.md#integral):

$$
\begin{aligned}
D_iG(x)
&=\lim_{h\to0}\int_0^1
\frac{g(t,x+he_i)-g(t,x)}h\,dt\\
&=\boxed{\int_0^1D_i g(t,x)\,dt}.
\end{aligned}
$$

To prove continuity, if $x_k\to x$, joint continuity makes $D_i g(t,x_k)\to D_i g(t,x)$ uniformly for $t\in[0,1]$ once the $x_k$ lie in a compact neighbourhood of $x$. Hence $D_iG(x_k)\to D_iG(x)$. This proves the stated [differentiation under the integral sign](../../../analysis.md#differentiation-under-the-integral-sign) result and the continuity of every partial derivative.

<h3 id="10f/b">b</h3>

↑ **Parent:** [10F](#10f)

<h4 id="10f/b/solution">Solution</h4>

↑ **Parent:** [B](#10f/b)

For fixed $(x_1,x_2)$, apply the given one-variable identity to the [smooth function](../../../analysis.md#smooth-function)

$$
u(t)=f(x_1,tx_2).
$$

The [chain rule](../../../calculus.md#chain-rule) gives

$$
u'(0)=x_2D_2f(x_1,0),
\qquad
u''(t)=x_2^2D_2^2f(x_1,tx_2).
$$

Therefore

$$
f(x_1,x_2)
=f(x_1,0)+x_2D_2f(x_1,0)+x_2^2h(x_1,x_2),
$$

where

$$
\boxed{
h(x_1,x_2)
=\int_0^1(1-t)D_2^2f(x_1,tx_2)\,dt
}.
$$

Every derivative of the integrand is continuous. Repeated [differentiation under the integral sign](../../../analysis.md#differentiation-under-the-integral-sign) therefore shows that $h$ is smooth. This is the [Second-order Hadamard lemma](../../../analysis.md#second-order-hadamard-lemma).

## 11F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="11f/solution">Solution</h3>

↑ **Parent:** [11F](#11f)

An [abstract smooth surface](../../../differential-geometry.md#abstract-smooth-surface) is a Hausdorff second-countable topological space with an atlas of [charts](../../../differential-geometry.md#manifold-chart) to open subsets of $\mathbb R^2$ whose transition maps are smooth. It is [orientable](../../../differential-geometry.md#orientable-smooth-manifold) when it has such an atlas for which every transition map has positive [Jacobian determinant](../../../calculus.md#jacobian-determinant). A map $f:S_1\to S_2$ is a [smooth map](../../../differential-geometry.md#smooth-map-between-manifolds) when every coordinate representation

$$
\psi\circ f\circ\phi^{-1}
$$

is smooth wherever it is defined.

The map $a:C\to C$ is a smooth involution with no fixed point: the equation

$$
(x,y,z)=(-x,-y,-z)
$$

would force $x=y=0$, which is impossible on $x^2+y^2=1$. For each $p\in C$, choose a sufficiently small coordinate neighbourhood $U_p$ such that

$$
U_p\cap a(U_p)=\varnothing.
$$

Then the quotient projection restricts to a homeomorphism

$$
\pi|_{U_p}:U_p\longrightarrow \pi(U_p).
$$

Transporting a smooth chart $\phi_p:U_p\to\mathbb R^2$ across this homeomorphism gives the quotient chart

$$
\widetilde\phi_p
=\phi_p\circ(\pi|_{U_p})^{-1}.
$$

On an overlap, a lift lies either in another chosen neighbourhood or in its image under $a$. The corresponding transition map is therefore a transition map on $C$, possibly composed with the diffeomorphism $a$, and is smooth. Since this is a free action of the finite group $\{1,a\}$, the quotient is Hausdorff and second countable. This constructs the [smooth quotient by a free finite group action](../../../differential-geometry.md#smooth-quotient-by-a-free-finite-group-action), and in these charts $\pi$ is locally the identity. Hence $\pi$ is a [local diffeomorphism](../../../calculus.md#local-diffeomorphism), in particular smooth.

To test orientability, parametrize the cylinder by

$$
F(\theta,z)=(\cos\theta,\sin\theta,z).
$$

The involution acts in these coordinates as

$$
(\theta,z)\longmapsto(\theta+\pi,-z),
$$

whose derivative has determinant $-1$. Thus $a$ is an [orientation-reversing diffeomorphism](../../../differential-geometry.md#orientation-reversing-diffeomorphism) of the cylinder.

If the quotient surface $S$ were orientable, its orientation would pull back through the local diffeomorphism $\pi$ to an orientation of $C$. The identity $\pi\circ a=\pi$ would then force $a$ to preserve that pulled-back orientation, contradicting the negative determinant above. Therefore

$$
\boxed{S\text{ is not orientable}}.
$$

## 12B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="12b/solution">Solution</h3>

↑ **Parent:** [12B](#12b)

The [Laplace transform](../../../analysis.md#laplace-transform) of a function on $t\geq0$ is

$$
\widehat f(s)=\mathcal L\{f\}(s)
=\int_0^\infty e^{-st}f(t)\,dt,
$$

for values of $s$ for which the [integral](../../../calculus.md#integral) converges. [Integration by parts](../../../calculus.md#integration-by-parts) gives the [Laplace transform of a derivative](../../../analysis.md#laplace-transform-of-a-derivative)

$$
\boxed{\mathcal L\{f'\}(s)=s\widehat f(s)-f(0)}.
$$

Write $\widehat N_i(s)=\mathcal L\{N_i\}(s)$. Transforming the first two equations and using the initial data gives

$$
\widehat N_1(s)=\frac{N}{s+\lambda_1},
\qquad
\widehat N_2(s)
=\frac{N\lambda_1}{(s+\lambda_1)(s+\lambda_2)}.
$$

The third equation then gives

$$
(s+\lambda_3)\widehat N_3(s)-n
=\lambda_2\widehat N_2(s),
$$

and hence

$$
\widehat N_3(s)
=\frac n{s+\lambda_3}
+\frac{N\lambda_1\lambda_2}
{(s+\lambda_1)(s+\lambda_2)(s+\lambda_3)}.
$$

A [partial fraction decomposition](../../../isolated-singularity.md#partial-fraction-decomposition) therefore yields the [sequential radioactive decay](../../../physics.md#sequential-radioactive-decay) formula

$$
\boxed{
\begin{aligned}
N_3(t)={}&ne^{-\lambda_3t}\\
&+N\lambda_1\lambda_2\left[
\frac{e^{-\lambda_1t}}{(\lambda_2-\lambda_1)(\lambda_3-\lambda_1)}
+\frac{e^{-\lambda_2t}}{(\lambda_1-\lambda_2)(\lambda_3-\lambda_2)}
+\frac{e^{-\lambda_3t}}{(\lambda_1-\lambda_3)(\lambda_2-\lambda_3)}
\right].
\end{aligned}
}
$$

Now let $\lambda_1=\lambda_2=\lambda$ and put $\Delta=\lambda_3-\lambda>0$. The transformed contribution originating from the initial $N_1$ population becomes

$$
\frac{N\lambda^2}{(s+\lambda)^2(s+\lambda_3)}.
$$

Equivalently, solve the middle equation first to obtain

$$
N_2(t)=N\lambda t e^{-\lambda t},
$$

and use an [integrating factor](../../../differential-equation.md#integrating-factor) in the final equation:

$$
N_3(t)=ne^{-\lambda_3t}
+N\lambda^2e^{-\lambda_3t}\int_0^t u e^{\Delta u}\,du.
$$

Evaluating the elementary integral gives

$$
\boxed{
N_3(t)
=ne^{-\lambda_3t}
+\frac{N\lambda^2}{(\lambda_3-\lambda)^2}
\left[
e^{-\lambda t}\bigl((\lambda_3-\lambda)t-1\bigr)
+e^{-\lambda_3t}
\right]
}.
$$

## 13D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="13d/a">a</h3>

↑ **Parent:** [13D](#13d)

<h4 id="13d/a/solution">Solution</h4>

↑ **Parent:** [A](#13d/a)

Let $y_\varepsilon=y+\varepsilon\eta$, where the [variation](../../../calculus-of-variations.md#variation) $\eta$ satisfies $\eta(a)=\eta(b)=0$. Differentiating the [functional](../../../calculus-of-variations.md#functional) at $\varepsilon=0$ gives its [first variation](../../../calculus-of-variations.md#first-variation)

$$
\delta I
=\int_a^b\left(L_y\eta+L_{y'}\eta'\right)\,dx.
$$

Using [integration by parts](../../../calculus.md#integration-by-parts) and the fixed endpoint conditions,

$$
\delta I
=\int_a^b\left(
L_y-\frac d{dx}L_{y'}
\right)\eta\,dx.
$$

If this vanishes for every admissible $\eta$, the [fundamental lemma of the calculus of variations](../../../calculus-of-variations.md#fundamental-lemma-of-the-calculus-of-variations) gives the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation)

$$
\boxed{\frac d{dx}\frac{\partial L}{\partial y'}
-\frac{\partial L}{\partial y}=0}.
$$

<h3 id="13d/b">b</h3>

↑ **Parent:** [13D](#13d)

<h4 id="13d/b/solution">Solution</h4>

↑ **Parent:** [B](#13d/b)

For

$$
L=\frac{\sqrt{1+y'^2}}x,
$$

one has $L_y=0$ and

$$
L_{y'}=\frac{y'}{x\sqrt{1+y'^2}}.
$$

A circle of radius $R$ centred at $(0,c)$ on the $y$-axis satisfies

$$
x^2+(y-c)^2=R^2,
\qquad
y'=-\frac{x}{y-c}.
$$

On any arc that does not cross $y=c$,

$$
\sqrt{1+y'^2}=\frac R{|y-c|},
\qquad
L_{y'}=-\frac{\operatorname{sgn}(y-c)}R,
$$

which is constant. Hence $dL_{y'}/dx=0=L_y$, so the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) holds and $\delta I=0$. These circles are the coordinate-swapped form of a [Geodesic in the Poincare half-plane model](../../../geometry-and-topology.md#geodesic-in-the-poincare-half-plane-model).

<h3 id="13d/c">c</h3>

↑ **Parent:** [13D](#13d)

<h4 id="13d/c/solution">Solution</h4>

↑ **Parent:** [C](#13d/c)

Here the integrand

$$
L=\frac{\sqrt{1+y'^2}}y
$$

has no explicit $x$-dependence. The [Beltrami identity](../../../analysis.md#beltrami-identity) therefore gives

$$
L-y'L_{y'}
=\frac1{y\sqrt{1+y'^2}}
=\frac1R
$$

for a positive constant $R$. Thus

$$
y'^2=\frac{R^2-y^2}{y^2},
$$

whose nonvertical solutions are the semicircles

$$
(x-c)^2+y^2=R^2.
$$

The endpoint $(a,a)$ and the prescribed value at $x=b$ both lie on

$$
(x-a)^2+y^2=a^2,
$$

because

$$
(b-a)^2+(2ab-b^2)=a^2.
$$

The required positive arc is consequently

$$
\boxed{y(x)=\sqrt{a^2-(x-a)^2}=\sqrt{2ax-x^2}},
\qquad a\leq x\leq b.
$$

The condition $b<2a$ keeps the endpoint above the $x$-axis. The sketch is the descending part of the upper semicircle of radius $a$ centred at $(a,0)$, from $(a,a)$ to

$$
\left(b,\sqrt{2ab-b^2}\right).
$$

This is precisely a [Geodesic in the Poincare half-plane model](../../../geometry-and-topology.md#geodesic-in-the-poincare-half-plane-model).

## 14C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="14c/solution">Solution</h3>

↑ **Parent:** [14C](#14c)

For

$$
\theta(x,t)=t^{-1/2}e^{-x^2/(4Dt)},
$$

direct [differentiation](../../../calculus.md#partial-derivative) gives

$$
\theta_t
=\left(-\frac1{2t}+\frac{x^2}{4Dt^2}\right)\theta
$$

and

$$
D\theta_{xx}
=D\left(-\frac1{2Dt}+\frac{x^2}{4D^2t^2}\right)\theta
=\left(-\frac1{2t}+\frac{x^2}{4Dt^2}\right)\theta.
$$

Thus $\theta_t=D\theta_{xx}$.

Its total mass is found from the [Gaussian integral](../../../calculus.md#gaussian-integral):

$$
\int_{-\infty}^{\infty}\theta(x,t)\,dx
=2\sqrt{\pi D}.
$$

The unit-mass solution converging to the [Dirac delta function](../../../distribution-theory.md#dirac-delta-function) as $t\downarrow0$ is therefore the [heat kernel](../../../diffusion-equation.md#heat-kernel)

$$
\boxed{
K(x,t)=\frac1{\sqrt{4\pi Dt}}
\exp\left(-\frac{x^2}{4Dt}\right)
}.
$$

For the second initial condition, the [heat-kernel solution](../../../diffusion-equation.md#heat-kernel-solution) is the [convolution](../../../fourier-analysis.md#convolution)

$$
\theta(x,t)
=\int_{-1}^1
\frac1{\sqrt{4\pi Dt}}
\exp\left(-\frac{(x-y)^2}{4Dt}\right)\,dy.
$$

With $u=(x-y)/(2\sqrt{Dt})$ and the definition of the [error function](../../../calculus.md#error-function), this becomes

$$
\boxed{
\theta(x,t)=\frac12\left[
\operatorname{Erf}\left(\frac{x+1}{2\sqrt{Dt}}\right)
-\operatorname{Erf}\left(\frac{x-1}{2\sqrt{Dt}}\right)
\right]
}.
$$

This is the [heat equation with interval-indicator initial data](../../../diffusion-equation.md#heat-equation-with-interval-indicator-initial-data) for $a=1$.

At $t=0$ the graph is the rectangle of height one on $[-1,1]$. For every $t>0$ it is smooth, positive and even, with its maximum at $x=0$. As time increases the graph broadens and its maximum falls, while its total area remains $2$; pointwise it tends to zero as $t\to\infty$.

## 15C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="15c/a">a</h3>

↑ **Parent:** [15C](#15c)

<h4 id="15c/a/solution">Solution</h4>

↑ **Parent:** [A](#15c/a)

The [orbital angular momentum commutation relations](../../../quantum-mechanics.md#orbital-angular-momentum-commutation-relations) give

$$
[L_z,L_x]=i\hbar L_y,
\qquad
[L_z,L_y]=-i\hbar L_x.
$$

Consequently

$$
\begin{aligned}
[L_z,L_\pm]
&=[L_z,L_x]\pm i[L_z,L_y]\\
&=i\hbar L_y\pm\hbar L_x
=\boxed{\pm\hbar L_\pm}.
\end{aligned}
$$

The same commutation relations imply $[L^2,L_x]=[L^2,L_y]=0$, and hence

$$
\boxed{[L^2,L_\pm]=0}.
$$

These are the defining identities for the [angular momentum ladder operators](../../../quantum-mechanics.md#angular-momentum-ladder-operator).

If

$$
L_z\phi=m\hbar\phi,
\qquad
L^2\phi=\ell(\ell+1)\hbar^2\phi,
$$

then, whenever $L_\pm\phi\ne0$,

$$
\begin{aligned}
L_z(L_\pm\phi)
&=([L_z,L_\pm]+L_\pm L_z)\phi
=(m\pm1)\hbar L_\pm\phi,\\
L^2(L_\pm\phi)
&=L_\pm L^2\phi
=\ell(\ell+1)\hbar^2L_\pm\phi.
\end{aligned}
$$

**Thus $L_\pm\phi$ has quantum numbers $(\ell,m\pm1)$.**

<h3 id="15c/b">b</h3>

↑ **Parent:** [15C](#15c)

<h4 id="15c/b/solution">Solution</h4>

↑ **Parent:** [B](#15c/b)

The Hamiltonian is the sum of three commuting one-dimensional [harmonic-oscillator](../../../quantum-mechanics.md#quantum-harmonic-oscillator) Hamiltonians. Its product [eigenstates](../../../quantum-mechanics.md#eigenstate) are

$$
\Psi_{n_xn_yn_z}(x,y,z)
=\psi_{n_x}(x)\psi_{n_y}(y)\psi_{n_z}(z),
$$

with energies

$$
\boxed{
E_{n_xn_yn_z}
=\hbar\omega\left(n_x+n_y+n_z+\frac32\right)
}.
$$

Equivalently, the level with $N=n_x+n_y+n_z$ has energy $E_N=\hbar\omega(N+3/2)$, as in the [three-dimensional isotropic harmonic oscillator](../../../quantum-mechanics.md#three-dimensional-isotropic-harmonic-oscillator).

Up to normalization, the ground-state wavefunction is

$$
\Psi_{000}
=\exp\left[-\frac{M\omega}{2\hbar}(x^2+y^2+z^2)\right].
$$

It is radial, so $\nabla\Psi_{000}$ is parallel to the position vector. Since the [orbital angular momentum](../../../quantum-mechanics.md#orbital-angular-momentum) is $L=-i\hbar\,r\times\nabla$, every component of $L$ annihilates this state. Therefore

$$
L_z\Psi_{000}=0,
\qquad
L^2\Psi_{000}=0,
$$

and the ground state has $\ell=m=0$.

The first excited level has $N=1$ and is spanned by

$$
x\Psi_{000},\qquad y\Psi_{000},\qquad z\Psi_{000}.
$$

The state

$$
\Phi_0=z\Psi_{000}
$$

satisfies $L_z\Phi_0=0$. Applying the ladder operators gives

$$
L_+\Phi_0=-\hbar(x+iy)\Psi_{000},
\qquad
L_-\Phi_0=\hbar(x-iy)\Psi_{000}.
$$

Hence convenient $m=\pm1$ eigenstates are

$$
\boxed{\Phi_{\pm1}=(x\pm iy)\Psi_{000}},
$$

up to normalization and irrelevant overall phases.

Finally, the isotropic Hamiltonian is rotationally invariant. The [rotational invariance of a central-potential Hamiltonian](../../../quantum-mechanics.md#rotational-invariance-of-a-central-potential-hamiltonian) gives

$$
[H,L_z]=[H,L^2]=[L_z,L^2]=0.
$$

These commuting self-adjoint operators can be simultaneously diagonalized within each energy eigenspace, which is why joint eigenstates of $H,L^2,L_z$ must exist.

## 16A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="16a/a">a</h3>

↑ **Parent:** [16A](#16a)

<h4 id="16a/a/solution">Solution</h4>

↑ **Parent:** [A](#16a/a)

In [spherical symmetry](../../../geometry-and-topology.md#spherical-symmetry), the velocity is radial and constant over each sphere. Hence

$$
Q(R,t)=4\pi R^2u(R,t).
$$

Apply the [divergence theorem](../../../calculus.md#divergence-theorem) to the fluid shell between radii $R_1$ and $R_2$. Since the flow is [incompressible](../../../fluid-mechanics.md#incompressible-flow),

$$
0=\int_{\text{shell}}\nabla\cdot u\,dV
=Q(R_2,t)-Q(R_1,t).
$$

**Thus $Q$ is independent of $R$ and is a function of time alone. This is the flux law for [spherically symmetric incompressible radial flow](../../../fluid-mechanics.md#spherically-symmetric-incompressible-radial-flow).**

<h3 id="16a/b">b</h3>

↑ **Parent:** [16A](#16a)

<h4 id="16a/b/solution">Solution</h4>

↑ **Parent:** [B](#16a/b)

The radial velocity and [velocity potential](../../../fluid-mechanics.md#velocity-potential) are

$$
u(r,t)=\frac{Q(t)}{4\pi r^2},
\qquad
\phi(r,t)=-\frac{Q(t)}{4\pi r}.
$$

Choose the gauge in the [Unsteady Bernoulli equation](../../../fluid-mechanics.md#unsteady-bernoulli-equation) by evaluating it at infinity, where $u=0$, $\phi=0$, and $p=p_0$:

$$
\phi_t+\frac12u^2+\frac p\rho=\frac{p_0}\rho.
$$

At the cavity surface the vacuum pressure is zero, and the [kinematic boundary condition](../../../fluid-mechanics.md#kinematic-boundary-condition) gives $u(a,t)=\dot a$. Since

$$
\phi_t(a,t)=-\frac1{4\pi a}\frac{dQ}{dt},
$$

Bernoulli's equation becomes

$$
-\frac1{4\pi a}\frac{dQ}{dt}
+\frac{\dot a^2}{2}
=\frac{p_0}{\rho}.
$$

Therefore

$$
\boxed{
\frac1{4\pi a}\frac{dQ}{dt}
-\frac{\dot a^2}{2}
=-\frac{p_0}{\rho}
}.
$$

<h3 id="16a/c">c</h3>

↑ **Parent:** [16A](#16a)

<h4 id="16a/c/solution">Solution</h4>

↑ **Parent:** [C](#16a/c)

At the moving boundary,

$$
Q=4\pi a^2\dot a.
$$

Substitution into the result of part (b) gives the [Rayleigh collapse equation](../../../fluid-mechanics.md#rayleigh-collapse-of-a-spherical-cavity)

$$
a\ddot a+\frac32\dot a^2=-\frac{p_0}{\rho}.
$$

Treat $v=\dot a$ as a function of $a$, so that $\ddot a=v\,dv/da$. With $w=v^2$, the equation becomes

$$
a\frac{dw}{da}+3w=-\frac{2p_0}{\rho}.
$$

Multiplication by the [integrating factor](../../../differential-equation.md#integrating-factor) $a^3$ after division by $a$ gives

$$
\frac d{da}(a^3w)=-\frac{2p_0}{\rho}a^2.
$$

Using $w(a_0)=0$,

$$
w(a)=\frac{2p_0}{3\rho}
\left(\frac{a_0^3}{a^3}-1\right).
$$

The collapsing branch has negative radial velocity, so

$$
\boxed{
\dot a=-\sqrt{\frac{2p_0}{3\rho}
\left(\frac{a_0^3}{a^3}-1\right)}
}.
$$

<h3 id="16a/d">d</h3>

↑ **Parent:** [16A](#16a)

<h4 id="16a/d/solution">Solution</h4>

↑ **Parent:** [D](#16a/d)

Since $dt=da/\dot a$ on the collapsing branch, the time for $a$ to decrease from $a_0$ to zero is

$$
\boxed{
\tau
=\sqrt{\frac{3\rho}{2p_0}}
\int_0^{a_0}
\frac{da}{\sqrt{a_0^3/a^3-1}}
}.
$$

Equivalently, scaling $a=a_0x$ gives

$$
\boxed{\tau
=a_0\sqrt{\frac{3\rho}{2p_0}}
\int_0^1\frac{x^{3/2}}{\sqrt{1-x^3}}\,dx.}
$$

## 17H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="17h/a">a</h3>

↑ **Parent:** [17H](#17h)

<h4 id="17h/a/solution">Solution</h4>

↑ **Parent:** [A](#17h/a)

Here $X$ has the [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) $\operatorname{Bin}(n,\theta)$, so, up to a factor independent of $\theta$, the [likelihood function](../../../statistical-modelling.md#likelihood-function) is

$$
L(\theta;X)=\theta^X(1-\theta)^{n-X}.
$$

For $0<X<n$, differentiating the [log-likelihood](../../../statistical-modelling.md#log-likelihood) gives

$$
\frac X\theta-\frac{n-X}{1-\theta}=0,
$$

and the boundary cases give the same formula. Thus the [binomial proportion maximum-likelihood estimator](../../../statistical-modelling.md#binomial-proportion-maximum-likelihood-estimator) is

$$
\boxed{\widehat\theta=\frac Xn}.
$$

<h3 id="17h/b">b</h3>

↑ **Parent:** [17H](#17h)

<h4 id="17h/b/solution">Solution</h4>

↑ **Parent:** [B](#17h/b)

The estimator is unbiased because $\mathbb E_\theta X=n\theta$, and

$$
\operatorname{Var}_\theta(\widehat\theta)
=\frac1{n^2}\operatorname{Var}_\theta(X)
=\frac{\theta(1-\theta)}n.
$$

The [bias-variance decomposition of mean squared error](../../../statistical-modelling.md#bias-variance-decomposition-of-mean-squared-error) therefore gives

$$
\boxed{f(\theta)
=\mathbb E_\theta[(\widehat\theta-\theta)^2]
=\frac{\theta(1-\theta)}n}.
$$

The quadratic $\theta(1-\theta)$ is maximized at $\theta=1/2$, so

$$
\boxed{\sup_{0<\theta<1}f(\theta)=\frac1{4n}}.
$$

<h3 id="17h/c">c</h3>

↑ **Parent:** [17H](#17h)

<h4 id="17h/c/solution">Solution</h4>

↑ **Parent:** [C](#17h/c)

The uniform prior is the [Beta distribution](../../../probability-theory.md#beta-distribution) $\operatorname{Beta}(1,1)$. By [Beta-binomial conjugacy](../../../statistical-inference.md#beta-binomial-conjugacy), after observing $X$ heads the posterior is

$$
\theta\mid X\sim\operatorname{Beta}(X+1,n-X+1).
$$

The [Bayes estimator under squared error loss](../../../statistical-inference.md#bayes-estimator-under-squared-error-loss) is the posterior mean, hence

$$
\boxed{\widehat\theta_B=\frac{X+1}{n+2}}.
$$

<h3 id="17h/d">d</h3>

↑ **Parent:** [17H](#17h)

<h4 id="17h/d/solution">Solution</h4>

↑ **Parent:** [D](#17h/d)

For the weighted loss, the [Bayes estimator under parameter-weighted squared error](../../../statistical-inference.md#bayes-estimator-under-parameter-weighted-squared-error) is the mean of the posterior after multiplication by

$$
\theta^{\alpha-1}(1-\theta)^{\beta-1}.
$$

Since the original posterior density is proportional to

$$
\theta^X(1-\theta)^{n-X},
$$

the reweighted density is $\operatorname{Beta}(X+\alpha,n-X+\beta)$. Its mean gives

$$
\widetilde\theta=\frac{X+\alpha}{n+\alpha+\beta}.
$$

Writing this in the required form,

$$
\boxed{
\widetilde\theta
=w\widehat\theta+(1-w)\theta_0,
\qquad
w=\frac n{n+\alpha+\beta},
\qquad
\theta_0=\frac{\alpha}{\alpha+\beta}
}.
$$

<h3 id="17h/e">e</h3>

↑ **Parent:** [17H](#17h)

<h4 id="17h/e/solution">Solution</h4>

↑ **Parent:** [E](#17h/e)

For

$$
\widetilde\theta=w\frac Xn+(1-w)\theta_0,
$$

the bias and variance are

$$
\mathbb E_\theta\widetilde\theta-\theta
=(1-w)(\theta_0-\theta),
\qquad
\operatorname{Var}_\theta(\widetilde\theta)
=\frac{w^2}{n}\theta(1-\theta).
$$

The [bias-variance decomposition of mean squared error](../../../statistical-modelling.md#bias-variance-decomposition-of-mean-squared-error) yields

$$
\boxed{
g_{w,\theta_0}(\theta)
=\frac{w^2}{n}\theta(1-\theta)
+(1-w)^2(\theta-\theta_0)^2
}.
$$

This is the risk formula for an [affine shrinkage estimator for a binomial proportion](../../../statistical-modelling.md#affine-shrinkage-estimator-for-a-binomial-proportion).

<h3 id="17h/f">f</h3>

↑ **Parent:** [17H](#17h)

<h4 id="17h/f/solution">Solution</h4>

↑ **Parent:** [F](#17h/f)

Set $\theta_0=1/2$ and $z=(\theta-1/2)^2$. Since

$$
\theta(1-\theta)=\frac14-z,
\qquad
0\leq z<\frac14,
$$

the risk is affine in $z$:

$$
g_{w,1/2}(\theta)
=\frac{w^2}{4n}
+z\left((1-w)^2-\frac{w^2}{n}\right).
$$

Its supremum is therefore controlled by the midpoint $z=0$ and the endpoint limit $z\to1/4$. Requiring both endpoint values to be at most the MLE's maximal risk $1/(4n)$ gives

$$
\frac{w^2}{4n}\leq\frac1{4n},
\qquad
\frac{(1-w)^2}{4}\leq\frac1{4n}.
$$

Equivalently,

$$
|w|\leq1,
\qquad
|1-w|\leq\frac1{\sqrt n}.
$$

Their intersection is

$$
\boxed{1-\frac1{\sqrt n}\leq w\leq1}.
$$

For precisely this range, the shrinkage estimator has maximal [mean squared error](../../../statistical-modelling.md#mean-squared-error) no greater than that of $\widehat\theta$.

## 18H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="18h/a">a</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/a/solution">Solution</h4>

↑ **Parent:** [A](#18h/a)

A vector $x$ is a [basic feasible solution](../../../mathematical-optimization.md#basic-feasible-solution) when

$$
Ax=b,\qquad x\geq0,
$$

and the columns $A_i$ for which $x_i>0$ are [linearly independent](../../../vector-space.md#linear-independence). Equivalently, after extending those columns to a basis of the column space of $A$, one sets all nonbasic variables to zero and solves for the basic variables, obtaining a nonnegative vector.

<h3 id="18h/b">b</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/b/solution">Solution</h4>

↑ **Parent:** [B](#18h/b)

Choose an optimal feasible vector $x$ having as few positive coordinates as possible, and let

$$
S=\{i:x_i>0\}.
$$

If the columns $(A_i)_{i\in S}$ were linearly dependent, there would be a nonzero vector $h$, supported on $S$, such that $Ah=0$. For all sufficiently small positive $\varepsilon$, both

$$
x+\varepsilon h
\quad\hbox{and}\quad
x-\varepsilon h
$$

would remain feasible.

If $c^Th\ne0$, one of these two perturbations would increase the objective, contradicting optimality. Hence $c^Th=0$. We may then increase $\varepsilon$ in one of the two directions until at least one positive coordinate first becomes zero. The resulting vector is still feasible and optimal but has smaller positive support, contradicting the choice of $x$.

**Thus the active columns are linearly independent, so $x$ is basic. This proves the [Fundamental theorem of linear programming](../../../mathematical-optimization.md#fundamental-theorem-of-linear-programming): whenever the finite maximum is attained, an optimal basic feasible solution exists.**

<h3 id="18h/c">c</h3>

↑ **Parent:** [18H](#18h)

<h4 id="18h/c/i">i</h4>

↑ **Parent:** [C](#18h/c)

<h5 id="18h/c/i/solution">Solution</h5>

↑ **Parent:** [I](#18h/c/i)

Apply the [Charnes-Cooper transformation](../../../mathematical-optimization.md#charnes-cooper-transformation) to any feasible point $x$ of $Q$:

$$
y=\frac{x}{d^Tx},
\qquad
t=\frac1{d^Tx}.
$$

Then

$$
y\geq0,\quad t>0,\quad Ay=bt,\quad d^Ty=1,
$$

so $(y,t)$ is feasible for $R$, and

$$
c^Ty=\frac{c^Tx}{d^Tx}.
$$

In particular, the given solution $x^*$ of $Q$ produces a feasible point of $R$ with the same objective value, so

$$
\max R\geq\max Q.
$$

Moreover, because every $d_i>0$, the equation $d^Ty=1$ implies

$$
0\leq y_i\leq\frac1{d_i}.
$$

The linear objective $c^Ty$ is therefore bounded on the feasible set. The feasible $y$ lie in the compact simplex $\{y\geq0:d^Ty=1\}$. Their subset arising in $R$ is closed: if $b\ne0$, any nonzero component of $b$ determines $t$ continuously from $Ay=bt$, while if $b=0$ the condition is simply $Ay=0$. Hence the feasible $y$ form a [compact set](../../../topology.md#compact-space), on which the continuous objective $c^Ty$ attains a finite maximum. Thus $R$ has a finite maximum at least as large as that of $Q$.

<h4 id="18h/c/ii">ii</h4>

↑ **Parent:** [C](#18h/c)

<h5 id="18h/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#18h/c/ii)

Let $(y,t)$ be feasible for $R$. Since $d_i>0$ and $d^Ty=1$, the vector $y$ is nonzero. Every entry of $A$ is strictly positive and $y\geq0$, so every component of $Ay$ is strictly positive. The relation

$$
Ay=bt
$$

therefore forces $t>0$.

Set $x=y/t$. Then

$$
x\geq0,\qquad Ax=b,\qquad d^Tx=\frac1t>0,
$$

so $x$ is feasible for $Q$, and

$$
\frac{c^Tx}{d^Tx}
=\frac{c^Ty/t}{1/t}
=c^Ty.
$$

Thus every feasible value of $R$ is a feasible value of the [linear-fractional program](../../../mathematical-optimization.md#linear-fractional-programming) $Q$. Together with part (i), this proves

$$
\boxed{\max R=\max Q}.
$$

<h4 id="18h/c/iii">iii</h4>

↑ **Parent:** [C](#18h/c)

<h5 id="18h/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#18h/c/iii)

Let $(y,t)$ be a basic feasible solution of $R$. Part (ii) gives $t>0$, and put $x=y/t$. We already know that $x$ is feasible for $P$.

Suppose the columns $A_i$ with $y_i>0$ were linearly dependent. Then some nonzero $h$, supported on those indices, would satisfy $Ah=0$. Put

$$
q=d^Th,\qquad
\delta y=h-qy,\qquad
\delta t=-qt.
$$

Since $d^Ty=1$ and $Ay=bt$,

$$
d^T\delta y=0,
\qquad
A\delta y-b\delta t=0.
$$

The vector $(\delta y,\delta t)$ is nonzero and is supported only on positive variables of $(y,t)$. It is therefore a linear dependence among the active constraint columns of $R$, contradicting that $(y,t)$ is basic. Hence the active columns $A_i$ are linearly independent, and

$$
x=\frac yt\in\mathcal B.
$$

By the [Fundamental theorem of linear programming](../../../mathematical-optimization.md#fundamental-theorem-of-linear-programming), $R$ has an optimal basic feasible solution. Its image $x\in\mathcal B$ has the same objective ratio, by part (ii). Conversely, every $x\in\mathcal B$ is feasible for $Q$ and maps to a feasible point of $R$. Since $x^*$ solves $Q$,

$$
\boxed{
\frac{c^Tx^*}{d^Tx^*}
=\max_{x\in\mathcal B}\frac{c^Tx}{d^Tx}
}.
$$

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
