# Paper 302

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20302.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20302.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
  - [f](#3/f)
    - [Solution](#3/f/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)
  - [f](#4/f)
    - [Solution](#4/f/solution)

## 1

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Put $\Lambda(t)=I+tX+O(t^2)$ in $\Lambda^T\eta\Lambda=\eta$. The coefficient of $t$ is $X^T\eta+\eta X$, so it must vanish. For $X=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ this condition is

$$
\begin{pmatrix}2a&b-c\\b-c&-2d\end{pmatrix}=0.
$$

Hence $a=d=0$ and $b=c$. Thus the [Lie algebra](../../../lie-algebra.md) is one-dimensional with basis

$$
K=\begin{pmatrix}0&1\\1&0\end{pmatrix},
\qquad \mathfrak{so}(1,1)=\mathbb RK.
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write $X(\varphi)=\varphi K$. Since $K^2=I$, the [Exponential map of a Lie group](../../../lie-theory.md#exponential-map-of-a-lie-group) gives

$$
\Lambda(\varphi)=e^{\varphi K}
=\cosh\varphi,I+\sinh\varphi,K
=\begin{pmatrix}\cosh\varphi&\sinh\varphi\\\sinh\varphi&\cosh\varphi\end{pmatrix}.
$$

The hyperbolic addition formulas give $\Lambda(\varphi)\Lambda(\psi)=\Lambda(\varphi+\psi)$ and $\Lambda(\varphi)^{-1}=\Lambda(-\varphi)$, so these matrices form a subgroup of the [One-dimensional Lorentz group](../../../special-relativity.md#one-dimensional-lorentz-group). It is Abelian because addition in $\mathbb R$ is commutative. It is noncompact because $\cosh\varphi$ is unbounded, equivalently because the subgroup is homeomorphic to $\mathbb R$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For the [null coordinates in two-dimensional Minkowski spacetime](../../../special-relativity.md#null-coordinates-in-two-dimensional-minkowski-spacetime), direct substitution gives

$$
u'=x'+y'=e^\varphi u,
\qquad
v'=x'-y'=e^{-\varphi}v.
$$

Thus a boost dilates one null direction and contracts the other by the reciprocal factor. It preserves

$$
uv=x^2-y^2.
$$

The invariant curves are therefore the level sets $x^2-y^2=c$: the branches of hyperbolas for $c\ne0$, together with the two null lines when $c=0$. Each connected branch is preserved by the identity component.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Solving $\Lambda^T\eta\Lambda=\eta$ with $\det\Lambda=1$ shows that every element is either $\Lambda(\varphi)$ or $-\Lambda(\varphi)$. Hence

$$
SO(1,1)=\{\Lambda(\varphi):\varphi\in\mathbb R\}
\sqcup\{-\Lambda(\varphi):\varphi\in\mathbb R\}.
$$

Each set is connected, but the sign of the $(1,1)$ entry cannot change continuously because its absolute value is at least one. Thus $SO(1,1)$ has two connected components. The matrix $-I$ lies in the component disjoint from the identity.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

For $\varphi\ne\pm1$, the [Cayley transform](../../../lie-theory.md#cayley-transform-lie-theory) is

$$
C(\varphi K)
=\frac1{1-\varphi^2}
\begin{pmatrix}1+\varphi^2&2\varphi\\2\varphi&1+\varphi^2\end{pmatrix}.
$$

Writing its diagonal and off-diagonal entries as $a,b$, one has $a^2-b^2=1$, so $C^T\eta C=\eta$ and $\det C=1$. For $|\varphi|<1$, put $\varphi=\tanh(t/2)$ to obtain $C(\varphi K)=\Lambda(t)$, so this interval covers the identity component. For $|\varphi|>1$ the image lies in the other component and covers it except for $-I$, approached only as $|\varphi|\to\infty$. The [Exponential map of a Lie group](../../../lie-theory.md#exponential-map-of-a-lie-group) reaches only the identity component, whereas the Cayley transform also reaches nonidentity-component elements but omits $-I$ and is undefined at $\varphi=\pm1$.

## 2

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Differentiating $\Lambda^T\eta\Lambda=\eta$ at the identity gives $X^T\eta+\eta X=0$. The six matrices

$$
(M^{\mu\nu})^\alpha{}_{\beta}
=\eta^{\mu\alpha}\delta^\nu_\beta
-\eta^{\nu\alpha}\delta^\mu_\beta,
\qquad M^{\mu\nu}=-M^{\nu\mu},
$$

obey this condition and form a basis of the [Lorentz algebra](../../../semisimple-lie-algebra.md#lorentz-algebra). With cyclic indices,

$$
J_1=M^{23},\quad J_2=M^{31},\quad J_3=M^{12},
\qquad K_i=M^{0i}.
$$

The $J_i$ mix the two spatial coordinates perpendicular to $x^i$ and therefore generate rotations about that axis; $K_i$ mixes $x^0$ with $x^i$ and generates a Lorentz boost in the $x^i$ direction.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Matrix multiplication gives

$$
[J_i,J_j]=\epsilon_{ijk}J_k,
\qquad [J_i,K_j]=\epsilon_{ijk}K_k,
\qquad [K_i,K_j]=-\epsilon_{ijk}J_k.
$$

For example, $[J_1,J_2]=J_3$, $[K_1,K_2]=-J_3$, and $[J_1,K_2]=K_3$. Over $\mathbb C$, define

$$
A_i=\frac12(J_i+iK_i),
\qquad B_i=\frac12(J_i-iK_i).
$$

Then $[A_i,A_j]=\epsilon_{ijk}A_k$, $[B_i,B_j]=\epsilon_{ijk}B_k$, and $[A_i,B_j]=0$. This proves the [chiral decomposition of the complex Lorentz algebra](../../../semisimple-lie-algebra.md#chiral-decomposition-of-the-complex-lorentz-algebra). Its finite-dimensional irreducible representations are tensor products of irreducible representations of the two factors and are labelled by pairs $(j_L,j_R)$ of nonnegative half-integers.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

A coordinate transformation $x\mapsto Px$ conjugates an infinitesimal generator, hence $M^{\mu\nu}\mapsto PM^{\mu\nu}P$. It fixes the rotation generators $J_i$ and negates the boosts $K_i$. Therefore it exchanges $A_i$ and $B_i$, and the [parity action on a Lorentz representation](../../../semisimple-lie-algebra.md#parity-action-on-a-lorentz-representation) is

$$
(j_L,j_R)\longmapsto(j_R,j_L).
$$

An irreducible representation is parity invariant precisely when $j_L=j_R$. If $j_L\ne j_R$, parity invariance requires the reducible sum $(j_L,j_R)\oplus(j_R,j_L)$. Thus the two [Weyl-spinor](../../../relativistic-quantum-field.md#weyl-spinor) representations $(1/2,0)$ and $(0,1/2)$ are exchanged, while their direct sum is the parity-invariant [Dirac spinor](../../../relativistic-quantum-field.md#dirac-spinor).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Parity preserves the [Minkowski metric](../../../special-relativity.md#minkowski-metric) but reverses orientation. Hence ordinary tensor contraction makes

$$
C_1=M_{\mu\nu}M^{\mu\nu}
$$

parity even, while the Levi-Civita pseudotensor changes sign and makes

$$
C_2=M_{\mu\nu}\widetilde M^{\mu\nu}
$$

parity odd. Equivalently, $C_1$ is proportional to $\mathbf J^2-\mathbf K^2$ and $C_2$ to $\mathbf J\cdot\mathbf K$. The combinations $C_1\pm iC_2$ are proportional to the two quadratic [Lorentz Casimir invariants](../../../semisimple-lie-algebra.md#lorentz-casimir-invariants), and parity exchanges them exactly as it exchanges the two factors in the complexified algebra.

## 3

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [Adjoint representation of a Lie algebra](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) is

$$
\operatorname{ad}:\mathfrak g\to\mathfrak{gl}(\mathfrak g),
\qquad \operatorname{ad}_X(Y)=[X,Y].
$$

It is linear. The [Jacobi identity](../../../lie-algebra.md#jacobi-identity) gives

$$
[\operatorname{ad}_X,\operatorname{ad}_Y]Z
=[X,[Y,Z]]-[Y,[X,Z]]=[[X,Y],Z]
=\operatorname{ad}_{[X,Y]}Z,
$$

so it is a [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [Killing form](../../../lie-algebra.md#killing-form) is $\kappa(X,Y)=\operatorname{Tr}(\operatorname{ad}_X\operatorname{ad}_Y)$. From part (a),

$$
\begin{aligned}
\kappa([X,Y],Z)
&=\operatorname{Tr}([\operatorname{ad}_X,\operatorname{ad}_Y]\operatorname{ad}_Z)\\
&=\operatorname{Tr}(\operatorname{ad}_X[\operatorname{ad}_Y,\operatorname{ad}_Z])\\
&=\kappa(X,[Y,Z]),
\end{aligned}
$$

where the middle equality uses cyclicity of the [trace](../../../linear-algebra.md#matrix-trace).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Each [structure constant of a Lie algebra](../../../lie-algebra.md#structure-constant-of-a-lie-algebra) satisfies $f_{ab}{}^d=-f_{ba}{}^d$, so $f_{abc}=f_{ab}{}^d\kappa_{dc}$ is antisymmetric in $a,b$. Invariance of the [Killing form](../../../lie-algebra.md#killing-form) gives

$$
f_{abc}=\kappa([T_a,T_b],T_c)
=\kappa(T_a,[T_b,T_c])=f_{bca}.
$$

This cyclic symmetry together with antisymmetry in the first pair implies antisymmetry under every transposition. Thus $f_{abc}$ is totally antisymmetric.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let $W\subseteq\mathfrak g$ be invariant under the [Adjoint representation of a Lie algebra](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra). Then $[\mathfrak g,W]\subseteq W$, so $W$ is an ideal. If $\mathfrak g$ is a [simple Lie algebra](../../../semisimple-lie-algebra.md#simple-lie-algebra), its only ideals are $0$ and $\mathfrak g$. Hence the adjoint representation is irreducible. Compact type is compatible with the anti-Hermitian realization used below, although simplicity alone proves this [adjoint irreducibility of a simple Lie algebra](../../../lie-algebra.md#adjoint-irreducibility-of-a-simple-lie-algebra).

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The [Trace form of a Lie algebra representation](../../../lie-algebra.md#trace-form-of-a-lie-algebra-representation) is invariant because

$$
\begin{aligned}
H([X,Y],Z)
&=\operatorname{Tr}([d(X),d(Y)]d(Z))\\
&=\operatorname{Tr}(d(X)[d(Y),d(Z)])
=H(X,[Y,Z]).
\end{aligned}
$$

Choose a basis orthonormal for the positive-definite form $-\kappa$ of the compact simple algebra. Any invariant bilinear form determines an endomorphism commuting with the irreducible adjoint action; [Schur lemma](../../../representation-theory.md#schur-s-lemma) makes it scalar. Thus $H(T_a,T_b)=c\delta_{ab}$. Since $d(T_a)$ is anti-Hermitian,

$$
H(T_a,T_a)=-\operatorname{Tr}(d(T_a)^\dagger d(T_a))<0.
$$

The inequality is strict because the kernel of the nontrivial irreducible representation is an ideal and hence zero. Therefore $c=-\mu$ with $\mu>0$.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

For the [trace trilinear form of a Lie algebra representation](../../../lie-algebra.md#trace-trilinear-form-of-a-lie-algebra-representation), the trace of a commutator vanishes:

$$
B([X,Y],Z,W)+B(Y,[X,Z],W)+B(Y,Z,[X,W])=0.
$$

Taking $X=T_b$, $Y=T_a$, $Z=T_c$, $W=T_d$ and expanding each [Lie bracket](../../../lie-algebra.md#lie-bracket) gives

$$
f^e{}_{ba}B_{cde}+f^e{}_{bc}B_{dae}+f^e{}_{bd}B_{ace}=0.
$$

Since $f_a{}^{bc}$ is antisymmetric in $b,c$,

$$
\begin{aligned}
f_a{}^{bc}B_{bcd}
&=\frac12f_a{}^{bc}\operatorname{Tr}([d(T_b),d(T_c)]d(T_d))\\
&=\frac12f_a{}^{bc}f_{bc}{}^eH(T_e,T_d).
\end{aligned}
$$

Raising indices with the inverse [Killing form](../../../lie-algebra.md#killing-form) gives $f_a{}^{bc}f_{bc}{}^e=\delta_a{}^e$ in the stated normalization. Using $H(T_e,T_d)=-\mu\delta_{ed}$ proves

$$
\boxed{f_a{}^{bc}B_{bcd}=-\frac\mu2\delta_{ad}.}
$$

## 4

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [special orthogonal group](../../../linear-algebra.md#special-orthogonal-group) is

$$
SO(5)=\{R\in GL(5,\mathbb R):R^TR=I,\ \det R=1\}.
$$

Its [Lie algebra](../../../lie-algebra.md) consists of antisymmetric $5\times5$ matrices, determined by the entries above the diagonal. Therefore

$$
\boxed{D=\binom52=10.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For every $R\in SO(4)$,

$$
\iota(R)=\begin{pmatrix}R&0\\0&1\end{pmatrix}
$$

is orthogonal with determinant one. Moreover $\iota(R_1R_2)=\iota(R_1)\iota(R_2)$ and $\iota$ is injective, so these block-diagonal matrices form an $SO(4)$ subgroup of $SO(5)$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Under the subgroup in part (b), $(v,s)\in\mathbb R^4\oplus\mathbb R$ transforms as $(Rv,s)$, hence

$$
\mathbf5\downarrow SO(4)=\mathbf4\oplus\mathbf1.
$$

An element of $\mathfrak{so}_5$ has the unique block form

$$
X=\begin{pmatrix}A&v\\-v^T&0\end{pmatrix},
\qquad A\in\mathfrak{so}_4,quad v\in\mathbb R^4.
$$

Conjugation by $\iota(R)$ sends $(A,v)$ to $(RAR^{-1},Rv)$. Thus

$$
\mathbf{10}\downarrow SO(4)=\mathbf6_{\mathrm{ad}}\oplus\mathbf4,
$$

and the dimensions check as $5=4+1$ and $10=6+4$. These are the [SO5 to SO4 branching](../../../semisimple-lie-algebra.md#so5-to-so4-branching) rules.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The [fundamental weights](../../../semisimple-lie-algebra.md#fundamental-weight) satisfy $2(\omega_i,\alpha_j)/(\alpha_j,\alpha_j)=\delta_{ij}$. Since $|\alpha_1|^2=1$ and $|\alpha_2|^2=2$, solving gives

$$
\omega_1=\left(\frac12,\frac12\right),
\qquad \omega_2=(0,1).
$$

The full [B2 root system](../../../semisimple-lie-algebra.md#b2-root-system) is

$$
\{(\pm1,0),(0,\pm1),(\pm1,\pm1)\}.
$$

The [weight lattice](../../../semisimple-lie-algebra.md#weight-lattice) is generated by $\omega_1,omega_2$; geometrically it consists of the integer lattice together with the translate in which both coordinates are half-integers.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

The [Fundamental representations of B2](../../../semisimple-lie-algebra.md#fundamental-representations-of-b2) have weight sets

$$
d_{[1,0]}:\quad
\left\{\left(\frac12,\frac12\right),
\left(\frac12,-\frac12\right),
\left(-\frac12,\frac12\right),
\left(-\frac12,-\frac12\right)\right\},
$$

so $\dim d_{[1,0]}=4$, and

$$
d_{[0,1]}:\quad
\{(1,0),(-1,0),(0,1),(0,-1),(0,0)\},
$$

so $\dim d_{[0,1]}=5$. The [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) has all eight roots as nonzero weights and zero with multiplicity two. Its [highest root](../../../semisimple-lie-algebra.md#highest-root) is

$$
2\alpha_1+\alpha_2=(1,1)=2\omega_1,
$$

so its highest-weight label is $[2,0]$ and its dimension is $8+2=10$.

<h3 id="4/f">f</h3>

↑ **Parent:** [4](#4)

<h4 id="4/f/solution">Solution</h4>

↑ **Parent:** [F](#4/f)

Using $\mathfrak{so}_4\cong\mathfrak{su}_2\oplus\mathfrak{su}_2$, the five-dimensional vector representation restricts as

$$
d_{[0,1]}\to(\tfrac12,\tfrac12)\oplus(0,0),
$$

which is the $\mathbf4\oplus\mathbf1$ decomposition from part (c). The four-dimensional spin representation is naturally a representation of $\mathfrak{so}_5$ or $Spin(5)$ rather than an honest representation of $SO(5)$; it restricts as

$$
d_{[1,0]}\to(\tfrac12,0)\oplus(0,\tfrac12),
$$

the two chiral spin representations of $\mathfrak{so}_4$. Finally,

$$
d_{[2,0]}\to(1,0)\oplus(0,1)\oplus(\tfrac12,\tfrac12),
$$

namely the two three-dimensional summands of the $SO(4)$ adjoint plus its four-dimensional vector, agreeing with $\mathbf{10}\to\mathbf6\oplus\mathbf4$ from the [SO5 to SO4 branching](../../../semisimple-lie-algebra.md#so5-to-so4-branching) calculation.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
