# Paper 4

↑ **Parent:** [Ib](../ib.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2023/paperib_4_2023.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2023/paperib_4_2023.pdf)

**Table of contents**

- [1F](#1f)
  - [Solution](#1f/solution)
- [2G](#2g)
  - [Solution](#2g/solution)
- [3G](#3g)
  - [i](#3g/i)
    - [Solution](#3g/i/solution)
  - [ii](#3g/ii)
    - [Solution](#3g/ii/solution)
  - [iii](#3g/iii)
    - [Solution](#3g/iii/solution)
- [4D](#4d)
  - [a](#4d/a)
    - [Solution](#4d/a/solution)
  - [b](#4d/b)
    - [Solution](#4d/b/solution)
- [5D](#5d)
  - [a](#5d/a)
    - [Solution](#5d/a/solution)
  - [b](#5d/b)
    - [Solution](#5d/b/solution)
  - [c](#5d/c)
    - [Solution](#5d/c/solution)
- [6B](#6b)
  - [a](#6b/a)
    - [Solution](#6b/a/solution)
  - [b](#6b/b)
    - [Solution](#6b/b/solution)
- [7H](#7h)
  - [a](#7h/a)
    - [Solution](#7h/a/solution)
  - [b](#7h/b)
    - [Solution](#7h/b/solution)
  - [c](#7h/c)
    - [Solution](#7h/c/solution)
- [8F](#8f)
  - [Solution](#8f/solution)
- [9E](#9e)
  - [Solution](#9e/solution)
- [10G](#10g)
  - [i](#10g/i)
    - [Solution](#10g/i/solution)
  - [ii](#10g/ii)
    - [Solution](#10g/ii/solution)
  - [iii](#10g/iii)
    - [Solution](#10g/iii/solution)
- [11E](#11e)
  - [a](#11e/a)
    - [Solution](#11e/a/solution)
  - [b](#11e/b)
    - [Solution](#11e/b/solution)
  - [c](#11e/c)
    - [Solution](#11e/c/solution)
  - [d](#11e/d)
    - [Solution](#11e/d/solution)
- [12B](#12b)
  - [a](#12b/a)
    - [Solution](#12b/a/solution)
  - [b](#12b/b)
    - [Solution](#12b/b/solution)
  - [c](#12b/c)
    - [Solution](#12b/c/solution)
- [13C](#13c)
  - [a](#13c/a)
    - [Solution](#13c/a/solution)
  - [b](#13c/b)
    - [i](#13c/b/i)
      - [Solution](#13c/b/i/solution)
    - [ii](#13c/b/ii)
      - [Solution](#13c/b/ii/solution)
    - [iii](#13c/b/iii)
      - [Solution](#13c/b/iii/solution)
- [14A](#14a)
  - [a](#14a/a)
    - [Solution](#14a/a/solution)
  - [b](#14a/b)
    - [Solution](#14a/b/solution)
  - [c](#14a/c)
    - [Solution](#14a/c/solution)
- [15D](#15d)
  - [a](#15d/a)
    - [Solution](#15d/a/solution)
  - [b](#15d/b)
    - [i](#15d/b/i)
      - [Solution](#15d/b/i/solution)
    - [ii](#15d/b/ii)
      - [Solution](#15d/b/ii/solution)
    - [iii](#15d/b/iii)
      - [Solution](#15d/b/iii/solution)
- [16C](#16c)
  - [a](#16c/a)
    - [Solution](#16c/a/solution)
  - [b](#16c/b)
    - [i](#16c/b/i)
      - [Solution](#16c/b/i/solution)
    - [ii](#16c/b/ii)
      - [Solution](#16c/b/ii/solution)
    - [iii](#16c/b/iii)
      - [Solution](#16c/b/iii/solution)
    - [iv](#16c/b/iv)
      - [Solution](#16c/b/iv/solution)
    - [v](#16c/b/v)
      - [Solution](#16c/b/v/solution)
    - [vi](#16c/b/vi)
      - [Solution](#16c/b/vi/solution)
- [17H](#17h)
  - [a](#17h/a)
    - [Solution](#17h/a/solution)
  - [b](#17h/b)
    - [Solution](#17h/b/solution)
  - [c](#17h/c)
    - [Solution](#17h/c/solution)
  - [d](#17h/d)
    - [Solution](#17h/d/solution)
- [18H](#18h)
  - [Solution](#18h/solution)

## 1F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1f/solution">Solution</h3>

↑ **Parent:** [1F](#1f)

A [bilinear form](../../../linear-algebra.md#bilinear-form) $B$ on $V$ is [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form) when

$$
B(v,w)=0\quad\text{for every }v\in V
\qquad\Longrightarrow\qquad w=0.
$$

In finite dimensions this is equivalent to nondegeneracy in the first argument.

Define the [linear map](../../../vector-space.md#linear-map)

$$
\beta_1:V\longrightarrow V^*,
\qquad
\beta_1(w)=B_1(-,w).
$$

Nondegeneracy makes $\beta_1$ injective. Since $V$ and its [dual space](../../../linear-algebra.md#dual-space) have the same finite dimension, $\beta_1$ is an isomorphism. Similarly define $\beta_2(w)=B_2(-,w)$ and set

$$
\boxed{\alpha=\beta_1^{-1}\beta_2}.
$$

Then $\alpha$ is linear and

$$
B_1(v,\alpha w)=\beta_1(\alpha w)(v)
=\beta_2(w)(v)=B_2(v,w).
$$

If $w\in\ker\alpha$, this identity gives $B_2(v,w)=0$ for every $v$. Conversely, if $B_2(v,w)=0$ for every $v$, then $B_1(v,\alpha w)=0$ for every $v$, so nondegeneracy gives $\alpha w=0$. Hence

$$
\boxed{\{w\in V:B_2(v,w)=0\text{ for every }v\in V\}=\ker\alpha}.
$$

This is the [representation of a bilinear form relative to a nondegenerate bilinear form](../../../linear-algebra.md#representation-of-a-bilinear-form-relative-to-a-nondegenerate-bilinear-form).

## 2G

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2g/solution">Solution</h3>

↑ **Parent:** [2G](#2g)

Fix $x\in X$. By assumption there is a neighbourhood $U$ of $x$ on which $f_n\to f$ with [uniform convergence](../../../real-analysis.md#uniform-convergence). Each restriction $f_n|_U$ is [continuous](../../../calculus.md#continuous-function), and a uniform limit of continuous functions is continuous. Thus $f|_U$ is continuous, in particular at $x$. Since $x$ was arbitrary, $f$ is continuous on $X$.

Now let $K\subseteq X$ be [compact](../../../topology.md#compact-space) and let $\varepsilon>0$. For each $x\in K$, choose a neighbourhood $U_x$ on which convergence is uniform. The sets $U_x$ cover $K$, so compactness gives a finite subcover

$$
K\subseteq U_{x_1}\cup\cdots\cup U_{x_m}.
$$

For each $j$, choose $N_j$ such that

$$
n\geq N_j,\ y\in U_{x_j}
\quad\Longrightarrow\quad |f_n(y)-f(y)|<\varepsilon.
$$

Taking $N=\max_jN_j$, every $y\in K$ belongs to one of these finitely many neighbourhoods, and therefore

$$
n\geq N\quad\Longrightarrow\quad
\sup_{y\in K}|f_n(y)-f(y)|<\varepsilon.
$$

**Thus $f_n\to f$ uniformly on every compact subset. This proves the [local uniform convergence on compact subsets](../../../real-analysis.md#local-uniform-convergence-on-compact-subsets) principle.**

## 3G

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3g/i">i</h3>

↑ **Parent:** [3G](#3g)

<h4 id="3g/i/solution">Solution</h4>

↑ **Parent:** [I](#3g/i)

The domains are not [conformally equivalent](../../../geometry-and-topology.md#conformal-equivalence). Suppose that $F:\mathbb C\setminus\{0\}\to\{w:0<|w|<1\}$ were a conformal equivalence. Since $F$ is bounded near zero, the [Riemann removable singularity theorem](../../../isolated-singularity.md#riemann-removable-singularity-theorem) extends it holomorphically across zero. The extension is a bounded [entire function](../../../complex-analysis.md#entire-function), so the [Liouville theorem](../../../complex-analysis.md#liouville-theorem) makes it constant, contradicting bijectivity. This is the [punctured plane is not conformally equivalent to the punctured unit disc](../../../geometry-and-topology.md#punctured-plane-is-not-conformally-equivalent-to-the-punctured-unit-disc) obstruction.

<h3 id="3g/ii">ii</h3>

↑ **Parent:** [3G](#3g)

<h4 id="3g/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3g/ii)

The domains are not [conformally equivalent](../../../geometry-and-topology.md#conformal-equivalence). If $F:\mathbb C\to\mathbb H$ were a conformal equivalence, composing it with a [Cayley transform](../../../geometry-and-topology.md#cayley-transform-hyperbolic-geometry) from the upper half-plane $\mathbb H$ to the unit disc would produce a bounded nonconstant [entire function](../../../complex-analysis.md#entire-function). This contradicts the [Liouville theorem](../../../complex-analysis.md#liouville-theorem), proving that the [complex plane is not conformally equivalent to the upper half-plane](../../../geometry-and-topology.md#complex-plane-is-not-conformally-equivalent-to-the-upper-half-plane).

<h3 id="3g/iii">iii</h3>

↑ **Parent:** [3G](#3g)

<h4 id="3g/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3g/iii)

The domains are [conformally equivalent](../../../geometry-and-topology.md#conformal-equivalence). The [Möbius transformation](../../../group-theory.md#mobius-transformation)

$$
T(z)=\frac{1+z}{1-z}
$$

maps the upper half of the unit disc onto the first quadrant: its diameter $(-1,1)$ maps to the positive real axis and its upper semicircle maps to the positive imaginary axis. Squaring maps the first quadrant bijectively and conformally onto the upper half-plane. Therefore

$$
\boxed{F(z)=\left(\frac{1+z}{1-z}\right)^2}
$$

is the required equivalence, as recorded by the [conformal equivalence between the upper half-disc and upper half-plane](../../../geometry-and-topology.md#conformal-equivalence-between-the-upper-half-disc-and-upper-half-plane).

## 4D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4d/a">a</h3>

↑ **Parent:** [4D](#4d)

<h4 id="4d/a/solution">Solution</h4>

↑ **Parent:** [A](#4d/a)

Write the [expectation value](../../../quantum-mechanics.md#expectation-value) as

$$
\langle O\rangle_\psi=\langle\psi|O|\psi\rangle.
$$

Differentiating and retaining the possible explicit time dependence of the [observable](../../../quantum-mechanics.md#observable) gives

$$
\frac d{dt}\langle O\rangle_\psi
=\langle\dot\psi|O|\psi\rangle
+\left\langle\psi\middle|\frac{\partial O}{\partial t}\middle|\psi\right\rangle
+\langle\psi|O|\dot\psi\rangle.
$$

The [Schrödinger equation](../../../physics.md#schrodinger-equation) and its adjoint are

$$
i\hbar|\dot\psi\rangle=H|\psi\rangle,
\qquad
-i\hbar\langle\dot\psi|=\langle\psi|H,
$$

where the [Hamiltonian operator](../../../quantum-mechanics.md#hamiltonian-quantum-mechanics) is Hermitian. Substitution yields

$$
\begin{aligned}
\frac d{dt}\langle O\rangle_\psi
&=\frac i\hbar\langle\psi|HO|\psi\rangle
-\frac i\hbar\langle\psi|OH|\psi\rangle
+\left\langle\frac{\partial O}{\partial t}\right\rangle_\psi\\
&=\boxed{\frac i\hbar\langle[H,O]\rangle_\psi
+\left\langle\frac{\partial O}{\partial t}\right\rangle_\psi}.
\end{aligned}
$$

This is the [proof of Ehrenfest theorem from the Schrodinger equation](../../../quantum-mechanics.md#proof-of-ehrenfest-theorem-from-the-schrodinger-equation).

<h3 id="4d/b">b</h3>

↑ **Parent:** [4D](#4d)

<h4 id="4d/b/solution">Solution</h4>

↑ **Parent:** [B](#4d/b)

For a particle in the scalar [potential energy](../../../classical-mechanics.md#potential-energy) $U(x)$,

$$
H=\frac{p^2}{2m}+U(x).
$$

The [canonical commutation relation](../../../quantum-mechanics.md#canonical-commutation-relation) $[x,p]=i\hbar$ gives

$$
[H,x]=\frac1{2m}[p^2,x]=-\frac{i\hbar}{m}p.
$$

The [Ehrenfest theorem](../../../quantum-mechanics.md#ehrenfest-theorem) with $O=x$ therefore gives

$$
\boxed{m\frac d{dt}\langle x\rangle_\psi=\langle p\rangle_\psi}.
$$

Since $[p^2,p]=0$ and direct action on a [wavefunction](../../../quantum-mechanics.md#wave-function) gives $[U(x),p]=i\hbar U'(x)$,

$$
\boxed{\frac d{dt}\langle p\rangle_\psi
=-\langle U'(x)\rangle_\psi}.
$$

Finally $H$ has no explicit time dependence and $[H,H]=0$, so

$$
\boxed{\frac d{dt}\langle H\rangle_\psi=0}.
$$

The first two equations are the expectation-value counterparts of momentum equals mass times velocity and [Newton's second law](../../../classical-mechanics.md#newton-s-second-law); the last is [conservation of energy](../../../physics.md#conservation-of-energy). They become the classical equations directly when the force varies negligibly across the wave packet, so that $\langle U'(x)\rangle\simeq U'(\langle x\rangle)$. These conclusions are summarized by the [classical equations from Ehrenfest theorem](../../../quantum-mechanics.md#classical-equations-from-ehrenfest-theorem).

## 5D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5d/a">a</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/a/solution">Solution</h4>

↑ **Parent:** [A](#5d/a)

Let $\theta$ be the angle between $r$ and the positive $z$-axis. By superposition of the [electric potential](../../../electromagnetism.md#electric-potential) of point charges,

$$
\Phi(r)=\frac{Q}{4\pi\epsilon_0}
\left(\frac N r-\frac1{|r-d\widehat z|}
-\frac M{|r+d\widehat z|}\right).
$$

For $r>d$, the [Legendre polynomial](../../../differential-equation.md#legendre-polynomial) expansion gives

$$
\frac1{|r\mp d\widehat z|}
=\frac1r\left[1\pm\frac d r\cos\theta
+\frac{d^2}{2r^2}(3\cos^2\theta-1)+O(r^{-3})\right].
$$

Therefore

$$
\boxed{\Phi(r,\theta)=\frac{Q}{4\pi\epsilon_0}\left[
\frac{N-M-1}{r}
+\frac{(M-1)d\cos\theta}{r^2}
-\frac{(M+1)d^2(3\cos^2\theta-1)}{2r^3}
+O(r^{-4})\right]}.
$$

The three displayed terms are respectively the monopole, dipole, and quadrupole terms of the [electric multipole expansion](../../../electromagnetism.md#electric-multipole-expansion). In particular, the total charge is $Q(N-M-1)$ and the [electric dipole moment](../../../electromagnetism.md#electric-dipole-moment) is $Qd(M-1)\widehat z$. This is the [multipole expansion of three collinear charges](../../../electromagnetism.md#multipole-expansion-of-three-collinear-charges).

<h3 id="5d/b">b</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/b/solution">Solution</h4>

↑ **Parent:** [B](#5d/b)

The monopole vanishes exactly when

$$
\boxed{N=M+1},
$$

and the dipole vanishes exactly when

$$
\boxed{M=1}.
$$

Since $N$ and $M$ are positive integers, both vanish precisely for

$$
\boxed{N=2,\qquad M=1}.
$$

Assume now that the monopole has been cancelled. If $Qd$ is held fixed while $d\to0$, the quadrupole coefficient $Qd^2=(Qd)d$ tends to zero, whereas the dipole coefficient $(M-1)Qd$ has a finite limit. For $M\ne1$ this is a point-dipole limit; for $M=1$ the limiting external potential vanishes.

If instead $Qd^2$ is held fixed, the dipole coefficient is

$$
(M-1)Qd=(M-1)\frac{Qd^2}{d}.
$$

It diverges unless $M=1$. When $M=1$ and $N=2$, both lower multipoles vanish and the quadrupole coefficient has a finite nonzero limit. These are the [dipole and quadrupole scaling limits of three collinear charges](../../../electromagnetism.md#dipole-and-quadrupole-scaling-limits-of-three-collinear-charges).

<h3 id="5d/c">c</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/c/solution">Solution</h4>

↑ **Parent:** [C](#5d/c)

Here $N=2$ and $M=1$. At $(x,0,0)$, the $z$-components of the fields of the two outer charges cancel by reflection symmetry. By [Coulomb's law](../../../electromagnetism.md#coulomb-s-law), the remaining field is

$$
E_x=\frac{2Qx}{4\pi\epsilon_0}
\left(\frac1{|x|^3}-\frac1{(x^2+d^2)^{3/2}}\right).
$$

Multiplying by the test charge $-Q$ gives

$$
\boxed{F=-\frac{Q^2x}{2\pi\epsilon_0}
\left(\frac1{|x|^3}-\frac1{(x^2+d^2)^{3/2}}\right)\widehat x}.
$$

The quantity in parentheses is positive. Thus for $x>0$ the force points in the negative $x$ direction, while for $x<0$ it points in the positive $x$ direction. It is always attractive toward the origin, as in the [transverse force from a collinear electric quadrupole](../../../electromagnetism.md#transverse-force-from-a-collinear-electric-quadrupole).

## 6B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="6b/a">a</h3>

↑ **Parent:** [6B](#6b)

<h4 id="6b/a/solution">Solution</h4>

↑ **Parent:** [A](#6b/a)

The nonzero [orthogonal polynomials](../../../numerical-analysis.md#orthogonal-polynomial) $Q_0,\ldots,Q_n$ have distinct degrees and form an orthogonal basis of $\mathcal P_n$. Define

$$
p_n^*=\sum_{k=0}^n
\frac{\langle f,Q_k\rangle}{\langle Q_k,Q_k\rangle}Q_k.
$$

For each $j\leq n$,

$$
\langle f-p_n^*,Q_j\rangle
=\langle f,Q_j\rangle
-\frac{\langle f,Q_j\rangle}{\langle Q_j,Q_j\rangle}
\langle Q_j,Q_j\rangle=0.
$$

Thus the residual $f-p_n^*$ is [orthogonal](../../../linear-algebra.md#orthogonal-vectors) to all of $\mathcal P_n$.

For any $p\in\mathcal P_n$, write

$$
f-p=(f-p_n^*)+(p_n^*-p).
$$

The two terms are orthogonal, so the [Pythagorean theorem in an inner-product space](../../../linear-algebra.md#pythagorean-theorem-in-an-inner-product-space) gives

$$
\lVert f-p\rVert^2
=\lVert f-p_n^*\rVert^2+\lVert p_n^*-p\rVert^2
\geq\lVert f-p_n^*\rVert^2.
$$

Equality holds only for $p=p_n^*$. This proves the formula and uniqueness of the [least-squares polynomial in an orthogonal-polynomial basis](../../../linear-algebra.md#least-squares-polynomial-in-an-orthogonal-polynomial-basis).

<h3 id="6b/b">b</h3>

↑ **Parent:** [6B](#6b)

<h4 id="6b/b/solution">Solution</h4>

↑ **Parent:** [B](#6b/b)

Part (a) shows that $f-p_n^*$ is orthogonal to $p_n^*\in\mathcal P_n$. Since

$$
f=(f-p_n^*)+p_n^*,
$$

the [Pythagorean theorem in an inner-product space](../../../linear-algebra.md#pythagorean-theorem-in-an-inner-product-space) immediately gives

$$
\boxed{\lVert f\rVert^2
=\lVert f-p_n^*\rVert^2+\lVert p_n^*\rVert^2}.
$$

This is the norm decomposition associated with [orthogonal projection onto a finite-dimensional subspace](../../../linear-algebra.md#orthogonal-projection-onto-a-finite-dimensional-subspace).

## 7H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="7h/a">a</h3>

↑ **Parent:** [7H](#7h)

<h4 id="7h/a/solution">Solution</h4>

↑ **Parent:** [A](#7h/a)

Let $g(0)=0$. [First-step analysis](../../../analysis.md#first-step-analysis) gives

$$
 g(1)=1+\frac12g(2),
$$



$$
 g(2)=1+\frac12g(1)+\frac12g(3),
$$

and, because state $3$ moves to $2$ or remains at $3$ with equal probabilities,

$$
 g(3)=1+\frac12g(2)+\frac12g(3).
$$

The last equation gives $g(3)=2+g(2)$. Substitution into the second gives $g(2)=4+g(1)$, and the first then gives $g(1)=3+g(1)/2$. Hence

$$
\boxed{g(1)=6,\qquad g(2)=10,\qquad g(3)=12}.
$$

These are the [expected hitting times](../../../markov-process.md#expected-hitting-time) of the absorbing state.

<h3 id="7h/b">b</h3>

↑ **Parent:** [7H](#7h)

<h4 id="7h/b/solution">Solution</h4>

↑ **Parent:** [B](#7h/b)

Let $h(i)$ be the probability of reaching state $3$ before state $0$. The boundary values are $h(0)=0$ and $h(3)=1$. [First-step analysis](../../../analysis.md#first-step-analysis) at states $1$ and $2$ gives

$$
h(1)=\frac12h(2),
\qquad
h(2)=\frac12h(1)+\frac12.
$$

Therefore $h(1)=h(1)/4+1/4$, so the requested [hitting probability](../../../markov-process.md#hitting-probability) is

$$
\boxed{h(1)=\frac13}.
$$

<h3 id="7h/c">c</h3>

↑ **Parent:** [7H](#7h)

<h4 id="7h/c/solution">Solution</h4>

↑ **Parent:** [C](#7h/c)

Let $u(i)$ be the expected number of visits to state $3$ before absorption, counting the present state when $i=3$. Its reward equations are

$$
u(0)=0,
\qquad
u(1)=\frac12u(2),
$$



$$
u(2)=\frac12u(1)+\frac12u(3),
\qquad
u(3)=1+\frac12u(2)+\frac12u(3).
$$

The last equation gives $u(3)=2+u(2)$, so the second nontrivial equation gives $u(2)=2+u(1)$. Hence $u(1)=1+u(1)/2$, and

$$
\boxed{u(1)=2}.
$$

**Thus the expected occupation count is two; together with the previous parts, this is the [four-state reflecting absorbing random walk](../../../markov-process.md#four-state-reflecting-absorbing-random-walk) calculation.**

## 8F

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="8f/solution">Solution</h3>

↑ **Parent:** [8F](#8f)

For ordered bases $\mathcal B=(v_1,\ldots,v_n)$ of $V$ and $\mathcal C=(w_1,\ldots,w_m)$ of $W$, the [matrix representation of a linear map](../../../vector-space.md#matrix-representation-of-a-linear-map) $\gamma:V\to W$ is the matrix whose $j$th column consists of the $\mathcal C$-coordinates of $\gamma(v_j)$. Thus

$$
[\gamma(v)]_{\mathcal C}
=[\gamma]_{\mathcal C\leftarrow\mathcal B}[v]_{\mathcal B}.
$$

The operators $\alpha,\beta:V\to V$ are [conjugate linear operators](../../../vector-space.md#conjugate-linear-operators) when there is an isomorphism $s:V\to V$ such that

$$
\beta=s^{-1}\alpha s.
$$

In one basis their matrices therefore satisfy $[\beta]=[s]^{-1}[\alpha][s]$, so they are similar matrices.

For invertible $\beta$, the map

$$
\phi_\beta(A)=\beta^{-1}A\beta
$$

is linear, and its inverse is $A\mapsto\beta A\beta^{-1}$; hence it is a linear isomorphism of $\operatorname{End}(V)$. If $\beta'=s^{-1}\beta s$, define $\Phi_s(A)=s^{-1}As$. A direct substitution gives

$$
\phi_{\beta'}=\Phi_s\phi_\beta\Phi_s^{-1},
$$

so $\phi_{\beta'}$ and $\phi_\beta$ are conjugate. This is the [conjugation operator on an endomorphism space](../../../vector-space.md#conjugation-operator-on-an-endomorphism-space).

It remains to compute the [Jordan normal form](../../../linear-operator-theory.md#jordan-normal-form) over $\mathbb C$. By the preceding conjugacy, we may put $\beta$ in Jordan form.

If

$$
\beta=\begin{pmatrix}\lambda&0\\0&\mu\end{pmatrix},
\qquad \lambda\mu\ne0,
$$

then the matrix units $E_{ij}$ are eigenvectors because

$$
\phi_\beta(E_{ij})=\frac{\beta_j}{\beta_i}E_{ij}.
$$

Thus

$$
\boxed{\operatorname{JNF}(\phi_\beta)
=\operatorname{diag}\left(1,1,\frac\mu\lambda,\frac\lambda\mu\right)}.
$$

This includes the scalar case $\lambda=\mu$, when $\phi_\beta$ is the identity.

Otherwise $\beta$ has one size-two [Jordan block](../../../linear-operator-theory.md#jordan-block). Multiplying $\beta$ by a nonzero scalar does not change $\phi_\beta$, and conjugating within its Jordan class allows us to use $J=I+N$ with $N=E_{12}$. Put $D=\phi_J-I$. Direct multiplication gives

$$
D(E_{11})=E_{12},\quad D(E_{12})=0,\quad
D(E_{22})=-E_{12},
$$



$$
D(E_{21})=E_{22}-E_{11}-E_{12}.
$$

Hence $D^3=0$, $\operatorname{rank}D=2$, and $\operatorname{rank}D^2=1$. The nilpotent Jordan blocks of $D$ therefore have sizes three and one. Adding the identity gives

$$
\boxed{\operatorname{JNF}(\phi_\beta)=J_3(1)\oplus J_1(1)}.
$$

These two cases are the [Jordan normal form of conjugation on two-by-two matrices](../../../linear-operator-theory.md#jordan-normal-form-of-conjugation-on-two-by-two-matrices).

## 9E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="9e/solution">Solution</h3>

↑ **Parent:** [9E](#9e)

Let

$$
F(X)=a_nX^n+\cdots+a_1X+a_0\in\mathbb Z[X]
$$

be a [primitive polynomial](../../../commutative-algebra.md#primitive-polynomial). The [Eisenstein criterion](../../../commutative-algebra.md#eisenstein-criterion) states that if a [prime number](../../../number-theory.md#prime-number) $p$ satisfies

$$
p\nmid a_n,\qquad p\mid a_j\ (0\leq j<n),\qquad p^2\nmid a_0,
$$

then $F$ is an [irreducible polynomial](../../../polynomial.md#irreducible-polynomial) in $\mathbb Z[X]$, equivalently in $\mathbb Q[X]$ by [Gauss lemma for polynomials](../../../commutative-algebra.md#gauss-lemma-for-polynomials).

To prove it, suppose that $F=GH$ with $G,H\in\mathbb Z[X]$ of positive degree. Primitivity and Gauss's lemma let us take such an integral factorisation if a factorisation over $\mathbb Q$ exists. Reducing modulo $p$ gives

$$
\overline G\,\overline H=\overline{a_n}X^n.
$$

Because $p$ does not divide the leading coefficient of $F$, neither factor loses degree on reduction. The polynomial ring $\mathbb F_p[X]$ is a [unique factorization domain](../../../algebra.md#unique-factorization-domain), so both reductions are monomials of positive degree. In particular, $p$ divides both constant terms $G(0)$ and $H(0)$. It follows that $p^2$ divides

$$
F(0)=G(0)H(0)=a_0,
$$

a contradiction. This proves the criterion.

For a prime $p$, translate the geometric sum by one:

$$
f(X+1)=\frac{(X+1)^p-1}{X}
=\sum_{k=1}^{p}\binom pk X^{k-1}.
$$

Its leading coefficient is one, every other coefficient is divisible by $p$, and its constant coefficient is $p$, which is not divisible by $p^2$. It is therefore Eisenstein at $p$. Translation $X\mapsto X+1$ is an automorphism of $\mathbb Z[X]$, so

$$
\boxed{f(X)=1+X+\cdots+X^{p-1}\text{ is irreducible}.}
$$

This is the [geometric-sum irreducibility criterion](../../../commutative-algebra.md#geometric-sum-irreducibility-criterion).

The [evaluation homomorphism](../../../commutative-algebra.md#evaluation-homomorphism)

$$
\operatorname{ev}_\zeta:\mathbb Z[X]\longrightarrow\mathbb C,
\qquad G\longmapsto G(\zeta),
$$

has image $\mathbb Z[\zeta]$ and contains $(f)$ in its kernel. Since $f$ is monic, division by $f$ in $\mathbb Z[X]$ writes every $G$ as $G=Qf+R$ with $\deg R<\deg f$. If $G(\zeta)=0$, then $R(\zeta)=0$; the irreducibility of $f$ says that $f$ is the [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) of $\zeta$, so $R=0$. Thus $\ker(\operatorname{ev}_\zeta)=(f)$, and the [first isomorphism theorem for rings](../../../commutative-algebra.md#first-isomorphism-theorem-for-rings) gives

$$
\boxed{\mathbb Z[\zeta]\cong\mathbb Z[X]/(f)}.
$$

Now take $p=3$. Then $\zeta^2+\zeta+1=0$, and the [Eisenstein integers](../../../commutative-algebra.md#eisenstein-integer) are

$$
\mathbb Z[\zeta]=\{a+b\zeta:a,b\in\mathbb Z\}.
$$

Complex conjugation sends $\zeta$ to $\zeta^2$, so the [field norm](../../../algebraic-number-theory.md#field-norm) is

$$
N(a+b\zeta)=(a+b\zeta)(a+b\zeta^2)=a^2-ab+b^2=|a+b\zeta|^2.
$$

Given $z=x+y\zeta\in\mathbb C$, choose integers $m,n$ with $|x-m|,|y-n|\leq\tfrac12$. For $q=m+n\zeta$,

$$
|z-q|^2=(x-m)^2-(x-m)(y-n)+(y-n)^2\leq\frac34<1.
$$

For $\alpha,\beta\in\mathbb Z[\zeta]$ with $\beta\ne0$, apply this to $z=\alpha/\beta$ and put $r=\alpha-q\beta$. Then

$$
N(r)=N(\beta)|z-q|^2<N(\beta).
$$

Hence the norm is a [Euclidean function](../../../commutative-algebra.md#euclidean-function), proving that $\mathbb Z[\zeta]$ is a [Euclidean domain](../../../commutative-algebra.md#euclidean-domain). This is the [Euclidean norm on the Eisenstein integers](../../../commutative-algebra.md#euclidean-norm-on-the-eisenstein-integers).

Finally suppose $A\in\mathrm{GL}_n(\mathbb Z)$ satisfies $A^2+A+I=0$. Make the free abelian group $M=\mathbb Z^n$ into a $\mathbb Z[\zeta]$-module by defining

$$
\zeta v=Av.
$$

This is well-defined precisely because $A$ obeys the same polynomial relation as $\zeta$. The module is finitely generated. It is also [torsion-free module](../../../module-theory.md#torsion-free-module): if $0\ne\alpha\in\mathbb Z[\zeta]$ and $\alpha v=0$, multiplication by the conjugate of $\alpha$ gives $N(\alpha)v=0$, and the additive group $\mathbb Z^n$ has no nonzero integer torsion.

A Euclidean domain is a [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain), and the [structure theorem for finitely generated modules over a principal ideal domain](../../../module-theory.md#structure-theorem-for-finitely-generated-modules-over-a-principal-ideal-domain) says that a finitely generated torsion-free module over one is free. Thus

$$
M\cong\mathbb Z[\zeta]^m
$$

for some $m$. Since $\mathbb Z[\zeta]$ has [free module](../../../module-theory.md#free-module) basis $1,\zeta$ over $\mathbb Z$, comparison of abelian ranks gives $n=2m$. There can consequently be no such matrix when $n$ is odd.

If $n=2m$, choose a $\mathbb Z[\zeta]$-basis $v_1,\ldots,v_m$. Then

$$
v_1,Av_1,\ldots,v_m,Av_m
$$

is a $\mathbb Z$-basis, and $A^2v_i=-v_i-Av_i$. In this basis the matrix of $A$ is a direct sum of $m$ copies of

$$
C=\begin{pmatrix}0&-1\\1&-1\end{pmatrix}.
$$

Every admissible matrix is therefore conjugate in $\mathrm{GL}_n(\mathbb Z)$ to $C^{\oplus m}$. Hence there is exactly one conjugacy class for even $n$, and none for odd $n$. This is the [classification of integral matrices satisfying the third cyclotomic polynomial](../../../module-theory.md#classification-of-integral-matrices-satisfying-the-third-cyclotomic-polynomial).

## 10G

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="10g/i">i</h3>

↑ **Parent:** [10G](#10g)

<h4 id="10g/i/solution">Solution</h4>

↑ **Parent:** [I](#10g/i)

A [compact space](../../../topology.md#compact-space) is a [topological space](../../../topology.md#topological-space) in which every [open cover](../../../topology.md#open-cover) has a finite subcover. A [Hausdorff space](../../../topology.md#hausdorff-space) is one in which every two distinct points have disjoint open neighbourhoods. A [homeomorphism](../../../topology.md#homeomorphism) is a bijection that is continuous and whose inverse is continuous.

For an [equivalence relation](../../../set-theory.md#equivalence-relation) $R$ on $X$, let $X/R$ be the set of equivalence classes and let

$$
q:X\longrightarrow X/R,
\qquad q(x)=[x].
$$

The [quotient topology](../../../topology.md#quotient-topology) declares $U\subseteq X/R$ open exactly when $q^{-1}(U)$ is open in $X$. It follows directly from the definition that $q$ is continuous.

Suppose that the continuous map $f:X\to Y$ is constant on equivalence classes. The only possible factorisation is

$$
F:X/R\longrightarrow Y,
\qquad F([x])=f(x),
$$

which is well-defined by the hypothesis and satisfies $F\circ q=f$. For every open $V\subseteq Y$,

$$
q^{-1}(F^{-1}(V))=f^{-1}(V)
$$

is open in $X$. The definition of the quotient topology therefore makes $F^{-1}(V)$ open, so $F$ is continuous. This proves the [universal property of the quotient topology](../../../topology.md#universal-property-of-the-quotient-topology).

<h3 id="10g/ii">ii</h3>

↑ **Parent:** [10G](#10g)

<h4 id="10g/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#10g/ii)

Let $X$ be [compact](../../../topology.md#compact-space) and $q:X\to X/R$ the quotient map. If $(U_i)_{i\in I}$ is an open cover of $X/R$, then $(q^{-1}(U_i))_{i\in I}$ is an open cover of $X$. A finite subfamily covers $X$; because $q$ is surjective, the corresponding $U_i$ cover $X/R$. Thus every quotient of a compact space is compact.

The Hausdorff property need not survive. On the [real line](../../../real-analysis.md#real-line), define

$$
xRy\quad\Longleftrightarrow\quad x-y\in\mathbb Q.
$$

The quotient $\mathbb R/\mathbb Q$ has more than one point. If two nonempty open subsets of the quotient were disjoint, their inverse images would be disjoint nonempty open subsets of $\mathbb R$ invariant under rational translation. But any two nonempty open intervals acquire an intersection after one is translated by a suitably chosen rational number, so two such saturated open sets cannot be disjoint. Distinct quotient points cannot be separated, and the quotient is not Hausdorff. This is the [non-Hausdorff quotient of the real line by rational translation](../../../topology.md#non-hausdorff-quotient-of-the-real-line-by-rational-translation).

Finally let $f:X\to Y$ be a continuous bijection, with $X$ compact and $Y$ Hausdorff. Every closed subset $C\subseteq X$ is compact. Its continuous image $f(C)$ is compact, and every compact subset of a Hausdorff space is closed. Hence $f$ is a [closed map](../../../topology.md#closed-map). For every closed $C\subseteq X$,

$$
(f^{-1})^{-1}(C)=f(C)
$$

is closed in $Y$, so $f^{-1}$ is continuous. Therefore $f$ is a homeomorphism. This is the [compact-to-Hausdorff continuous bijection theorem](../../../topology.md#compact-to-hausdorff-continuous-bijection-theorem).

<h3 id="10g/iii">iii</h3>

↑ **Parent:** [10G](#10g)

<h4 id="10g/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#10g/iii)

Define

$$
f:[0,1]^2\longrightarrow S^2,
$$



$$
f(x,y)=\bigl(\sin(\pi y)\cos(2\pi x),
\sin(\pi y)\sin(2\pi x),\cos(\pi y)).
$$

This is continuous and takes values on the [unit sphere](../../../topology.md#unit-sphere). It agrees at $(0,y)$ and $(1,y)$, is constant on the bottom edge, and is constant on the top edge. Thus it is constant on every $R$-class, so the [universal property of the quotient topology](../../../topology.md#universal-property-of-the-quotient-topology) gives a continuous map

$$
\overline f:X/R\longrightarrow S^2.
$$

For $0<y<1$, the third coordinate $\cos(\pi y)$ determines $y$, and the first two coordinates determine $x$ modulo one. Consequently the only equal values of $f$ in the open strip arise from $x=0$ and $x=1$. At $y=0$ the whole edge maps to the north pole, and at $y=1$ the whole edge maps to the south pole. These are exactly the identifications defining $R$, so $\overline f$ is injective. The spherical-coordinate formula also shows that it is surjective.

The square is compact, hence its quotient $X/R$ is compact by part (ii), while $S^2$ is Hausdorff as a subspace of $\mathbb R^3$. The [compact-to-Hausdorff continuous bijection theorem](../../../topology.md#compact-to-hausdorff-continuous-bijection-theorem) now makes $\overline f$ a homeomorphism. Geometrically, identifying the vertical sides produces a cylinder and collapsing each boundary circle to a point produces the [suspension of a topological space](../../../algebraic-topology.md#suspension-topology) $S^1$, which is $S^2$. This proves the [square quotient model of the two-sphere](../../../topology.md#square-quotient-model-of-the-two-sphere).

## 11E

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="11e/a">a</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/a/solution">Solution</h4>

↑ **Parent:** [A](#11e/a)

Let

$$
J(z)=\frac1{\overline z}
$$

be reflection in the unit circle, and represent a [Möbius transformation](../../../group-theory.md#mobius-transformation) $g$ by

$$
M=\begin{pmatrix}\alpha&\beta\\ \gamma&\delta\end{pmatrix}.
$$

A direct calculation shows that $JgJ$ is represented by

$$
\tau(M)=\begin{pmatrix}\overline\delta&\overline\gamma\\
\overline\beta&\overline\alpha\end{pmatrix}.
$$

Thus $gJ=Jg$ exactly when $M$ and $\tau(M)$ differ by a nonzero scalar. Applying the conjugate-linear involution $\tau$ twice shows that this scalar has [modulus](../../../complex-analysis.md#modulus) one. Rescaling $M$ by a suitable complex scalar then makes $M=\tau(M)$. Consequently all commuting maps, and only those maps, have the form

$$
\boxed{g(z)=\frac{az+b}{\overline b z+\overline a}},
\qquad |a|^2-|b|^2\ne0.
$$

This is the [Möbius maps commuting with reflection in the unit circle](../../../group-theory.md#mobius-maps-commuting-with-reflection-in-the-unit-circle) classification.

For such a map,

$$
|az+b|^2-|\overline b z+\overline a|^2
=(|a|^2-|b|^2)(|z|^2-1).
$$

It follows that $|g(z)|<1$ whenever $|z|<1$ precisely when

$$
\boxed{|a|>|b|}.
$$

The inverse has the same property, so these and only these maps preserve the unit disc.

<h3 id="11e/b">b</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/b/solution">Solution</h4>

↑ **Parent:** [B](#11e/b)

The [Poincare disc model](../../../geometry-and-topology.md#poincare-disk-model) is

$$
\mathbb D=\{z=x+iy:|z|<1\},
\qquad
ds^2=\frac{4(dx^2+dy^2)}{(1-|z|^2)^2}.
$$

Its geodesics through the origin are the Euclidean diameters. To see directly that the radial segment from $0$ to $re^{i\theta_0}$ minimizes length, write an arbitrary joining curve as $z(t)=r(t)e^{i\theta(t)}$. Its [hyperbolic length](../../../geometry-and-topology.md#hyperbolic-length-in-the-poincare-disc) satisfies

$$
\begin{aligned}
L
&=\int\frac{2\sqrt{\dot r^{\,2}+r^2\dot\theta^{\,2}}}{1-r^2}\,dt\\
&\geq\int\frac{2|\dot r|}{1-r^2}\,dt
\geq2\operatorname{artanh}r.
\end{aligned}
$$

The radial segment has constant $\theta$ and monotone $r$, so equality holds. Hence

$$
\boxed{d_{\mathbb D}(0,z)=2\operatorname{artanh}|z|}
$$

and every radial diameter is length minimizing. Rotational symmetry and uniqueness for the [geodesic equation](../../../riemannian-geometry.md#geodesic-equation) show that these are all geodesics through $0$.

Given any geodesic and a point $p$ on it, a disc-preserving map

$$
T(z)=e^{i\varphi}\frac{z-p}{1-\overline pz}
$$

takes $p$ to the origin. By part (a), $T$ is a hyperbolic isometry and commutes with $J(z)=1/\overline z$. The transformed geodesic is a diameter, hence a generalized circle invariant under $J$. Its inverse image is therefore also a [Generalized circle under a Möbius transformation](../../../group-theory.md#generalized-circle-under-a-mobius-transformation) invariant under $J$. Thus every hyperbolic geodesic is the part in $\mathbb D$ of a Euclidean line or circle preserved by reflection in the unit circle; equivalently, it is a diameter or a circle orthogonal to the unit circle. This is the [Geodesics of the Poincare disc](../../../geometry-and-topology.md#geodesics-of-the-poincare-disc) description.

<h3 id="11e/c">c</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/c/solution">Solution</h4>

↑ **Parent:** [C](#11e/c)

Rotate the disc so that $P=r\in(0,1)$ lies on the positive real axis. From part (b), the perpendicular hyperbolic line $\ell$ is a Euclidean circle orthogonal to the unit circle, with centre $c>1$ on the real axis and radius $R=c-r$. Orthogonality of the two circles gives

$$
c^2=1+R^2.
$$

Combining the two equations yields

$$
c=\frac{1+r^2}{2r},
\qquad
R=\frac{1-r^2}{2r}.
$$

The radial distance formula from part (b) says

$$
\rho=2\operatorname{artanh}r,
\qquad r=\tanh(\rho/2).
$$

The hyperbolic double-angle identities now give

$$
\sinh\rho=\frac{2r}{1-r^2},
\qquad
\tanh\rho=\frac{2r}{1+r^2}.
$$

Therefore

$$
\boxed{R=\frac1{\sinh\rho},
\qquad c=\frac1{\tanh\rho}}.
$$

This is the [Euclidean circle representing a perpendicular hyperbolic line](../../../geometry-and-topology.md#euclidean-circle-representing-a-perpendicular-hyperbolic-line).

<h3 id="11e/d">d</h3>

↑ **Parent:** [11E](#11e)

<h4 id="11e/d/solution">Solution</h4>

↑ **Parent:** [D](#11e/d)

Use the [hyperboloid model](../../../geometry-and-topology.md#hyperboloid-model) with [Minkowski inner product](../../../geometry-and-topology.md#minkowski-inner-product)

$$
\langle x,y\rangle_M=-x_0y_0+x_1y_1+x_2y_2.
$$

Put the vertex with angle $\theta$ at $v=(1,0,0)$, and place the endpoints of its adjacent sides of lengths $a$ and $b$ at

$$
P=(\cosh a,\sinh a,0),
$$



$$
Q=(\cosh b,\sinh b\cos\theta,
\sinh b\sin\theta).
$$

The geodesic through $P$ perpendicular to $vP$ has spacelike unit normal

$$
n_P=(\sinh a,\cosh a,0),
$$

while the geodesic through $Q$ perpendicular to $vQ$ has spacelike unit normal

$$
n_Q=(\sinh b,\cosh b\cos\theta,
\cosh b\sin\theta).
$$

These two geodesics form the remaining two sides of the quadrilateral. Their angle equals the angle between their normals in the tangent plane at their intersection. The third right angle therefore gives

$$
0=\langle n_P,n_Q\rangle_M
=-\sinh a\sinh b+\cosh a\cosh b\cos\theta.
$$

Dividing by $\cosh a\cosh b$ proves the [Lambert quadrilateral identity](../../../geometry-and-topology.md#lambert-quadrilateral)

$$
\boxed{\cos\theta=\tanh a\tanh b}.
$$

## 12B

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="12b/a">a</h3>

↑ **Parent:** [12B](#12b)

<h4 id="12b/a/solution">Solution</h4>

↑ **Parent:** [A](#12b/a)

Because the [matrix-valued Laplace transform](../../../analysis.md#matrix-valued-laplace-transform) is taken componentwise, for every $i,j$ we have

$$
\begin{aligned}
\bigl(\mathcal L\{AB\}(s))_{ij}
&=\int_0^\infty e^{-st}\sum_{k=1}^n A_{ik}B_{kj}(t)\,dt\\
&=\sum_{k=1}^n A_{ik}\int_0^\infty e^{-st}B_{kj}(t)\,dt\\
&=\bigl(A\mathcal L\{B\}(s))_{ij}.
\end{aligned}
$$

The sum is finite and $A$ is constant, so it may be moved outside the integral. Therefore

$$
\boxed{\mathcal L\{AB\}=A\mathcal L\{B\}}.
$$

<h3 id="12b/b">b</h3>

↑ **Parent:** [12B](#12b)

<h4 id="12b/b/solution">Solution</h4>

↑ **Parent:** [B](#12b/b)

Taking the [Laplace transform](../../../analysis.md#laplace-transform) of the differential equation and using

$$
\mathcal L\{y'\}(s)=sY(s)-y(0)
$$

gives

$$
sY-y_0=AY+G.
$$

Hence

$$
(sI-A)Y=y_0+G.
$$

Whenever $s$ is not an [eigenvalue](../../../linear-operator-theory.md#eigenvalue) of $A$, the matrix $sI-A$ is invertible, and thus

$$
\boxed{Y(s)=(sI-A)^{-1}(y_0+G(s))}.
$$

This is the [Laplace-transform solution of a constant-coefficient vector ODE](../../../analysis.md#laplace-transform-solution-of-a-constant-coefficient-vector-ode).

Set $g=0$. The given homogeneous solution is $y(t)=e^{tA}y_0$, so the preceding formula says

$$
\mathcal L\{e^{tA}\}(s)y_0=(sI-A)^{-1}y_0
$$

for every initial vector $y_0$. Equality on every vector gives the matrix identity

$$
\boxed{\mathcal L\{e^{tA}\}(s)=(sI-A)^{-1}},
$$

on the common domain of convergence and in particular away from the eigenvalues of $A$. This is the [Laplace transform of a matrix exponential](../../../linear-operator-theory.md#laplace-transform-of-a-matrix-exponential).

<h3 id="12b/c">c</h3>

↑ **Parent:** [12B](#12b)

<h4 id="12b/c/solution">Solution</h4>

↑ **Parent:** [C](#12b/c)

The coefficient matrix has [eigenvector](../../../linear-operator-theory.md#eigenvector) $u_+=(1,1)^T$ with eigenvalue $3$ and eigenvector $u_-=(1,-1)^T$ with eigenvalue $-1$. Write

$$
y(t)=p(t)u_++q(t)u_-.
$$

Since

$$
\begin{pmatrix}e^{2t}\\-2t\end{pmatrix}
=\frac{e^{2t}-2t}{2}u_+
+\frac{e^{2t}+2t}{2}u_-,
$$

and $y(0)=(1,-2)^T=-\tfrac12u_++\tfrac32u_-$, the system diagonalises to

$$
p'=3p+\frac{e^{2t}-2t}{2},\qquad p(0)=-\frac12,
$$



$$
q'=-q+\frac{e^{2t}+2t}{2},\qquad q(0)=\frac32.
$$

Using an [integrating factor](../../../differential-equation.md#integrating-factor) gives

$$
p(t)=-\frac19e^{3t}-\frac12e^{2t}+\frac t3+\frac19,
$$



$$
q(t)=\frac16e^{2t}+t-1+\frac73e^{-t}.
$$

The unique fastest term is therefore

$$
y(t)=-\frac19e^{3t}u_++O(e^{2t}).
$$

Consequently $e^{-nt}y(t)$ diverges for $n<3$, tends to zero for $n>3$, and for $n=3$ tends to the finite nonzero vector

$$
\boxed{\lim_{t\to\infty}e^{-3t}y(t)
=-\frac19\begin{pmatrix}1\\1\end{pmatrix}}.
$$

Thus the only requested integer is

$$
\boxed{n=3}.
$$

This is an instance of [dominant eigenmode in a forced linear system](../../../differential-equation.md#dominant-eigenmode-in-a-forced-linear-system).

## 13C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="13c/a">a</h3>

↑ **Parent:** [13C](#13c)

<h4 id="13c/a/solution">Solution</h4>

↑ **Parent:** [A](#13c/a)

Let $u\mapsto u+\varepsilon\eta$ and $v\mapsto v+\varepsilon\xi$, where the variations vanish on the boundary. The [first variation](../../../calculus-of-variations.md#first-variation) is

$$
\begin{aligned}
\delta\mathcal L
=\iint_\Omega \bigl(&f_u\eta+f_v\xi
+f_{u_x}\eta_x+f_{u_y}\eta_y\\
&+f_{v_x}\xi_x+f_{v_y}\xi_y)\,dx\,dy.
\end{aligned}
$$

Applying [integration by parts](../../../calculus.md#integration-by-parts) to the four derivative terms and discarding the boundary contributions gives

$$
\delta\mathcal L=\iint_\Omega
\left(f_u-\frac{\partial f_{u_x}}{\partial x}
-\frac{\partial f_{u_y}}{\partial y}\right)\eta\,dx\,dy
$$



$$
{}+\iint_\Omega
\left(f_v-\frac{\partial f_{v_x}}{\partial x}
-\frac{\partial f_{v_y}}{\partial y}\right)\xi\,dx\,dy.
$$

The variations $\eta$ and $\xi$ are independent and arbitrary in the interior. The [fundamental lemma of the calculus of variations](../../../calculus-of-variations.md#fundamental-lemma-of-the-calculus-of-variations) therefore gives the two [Euler-Lagrange equations for two fields](../../../analysis.md#euler-lagrange-equations-for-two-fields)

$$
\boxed{f_u-\partial_x f_{u_x}-\partial_y f_{u_y}=0},
$$



$$
\boxed{f_v-\partial_x f_{v_x}-\partial_y f_{v_y}=0}.
$$

<h3 id="13c/b">b</h3>

↑ **Parent:** [13C](#13c)

<h4 id="13c/b/i">i</h4>

↑ **Parent:** [B](#13c/b)

<h5 id="13c/b/i/solution">Solution</h5>

↑ **Parent:** [I](#13c/b/i)

For the [displacement gradient tensor](../../../continuum-mechanics.md#displacement-gradient-tensor) specified in the question,

$$
\nabla\mathbf u:\nabla\mathbf u^T
=\operatorname{tr}(\nabla\mathbf u\,\nabla\mathbf u^T)
=u_x^2+u_y^2+v_x^2+v_y^2,
$$

while the [divergence](../../../calculus.md#divergence) is $\nabla\cdot\mathbf u=u_x+v_y$. Hence the [isotropic linear-elastic energy density](../../../continuum-mechanics.md#isotropic-linear-elastic-energy-density) is

$$
\frac\mu2(u_x^2+u_y^2+v_x^2+v_y^2)
+\frac{\lambda+\mu}{2}(u_x+v_y)^2.
$$

Expanding the square and collecting terms yields

$$
\boxed{
\mathcal J=\iint_\Omega\left[
\left(\frac\lambda2+\mu\right)(u_x^2+v_y^2)
+\frac\mu2(u_y^2+v_x^2)
+(\lambda+\mu)u_xv_y
\right]dx\,dy}.
$$

<h4 id="13c/b/ii">ii</h4>

↑ **Parent:** [B](#13c/b)

<h5 id="13c/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#13c/b/ii)

Let the displayed integrand be $F$. Since it has no explicit dependence on $u$ or $v$, the [Euler-Lagrange equations for two fields](../../../analysis.md#euler-lagrange-equations-for-two-fields) are

$$
\partial_xF_{u_x}+\partial_yF_{u_y}=0,
\qquad
\partial_xF_{v_x}+\partial_yF_{v_y}=0.
$$

Its derivatives are

$$
F_{u_x}=(\lambda+2\mu)u_x+(\lambda+\mu)v_y,
\qquad F_{u_y}=\mu u_y,
$$



$$
F_{v_x}=\mu v_x,
\qquad F_{v_y}=(\lambda+2\mu)v_y+(\lambda+\mu)u_x.
$$

Thus

$$
(\lambda+2\mu)u_{xx}+\mu u_{yy}
+(\lambda+\mu)v_{xy}=0,
$$



$$
\mu v_{xx}+(\lambda+2\mu)v_{yy}
+(\lambda+\mu)u_{xy}=0.
$$

Using the [Laplacian](../../../calculus.md#laplacian), [gradient](../../../calculus.md#gradient), and [divergence](../../../calculus.md#divergence), these combine into the static [Navier-Cauchy equation](../../../continuum-mechanics.md#navier-cauchy-equation)

$$
\boxed{\mu\nabla^2\mathbf u
+(\lambda+\mu)\nabla(\nabla\cdot\mathbf u)=0}.
$$

<h4 id="13c/b/iii">iii</h4>

↑ **Parent:** [B](#13c/b)

<h5 id="13c/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#13c/b/iii)

In the one-dimensional limit, $v=0$ and $u=u(x)$. The first component of the [Navier-Cauchy equation](../../../continuum-mechanics.md#navier-cauchy-equation) reduces to

$$
(\lambda+2\mu)u''(x)=0.
$$

For a [nondegenerate one-dimensional elastic material](../../../continuum-mechanics.md#nondegenerate-one-dimensional-elastic-material), $\lambda+2\mu\ne0$, so $u''=0$ and $u(x)=Ax+B$. The [boundary conditions](../../../differential-equation.md#boundary-condition) $u(0)=0$ and $u(L)=\Delta$ give $B=0$ and $A=\Delta/L$. Therefore the [uniform extension of a one-dimensional elastic body](../../../continuum-mechanics.md#uniform-extension-of-a-one-dimensional-elastic-body) is

$$
\boxed{u(x)=\frac{\Delta}{L}x}.
$$

## 14A

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="14a/a">a</h3>

↑ **Parent:** [14A](#14a)

<h4 id="14a/a/solution">Solution</h4>

↑ **Parent:** [A](#14a/a)

Take the [Fourier transform](../../../analysis.md#fourier-transform) in $x$. Since $\widetilde{\theta_{xx}}=-k^2\widetilde\theta$, the transformed [heat equation](../../../diffusion-equation.md#heat-equation) is

$$
\frac{\partial\widetilde\theta}{\partial t}
=-Dk^2\widetilde\theta,
\qquad
\widetilde\theta(k,0)=\widetilde\Theta(k).
$$

Therefore

$$
\widetilde\theta(k,t)=e^{-Dk^2t}\widetilde\Theta(k).
$$

The given transform pair and the [convolution theorem](../../../fourier-analysis.md#convolution-theorem) yield the [heat-kernel solution](../../../diffusion-equation.md#heat-kernel-solution)

$$
\boxed{
\theta(x,t)=\frac1{\sqrt{4\pi Dt}}
\int_{-\infty}^{\infty}
\exp\left[-\frac{(x-\xi)^2}{4Dt}\right]
\Theta(\xi)\,d\xi}.
$$

<h3 id="14a/b">b</h3>

↑ **Parent:** [14A](#14a)

<h4 id="14a/b/solution">Solution</h4>

↑ **Parent:** [B](#14a/b)

The causal [Green function](../../../analysis.md#green-s-function) for the heat operator is

$$
G(x,t;\xi,\tau)=H(t-\tau)
\frac1{\sqrt{4\pi D(t-\tau)}}
\exp\left[-\frac{(x-\xi)^2}{4D(t-\tau)}\right],
$$

where $H$ is the [Heaviside step function](../../../analysis.md#heaviside-step-function). It vanishes for $t<\tau$, satisfies the homogeneous heat equation away from the source, and approaches $\delta(x-\xi)$ as $t\downarrow\tau$. Superposing the responses to all infinitesimal sources gives [Duhamel principle](../../../diffusion-equation.md#duhamel-s-principle):

$$
\boxed{
\theta_f(x,t)=\int_0^t\int_{-\infty}^{\infty}
\frac{\exp\left[-\dfrac{(x-\xi)^2}{4D(t-\tau)}\right]}
{\sqrt{4\pi D(t-\tau)}}
f(\xi,\tau)\,d\xi\,d\tau}.
$$

The lower limit and causality give the required homogeneous initial data.

<h3 id="14a/c">c</h3>

↑ **Parent:** [14A](#14a)

<h4 id="14a/c/solution">Solution</h4>

↑ **Parent:** [C](#14a/c)

Let

$$
g(x,t)=\frac1{\sqrt{4\pi Dt}}
\exp\left(-\frac{x^2}{4Dt}\right),
\qquad t>0.
$$

Convolution with the initial [Dirac delta function](../../../distribution-theory.md#dirac-delta-function) translates the [heat kernel](../../../diffusion-equation.md#heat-kernel), while part (b) propagates the impulsive source from time one. Hence

$$
\boxed{
\theta_c(x,t)=g(x-2\sqrt D,t)
-A H(t-1)g(x+2\sqrt D,t-1)}.
$$

At $(x,t)=(0,2)$ this becomes

$$
\theta_c(0,2)
=\frac{e^{-1/2}}{\sqrt{8\pi D}}
-A\frac{e^{-1}}{\sqrt{4\pi D}}.
$$

It vanishes exactly when

$$
A=\frac{e^{-1/2}}{\sqrt{8\pi D}}
\frac{\sqrt{4\pi D}}{e^{-1}}
=\boxed{\sqrt{\frac e2}}.
$$

This is the [cancellation of two heat-kernel impulses](../../../diffusion-equation.md#cancellation-of-two-heat-kernel-impulses).

## 15D

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="15d/a">a</h3>

↑ **Parent:** [15D](#15d)

<h4 id="15d/a/solution">Solution</h4>

↑ **Parent:** [A](#15d/a)

Use $[AB,C]=A[B,C]+[A,C]B$ and the [canonical commutation relation](../../../quantum-mechanics.md#canonical-commutation-relation). With $L_i=\varepsilon_{iab}x_ap_b$,

$$
\begin{aligned}
[L_i,x_j]
&=\varepsilon_{iab}x_a[p_b,x_j]
=-i\hbar\varepsilon_{iaj}x_a
=i\hbar\varepsilon_{ijk}x_k,\\
[L_i,p_j]
&=\varepsilon_{iab}[x_a,p_j]p_b
=i\hbar\varepsilon_{ijb}p_b
=i\hbar\varepsilon_{ijk}p_k.
\end{aligned}
$$

Using these two transformation laws on $L_j=\varepsilon_{jab}x_ap_b$ gives

$$
\begin{aligned}
[L_i,L_j]
&=\varepsilon_{jab}([L_i,x_a]p_b+x_a[L_i,p_b])\\
&=\boxed{i\hbar\varepsilon_{ijk}L_k}.
\end{aligned}
$$

These are the [orbital angular momentum commutation relations](../../../quantum-mechanics.md#orbital-angular-momentum-commutation-relations).

Now

$$
[L^2,L_i]=\sum_j\bigl(L_j[L_j,L_i]+[L_j,L_i]L_j).
$$

The factor $[L_j,L_i]$ is antisymmetric in $j$ and its remaining product is symmetric after the two terms are combined, so the contraction vanishes:

$$
\boxed{[L^2,L_i]=0}.
$$

The same commutators show that $p^2=p_jp_j$ and $r^2=x_jx_j$ are rotational scalars: their commutators with every $L_i$ vanish by contraction of the antisymmetric $\varepsilon_{ijk}$ with a symmetric product. Therefore $U(r)$ also commutes with every $L_i$, and for

$$
H=\frac{p^2}{2m}+U(r)
$$

we have $[H,L_i]=0$, hence

$$
\boxed{[H,L^2]=0}.
$$

In particular $H,L^2,L_3$ are pairwise commuting Hermitian operators. By [simultaneous diagonalization](../../../mathematics.md#simultaneous-diagonalization), they admit a common eigenbasis, subject to the usual spectral-domain qualifications for unbounded operators. This is the [rotational invariance of a central-potential Hamiltonian](../../../quantum-mechanics.md#rotational-invariance-of-a-central-potential-hamiltonian).

<h3 id="15d/b">b</h3>

↑ **Parent:** [15D](#15d)

<h4 id="15d/b/i">i</h4>

↑ **Parent:** [B](#15d/b)

<h5 id="15d/b/i/solution">Solution</h5>

↑ **Parent:** [I](#15d/b/i)

For a bound state, $E<0$ and therefore $\gamma>0$. As $r\to\infty$, the terms proportional to $1/r$ are subleading and the [Radial Schrodinger equation](../../../physics.md#radial-schrodinger-equation-for-the-hydrogen-atom) has dominant balance

$$
R''-\gamma^2R\simeq0.
$$

Its exponential behaviours are $e^{\gamma r}$ and $e^{-\gamma r}$. The growing solution is not [normalizable](../../../quantum-mechanics.md#normalizable-wavefunction), so

$$
\boxed{R(r)\sim e^{-\gamma r}}.
$$

<h4 id="15d/b/ii">ii</h4>

↑ **Parent:** [B](#15d/b)

<h5 id="15d/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#15d/b/ii)

Put $R=f e^{-\gamma r}$. Then

$$
R'=e^{-\gamma r}(f'-\gamma f),
\qquad
R''=e^{-\gamma r}(f''-2\gamma f'+\gamma^2f).
$$

After substitution and cancellation of the $\gamma^2f$ terms, the equation becomes

$$
rf''+(2-2\gamma r)f'+(\beta-2\gamma)f=0.
$$

For the [power series](../../../real-analysis.md#power-series) $f=\sum_{n=0}^{\infty}a_nr^n$, the coefficient of $r^{n-1}$ is

$$
n(n+1)a_n+(\beta-2\gamma n)a_{n-1}=0.
$$

Thus

$$
\boxed{a_n=\frac{2\gamma n-\beta}{n(n+1)}a_{n-1}}.
$$

If the series does not terminate, then $a_n/a_{n-1}\sim2\gamma/n$, so $f$ acquires the large-$r$ behaviour $e^{2\gamma r}$ and $R$ grows like $e^{\gamma r}$. Normalizability therefore requires termination, which occurs when

$$
2\gamma N-\beta=0
$$

for some positive integer $N$. Hence

$$
\gamma_N=\frac{\beta}{2N},
\qquad
E_N=-\frac{\hbar^2\gamma_N^2}{2m}
=-\frac{mq^4}{2\hbar^2N^2}.
$$

The ground state has $N=1$, so the [hydrogen ground-state energy](../../../physics.md#hydrogen-ground-state-energy) is

$$
\boxed{E_1=-\frac{mq^4}{2\hbar^2}}.
$$

This is the [series-termination quantization of the Coulomb radial equation](../../../physics.md#series-termination-quantization-of-the-coulomb-radial-equation).

<h4 id="15d/b/iii">iii</h4>

↑ **Parent:** [B](#15d/b)

<h5 id="15d/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#15d/b/iii)

Take the spherical harmonic $Y_{00}$ to have unit angular norm. The radial normalization condition is then

$$
1=\int_0^\infty |R(r)|^2r^2\,dr
=C^2\int_0^\infty r^2e^{-2\gamma r}\,dr
=\frac{C^2}{4\gamma^3}.
$$

Therefore

$$
\boxed{C=2\gamma^{3/2}}.
$$

Equivalently, if $R$ denotes the entire spherically symmetric wavefunction rather than the radial factor multiplying normalized $Y_{00}$, then $C=(\gamma^3/\pi)^{1/2}$.

The expected radius is

$$
\begin{aligned}
\langle r\rangle_R
&=C^2\int_0^\infty r^3e^{-2\gamma r}\,dr\\
&=4\gamma^3\frac{3!}{(2\gamma)^4}
=\boxed{\frac{3}{2\gamma}}.
\end{aligned}
$$

For the ground state, $\gamma=mq^2/\hbar^2$. The [Bohr radius](../../../physics.md#bohr-radius) is $a_0=\hbar^2/(mq^2)=1/\gamma$, so

$$
\boxed{\langle r\rangle_R=\frac32a_0}.
$$

The mean radius is therefore of the Bohr-radius scale and is one and a half times $a_0$. This is the [radial normalization of the hydrogen ground state](../../../physics.md#radial-normalization-of-the-hydrogen-ground-state).

## 16C

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="16c/a">a</h3>

↑ **Parent:** [16C](#16c)

<h4 id="16c/a/solution">Solution</h4>

↑ **Parent:** [A](#16c/a)

Write the free surface as the zero set

$$
S(x,y,z,t)=z-\eta(x,y,t)=0.
$$

Because this is a material surface, the [kinematic boundary condition](../../../fluid-mechanics.md#kinematic-boundary-condition) is $DS/Dt=0$. Thus, on $z=\eta$,

$$
0=S_t+uS_x+vS_y+wS_z
=-\eta_t-u\eta_x-v\eta_y+w.
$$

Therefore

$$
\boxed{w=\eta_t+u\eta_x+v\eta_y
=\frac{D\eta}{Dt}}
$$

at the free surface. This is the [kinematic boundary condition for a free-surface graph](../../../fluid-mechanics.md#kinematic-boundary-condition-for-a-free-surface-graph).

<h3 id="16c/b">b</h3>

↑ **Parent:** [16C](#16c)

<h4 id="16c/b/i">i</h4>

↑ **Parent:** [B](#16c/b)

<h5 id="16c/b/i/solution">Solution</h5>

↑ **Parent:** [I](#16c/b/i)

For [irrotational flow](../../../fluid-mechanics.md#irrotational-flow), $\mathbf u=\nabla\phi$. Incompressibility gives the [Laplace equation](../../../partial-differential-equation.md#laplace-equation)

$$
\boxed{\nabla^2\phi=0},
\qquad 0<x<L,quad0<y<L,quad z<0.
$$

The rigid side walls impose no penetration:

$$
\phi_x=0\quad(x=0,L),
\qquad
\phi_y=0\quad(y=0,L),
$$

and decay in the infinitely deep fluid requires $\nabla\phi\to0$ as $z\to-\infty$.

Linearizing the kinematic condition from part (a) about $z=0$ gives

$$
\boxed{\eta_t=\phi_z\quad(z=0)}.
$$

The [Unsteady Bernoulli equation](../../../fluid-mechanics.md#unsteady-bernoulli-equation), evaluated at the surface and linearized about hydrostatic equilibrium, gives the dynamic condition

$$
\boxed{\phi_t+g\eta
=-\frac{p_0}{\rho}cos\frac{\pi x}{L}
\cos\frac{2\pi y}{L}\cos(\omega t)quad(z=0)}.
$$

These are the [linearized free-surface boundary conditions](../../../fluid-mechanics.md#linearized-free-surface-boundary-conditions). Initial values for $\eta$ and $\phi$ specify the transient; below we also record the initially quiescent solution.

<h4 id="16c/b/ii">ii</h4>

↑ **Parent:** [B](#16c/b)

<h5 id="16c/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#16c/b/ii)

For

$$
\phi=Z(z)\cos\frac{\pi x}{L}
\cos\frac{2\pi y}{L}F(t),
$$

the normal derivative at $x=0,L$ contains $\sin(\pi x/L)$ and the normal derivative at $y=0,L$ contains $\sin(2\pi y/L)$. Both therefore vanish at the side walls.

At $z=0$, $\phi_t$ has exactly the same horizontal dependence as the imposed pressure. The dynamic boundary condition is consequently consistent provided $\eta$ has that same horizontal mode. This is the [rectangular standing surface-gravity mode](../../../fluid-mechanics.md#rectangular-standing-surface-gravity-mode) selected by the forcing.

<h4 id="16c/b/iii">iii</h4>

↑ **Parent:** [B](#16c/b)

<h5 id="16c/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#16c/b/iii)

Substitution into $\nabla^2\phi=0$ gives

$$
Z''-\left[\left(\frac\pi L\right)^2
+\left(\frac{2\pi}{L}\right)^2\right]Z=0.
$$

Set

$$
k=\frac{\pi\sqrt5}{L}.
$$

Then $Z=Ae^{kz}+Be^{-kz}$. Since the fluid occupies $z<0$, decay as $z\to-\infty$ forces $B=0$. Absorbing $A$ into $F$ and choosing $Z(0)=1$ gives

$$
\boxed{Z(z)=e^{kz},
\qquad k=\frac{\pi\sqrt5}{L}}.
$$

This is the usual exponential depth dependence of a [deep-water gravity wave](../../../fluid-mechanics.md#deep-water-gravity-wave).

<h4 id="16c/b/iv">iv</h4>

↑ **Parent:** [B](#16c/b)

<h5 id="16c/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#16c/b/iv)

With $Z'(0)=k$, the linearized kinematic condition gives

$$
\cos\frac{\pi x}{L}\cos\frac{2\pi y}{L}H'(t)
=k\cos\frac{\pi x}{L}\cos\frac{2\pi y}{L}F(t).
$$

Hence

$$
\boxed{\eta(x,y,t)=\cos\frac{\pi x}{L}
\cos\frac{2\pi y}{L}H(t)},
\qquad
\boxed{H'(t)=kF(t)}.
$$

<h4 id="16c/b/v">v</h4>

↑ **Parent:** [B](#16c/b)

<h5 id="16c/b/v/solution">Solution</h5>

↑ **Parent:** [V](#16c/b/v)

The dynamic condition reduces to

$$
F'(t)+gH(t)=-\frac{p_0}{\rho}\cos(\omega t).
$$

Differentiate $H'=kF$ and define the natural frequency

$$
\Omega^2=gk=\frac{\pi g\sqrt5}{L}.
$$

Then the surface amplitude obeys the [forced harmonic oscillator](../../../analysis.md#forced-harmonic-oscillator)

$$
\boxed{H''+\Omega^2H
=-\frac{kp_0}{\rho}\cos(\omega t)}.
$$

For $\omega\ne\Omega$, its general solution and the corresponding potential amplitude are

$$
H=C\cos(\Omega t)+D\sin(\Omega t)
+\frac{kp_0}{\rho(\omega^2-\Omega^2)}\cos(\omega t),
$$



$$
F=\frac{H'}k.
$$

If the fluid is initially quiescent, $H(0)=F(0)=0$, so

$$
\boxed{H(t)=\frac{kp_0}{\rho(\omega^2-\Omega^2)}
\bigl(\cos(\omega t)-\cos(\Omega t)\bigr)},
$$



$$
\boxed{F(t)=\frac{p_0}{\rho(\omega^2-\Omega^2)}
\bigl(\Omega\sin(\Omega t)-\omega\sin(\omega t)\bigr)}.
$$

<h4 id="16c/b/vi">vi</h4>

↑ **Parent:** [B](#16c/b)

<h5 id="16c/b/vi/solution">Solution</h5>

↑ **Parent:** [Vi](#16c/b/vi)

The denominators in part (v) vanish when the forcing frequency equals the natural [surface gravity wave](../../../fluid-mechanics.md#surface-gravity-wave) frequency

$$
\boxed{\omega=\Omega
=\sqrt{gk}
=\left(\frac{\pi g\sqrt5}{L}\right)^{1/2}}.
$$

At this value, the initially quiescent resonant solution is

$$
H(t)=-\frac{kp_0}{2\rho\Omega},t\sin(\Omega t),
$$



$$
F(t)=-\frac{p_0}{2\rho\Omega}
\bigl(\sin(\Omega t)+\Omega t\cos(\Omega t)\bigr).
$$

Both contain a term growing linearly in time. This is [resonance](../../../dynamical-systems.md#resonance): the pressure forcing repeatedly supplies energy in phase with the box's $(1,2)$ standing-wave mode. In the ideal inviscid linear model there is no damping or nonlinear saturation, so its amplitude is unbounded. This is the [resonance of a pressure-forced rectangular surface-gravity mode](../../../fluid-mechanics.md#resonance-of-a-pressure-forced-rectangular-surface-gravity-mode).

## 17H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="17h/a">a</h3>

↑ **Parent:** [17H](#17h)

<h4 id="17h/a/solution">Solution</h4>

↑ **Parent:** [A](#17h/a)

Write the linear mean model as

$$
Y_i=\theta x_i+\varepsilon_i,
\qquad
\mathbb E\varepsilon_i=0,
\qquad
\operatorname{var}(\varepsilon_i)=\theta x_i.
$$

The errors are independent but [heteroscedastic](../../../statistical-modelling.md#heteroscedastic). Minimizing the unweighted residual sum of squares

$$
Q(\theta)=\sum_{i=1}^n(Y_i-\theta x_i)^2
$$

gives the [normal equation](../../../statistical-modelling.md#normal-equation)

$$
0=Q'(\theta)=-2\sum_i x_i(Y_i-\theta x_i).
$$

Thus, provided $\sum_i x_i^2>0$,

$$
\boxed{\widehat\theta_{LS}
=\frac{\sum_i x_iY_i}{\sum_i x_i^2}}.
$$

Since $\mathbb EY_i=\theta x_i$,

$$
\mathbb E\widehat\theta_{LS}
=\frac{\theta\sum_i x_i^2}{\sum_i x_i^2}=\theta.
$$

**Hence it is an [unbiased estimator](../../../statistical-modelling.md#unbiased-estimator). This is the least-squares part of the [estimators for a Poisson exposure model](../../../statistical-modelling.md#estimators-for-a-poisson-exposure-model).**

<h3 id="17h/b">b</h3>

↑ **Parent:** [17H](#17h)

<h4 id="17h/b/solution">Solution</h4>

↑ **Parent:** [B](#17h/b)

Ignoring terms independent of $\theta$, the [log-likelihood](../../../statistical-modelling.md#log-likelihood) is

$$
\ell(\theta)
=\sum_i\bigl(Y_i\log\theta-\theta x_i\bigr)+\text{constant}.
$$

Its [score function](../../../statistical-modelling.md#informant-function) is

$$
\ell'(\theta)=\frac{\sum_iY_i}{\theta}-\sum_i x_i.
$$

Since $\ell''(\theta)=-(\sum_iY_i)/\theta^2\leq0$, the interior critical point is the maximum, giving

$$
\boxed{\widehat\theta_{MLE}
=\frac{\sum_iY_i}{\sum_i x_i}}.
$$

The sum of independent [Poisson distributions](../../../discrete-probability-distribution.md#poisson-distribution) is Poisson with mean $\theta\sum_i x_i$, so

$$
\mathbb E\widehat\theta_{MLE}=\theta.
$$

**Thus the [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator) is also unbiased.**

<h3 id="17h/c">c</h3>

↑ **Parent:** [17H](#17h)

<h4 id="17h/c/solution">Solution</h4>

↑ **Parent:** [C](#17h/c)

Put

$$
S_r=\sum_{i=1}^n x_i^r.
$$

Independence and $\operatorname{var}(Y_i)=\theta x_i$ give

$$
\boxed{\operatorname{var}(\widehat\theta_{LS})
=\frac{\theta S_3}{S_2^2}},
$$

whereas $\sum_iY_i\sim\operatorname{Poisson}(\theta S_1)$ gives

$$
\boxed{\operatorname{var}(\widehat\theta_{MLE})
=\frac{\theta}{S_1}}.
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), applied to $(x_i^{1/2})$ and $(x_i^{3/2})$, yields

$$
S_2^2=\left(\sum_i x_i^{1/2}x_i^{3/2}\right)^2
\leq S_1S_3.
$$

Consequently

$$
\boxed{\operatorname{var}(\widehat\theta_{MLE})
\leq\operatorname{var}(\widehat\theta_{LS})}.
$$

Equality holds exactly when all positive exposures $x_i$ are equal. This is the [variance comparison for Poisson exposure estimators](../../../statistical-modelling.md#variance-comparison-for-poisson-exposure-estimators).

<h3 id="17h/d">d</h3>

↑ **Parent:** [17H](#17h)

<h4 id="17h/d/solution">Solution</h4>

↑ **Parent:** [D](#17h/d)

Both alternatives have larger $\theta$, so use upper-tail rejection regions. Let $z_{0.95}=\Phi^{-1}(0.95)\simeq1.645$ be the 95th [quantile](../../../probability-theory.md#quantile-function) of the standard [normal distribution](../../../probability-theory.md#normal-distribution).

For the likelihood estimator,

$$
\sum_iY_i\sim\operatorname{Poisson}(\theta S_1).
$$

When $S_1$ is large, the [normal approximation to the Poisson distribution](../../../discrete-probability-distribution.md#normal-approximation-to-the-poisson-distribution) gives, under $H_0$,

$$
\widehat\theta_{MLE}\approx N\left(1,\frac1{S_1}\right).
$$

An approximate size-$0.05$ test therefore rejects $H_0$ when

$$
\boxed{\widehat\theta_{MLE}
>1+\frac{1.645}{\sqrt{S_1}}}.
$$

When every $x_i$ is large, $Y_i\approx N(\theta x_i,\theta x_i)$ independently. A linear combination of independent normal variables is normal, so under $H_0$,

$$
\widehat\theta_{LS}\approx
N\left(1,\frac{S_3}{S_2^2}\right).
$$

The corresponding approximate size-$0.05$ test rejects when

$$
\boxed{\widehat\theta_{LS}
>1+1.645\frac{\sqrt{S_3}}{S_2}}.
$$

In both cases the null rejection probability is approximately $0.05$, while values near the alternative mean $2$ increasingly fall in the rejection region as the total exposure grows. These are the [normal-approximation tests for a Poisson exposure model](../../../statistical-modelling.md#normal-approximation-tests-for-a-poisson-exposure-model).

## 18H

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="18h/solution">Solution</h3>

↑ **Parent:** [18H](#18h)

Let $p\in\mathbb R^m$ be Player I's row-strategy distribution and let $e$ denote an all-ones vector of the required dimension. Against column $j$, the expected payoff is $(p^TA)_j$. Thus Player I's [matrix-game optimization problem](../../../game-theory.md#matrix-game-optimization-problem) is

$$
\boxed{
\max_{p,v}v
\quad\text{subject to}\quad
A^Tp\geq ve,quad e^Tp=1,quad p\geq0}.
$$

Equivalently, Player I maximizes $\min_j(p^TA)_j$ over the probability simplex.

Let $q^*$ be an optimal mixed strategy for Player II and let the game value be $v^*$. A sufficient condition for a probability vector $p$ to be optimal for Player I is

$$
\boxed{p^TA\geq v^*e^T}.
$$

Indeed, this makes $p$ guarantee at least $v^*$ against every pure column and hence every mixed strategy. On the other hand, the optimality of $q^*$ prevents any row strategy from obtaining more than $v^*$ against $q^*$. Therefore $p$ is optimal. This is the [mixed-strategy optimality certificate for a matrix game](../../../game-theory.md#mixed-strategy-optimality-certificate-for-a-matrix-game).

Now suppose that $A$ is invertible and symmetric and that $A^{-1}e\geq0$. Put

$$
c=e^TA^{-1}e,
\qquad
p=q=\frac{A^{-1}e}{c}.
$$

The vector $A^{-1}e$ is nonzero and nonnegative, so $c>0$ and $p,q$ are probability vectors. Since $A$ is symmetric,

$$
p^TA=\frac{e^T}{c},
\qquad
Aq=\frac e c.
$$

Thus $p$ guarantees $1/c$ and $q$ holds the payoff to $1/c$. By the [minimax theorem](../../../game-theory.md#minimax-theorem),

$$
\boxed{v^*=\frac1{e^TA^{-1}e}}.
$$

This proves the [symmetric inverse formula for a matrix-game equilibrium](../../../game-theory.md#symmetric-inverse-formula-for-a-matrix-game-equilibrium).

For the card game, the payoff matrix to Player I is

$$
A=\begin{pmatrix}
2&3&4\\
3&4&-5\\
4&-5&-6
\end{pmatrix}.
$$

It is symmetric and invertible, and direct solution of $Ax=e$ gives

$$
A^{-1}e=\frac1{114}
\begin{pmatrix}41\\4\\5\end{pmatrix},
\qquad
e^TA^{-1}e=\frac{25}{57}.
$$

The preceding result therefore gives the same optimal strategy for both players:

$$
\boxed{
p^*=q^*=\begin{pmatrix}
41/50\\[2pt]2/25\\[2pt]1/10
\end{pmatrix}}.
$$

Thus each player chooses cards $1,2,3$ with probabilities $41/50,2/25,1/10$, respectively, and the value to Player I is

$$
\boxed{v^*=\frac{57}{25}\text{ pounds}}.
$$

This is the [three-card threshold-sum zero-sum game](../../../game-theory.md#three-card-threshold-sum-zero-sum-game).

## ↑ Ancestors (8)

1. [Ib](../ib.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
