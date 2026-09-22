# Paper 302

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_302.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_302.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
    - [iv](#1/b/iv)
      - [Solution](#1/b/iv/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
  - [f](#2/f)
    - [Solution](#2/f/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
    - [iii](#4/a/iii)
      - [Solution](#4/a/iii/solution)
    - [iv](#4/a/iv)
      - [Solution](#4/a/iv/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
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

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

The integers are closed under addition, addition is associative, zero is an identity, and $-n$ is the additive inverse of $n$. Thus $(\mathbb Z,+)$ is an [abelian group](../../../group.md#abelian-group).

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

The nonzero integers are closed under multiplication and contain the identity, but most elements have no inverse in the set: for example, the multiplicative inverse of $2$ is $1/2\notin\mathbb Z^*$. Hence $(\mathbb Z^*,\times)$ is not a group.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

Composition is associative, and

$$
(u,b)(u',b')=(uu',ub'+b)
$$

again has nonzero slope. The identity is $(1,0)$ and

$$
(u,b)^{-1}=(u^{-1},-u^{-1}b).
$$

**Thus these maps form the [real affine group](../../../lie-theory.md#orientation-preserving-affine-group-of-the-real-line) of the line, a nonabelian group.**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

In coordinates the [real Heisenberg group](../../../lie-algebra.md#heisenberg-group) law is

$$
(q,r,s)(q',r',s')=(q+q',r+r',s+s'+qr').
$$

Commuting this with every $(q',r',s')$ requires $qr'-q'r=0$ for all $q',r'$, hence $q=r=0$. Therefore

$$
\boxed{Z(G)=\{(0,0,s):s\in\mathbb R\}.}
$$

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

The Lie algebra consists of strictly upper-triangular matrices

$$
X=qQ+rR+sS,
\quad Q=E_{12},\quad R=E_{23},\quad S=E_{13}.
$$

The only nonzero basis bracket is $[Q,R]=S$. Thus the independent nonzero [structure constant of a Lie algebra](../../../lie-algebra.md#structure-constant-of-a-lie-algebra) values are $f_{QR}{}^S=1$ and $f_{RQ}{}^S=-1$.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

Since $X^3=0$,

$$
\exp(qQ+rR+tS)=I+qQ+rR+(t+qr/2)S.
$$

Every group element has the unique preimage $t=s-qr/2$, so the [Exponential map of a Lie group](../../../lie-theory.md#exponential-map-of-a-lie-group) is bijective. It is a diffeomorphism from $\mathbb R^3$ onto $G$, proving that $G$ is connected and simply connected.

<h4 id="1/b/iv">iv</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/b/iv)

The line $\mathbb RS$ is a nonzero central ideal, so the [Heisenberg Lie algebra](../../../lie-algebra.md#heisenberg-lie-algebra) is not simple. It is two-step nilpotent and hence solvable; a nonzero solvable Lie algebra is not semisimple. It is therefore neither simple nor semisimple.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Strictly, the normalized functions form the unit sphere rather than a vector space; let $V=L^2(\mathbb R)$ and restrict to normalized states when interpreting wavefunctions. The group law gives

$$
D(q,r,s)D(q',r',s')\psi(x)
=e^{-i(s+s'+qr')}e^{i(r+r')x}\psi(x-q-q')
=D(gg')\psi(x).
$$

Translation preserves Lebesgue measure and both exponential factors have unit modulus, so $D(g)$ preserves the inner product and is a [unitary representation](../../../representation-theory.md#unitary-representation). This is the [Schrödinger representation of the Heisenberg group](../../../lie-algebra.md#schrodinger-representation-of-the-heisenberg-group): $q$ translates position, $r$ translates momentum, and $s$ contributes the physically irrelevant overall phase.

## 2

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A [Lie bracket](../../../lie-algebra.md#lie-bracket) is bilinear, antisymmetric, and satisfies the [Jacobi identity](../../../lie-algebra.md#jacobi-identity). For a basis $T_a$,

$$
[T_a,T_b]=f_{ab}{}^cT_c.
$$

The [structure constant of a Lie algebra](../../../lie-algebra.md#structure-constant-of-a-lie-algebra) coefficients satisfy $f_{ab}{}^c=-f_{ba}{}^c$ and $f_{ab}{}^df_{dc}{}^e+f_{bc}{}^df_{da}{}^e+f_{ca}{}^df_{db}{}^e=0$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Conjugation differentiates to the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra)

$$
\operatorname{Ad}_gX=\left.\frac d{dt}\right|_{0}g\exp(tX)g^{-1}.
$$

Because conjugations compose, $\operatorname{Ad}_{gh}=\operatorname{Ad}_g\operatorname{Ad}_h$ and $\operatorname{Ad}_e=I$, so this is a group representation.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Differentiating $\operatorname{Ad}_{\exp(tX)}Y$ at zero gives the [Adjoint representation of a Lie algebra](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra)

$$
\operatorname{ad}_X(Y)=[X,Y].
$$

The Jacobi identity implies $[\operatorname{ad}_X,\operatorname{ad}_Y]=\operatorname{ad}_{[X,Y]}$, proving that it is a Lie-algebra representation.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Since $(\operatorname{ad}_{T_a})^c{}_b=f_{ab}{}^c$, the [Killing form](../../../lie-algebra.md#killing-form) has components

$$
\boxed{\kappa_{ab}=f_{ac}{}^d f_{bd}{}^c}.
$$

This is the matrix trace of $\operatorname{ad}_{T_a}\operatorname{ad}_{T_b}$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The displayed basis obeys $[\tau_a,\tau_b]=\epsilon_{abc}\tau_c$. Therefore

$$
\kappa(\tau_a,\tau_b)
=\epsilon_{ac d}\epsilon_{bd c}=-2\delta_{ab}.
$$

The basis is adapted to the Killing form in the usual orthogonal-basis sense, since its Gram matrix is diagonal; rescaling by $1/\sqrt2$ makes it orthonormal for $-\kappa$.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

The [complexification of a Lie algebra](../../../lie-algebra.md#complexification-of-a-lie-algebra) is $\mathfrak{su}(2)_{\mathbb C}=\mathfrak{su}(2)\otimes_{\mathbb R}\mathbb C\cong\mathfrak{sl}_2(\mathbb C)$. With $[H,E_\pm]=\pm2E_\pm$ and $[E_+,E_-]=H$, the Killing matrix in the ordered basis $(E_+,E_-,H)$ is

$$
\begin{pmatrix}0&4&0\\4&0&0\\0&0&8\end{pmatrix}.
$$

This Cartan-Weyl basis is adapted to the root decomposition, but it is not Killing-orthogonal because $\kappa(E_+,E_-)=4$.

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

Using the matrix-unit commutator and summing the adjoint indices gives

$$
\boxed{\kappa(X,Y)=2n\operatorname{tr}(XY)-2\operatorname{tr}(X)\operatorname{tr}(Y)}.
$$

Equivalently, in components this is $2nX^i{}_jY^j{}_i-2X^i{}_iY^j{}_j$. It vanishes on the scalar center, as expected because $\mathfrak{gl}_n$ is not semisimple.

## 3

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [Lorentz group](../../../special-relativity.md#lorentz-group) consists of linear maps $x\mapsto\Lambda x$ satisfying $\Lambda^T\eta\Lambda=\eta$. The [Poincaré group](../../../special-relativity.md#poincare-group) consists of affine isometries $x\mapsto\Lambda x+a$ and has multiplication

$$
(a,\Lambda)(b,M)=(a+\Lambda b,\Lambda M).
$$

**Thus it is the semidirect product $\mathbb R^{1,3}\rtimes O(1,3)$, with the Lorentz group as the subgroup fixing the spacetime origin.**

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

With cyclic spatial indices,

$$
J_1=M^{23},\quad J_2=M^{31},\quad J_3=M^{12},
\qquad K_i=M^{0i}.
$$

Substitution in the given [Poincare algebra](../../../special-relativity.md#poincare-algebra) brackets yields

$$
\boxed{[J_1,J_2]=J_3,
\qquad [J_1,K_2]=K_3,
\qquad [K_1,K_2]=-J_3.}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Because the translations commute, $P^\sigma P^\mu$ is symmetric in $(\sigma,\mu)$, whereas the Levi-Civita tensor in the [Pauli-Lubanski pseudovector](../../../special-relativity.md#pauli-lubanski-pseudovector) is antisymmetric, so $W_\mu P^\mu=0$. Moreover,

$$
[W_\mu,P^\tau]
=\frac12\epsilon_{\mu\nu\rho\sigma}
(\eta^{\rho\tau}P^\nu-\eta^{\nu\tau}P^\rho)P^\sigma=0,
$$

because the two terms cancel after relabeling and each remaining momentum product is symmetric.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

In the rest frame $P^\mu=(m,0,0,0)$, antisymmetry gives $W_0=0$. Taking $\epsilon_{0123}=+1$ and $J_3=M^{12}$ gives

$$
W_3=-mJ_3.
$$

Hence

$$
W_0|j,j_3\rangle=0,
\qquad
W_3|j,j_3\rangle=-m j_3|j,j_3\rangle.
$$

The sign of the second eigenvalue reverses if the opposite Levi-Civita convention is chosen.

## 4

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

A [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) of a complex semisimple Lie algebra is a maximal abelian subalgebra consisting of semisimple elements.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

For a Cartan subalgebra $\mathfrak h$, the root set consists of the nonzero linear functionals $\alpha\in\mathfrak h^*$ for which $\mathfrak g_\alpha=\{X:[H,X]=\alpha(H)X\}$ is nonzero. It is the [root system](../../../semisimple-lie-algebra.md#root-system) of the Lie algebra.

<h4 id="4/a/iii">iii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/a/iii)

A [root string](../../../semisimple-lie-algebra.md#root-string) through $\beta$ in the $\alpha$ direction is the uninterrupted sequence $\beta-p\alpha,\ldots,\beta+q\alpha$ of roots, with $p-q=\langle\beta,\alpha^\vee\rangle$.

<h4 id="4/a/iv">iv</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#4/a/iv)

For ordered simple roots, the [Cartan matrix](../../../semisimple-lie-algebra.md#cartan-matrix) is $A_{ij}=\langle\alpha_i,\alpha_j^\vee\rangle=2(\alpha_i,\alpha_j)/(\alpha_j,\alpha_j)$. It determines their relative lengths and angles.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

The first diagram is $D_4$, with central node $\alpha_2$. Its Cartan matrix is

$$
\begin{pmatrix}
2&-1&0&0\\-1&2&-1&-1\\0&-1&2&0\\0&-1&0&2
\end{pmatrix}.
$$

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

The second diagram is $F_4$; the arrow points from the long root $\alpha_2$ toward the short root $\alpha_3$. Thus

$$
\begin{pmatrix}
2&-1&0&0\\-1&2&-2&0\\0&-1&2&-1\\0&0&-1&2
\end{pmatrix}.
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [classification of rank-two root systems](../../../semisimple-lie-algebra.md#classification-of-rank-two-root-systems) gives $A_1\times A_1$, $A_2$, $B_2$, and $G_2$. The first is reducible and corresponds to a semisimple but nonsimple algebra. Hence the complex simple rank-two algebras are $A_2$, $B_2=C_2$, and $G_2$, so $N=3$.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

This is the [G2 root system](../../../semisimple-lie-algebra.md#g2-root-system), with $\alpha$ long and $\beta$ short. Its positive roots are

$$
\beta,\ \alpha,\ \alpha+\beta,\ \alpha+2\beta,\ \alpha+3\beta,\ 2\alpha+3\beta,
$$

and the full root set includes their negatives. Thus $\dim\mathfrak g=12+2=14$. Finally

$$
4\cos^2\theta=A_{12}A_{21}=3,
$$

and simple roots have obtuse angle, so $\theta=5\pi/6$.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

For $x\alpha+y\beta$, the simple-coroot coordinates are $2x-y$ and $-3x+2y$. Solving for the [fundamental weights](../../../semisimple-lie-algebra.md#fundamental-weight) gives

$$
\chi=2\alpha+3\beta,
\qquad
\omega=\alpha+2\beta.
$$

Hence $C_1=2$, $C_2=3$, and $C_3=2$. The weight $\omega$ is the fundamental weight of the short root, and its [highest-weight representation](../../../semisimple-lie-algebra.md#highest-weight-representation) is the seven-dimensional fundamental representation of $G_2$. Its weights are zero and the six short roots.

<h3 id="4/f">f</h3>

↑ **Parent:** [4](#4)

<h4 id="4/f/solution">Solution</h4>

↑ **Parent:** [F](#4/f)

Under $\mathfrak{sl}(2)_\alpha$, a root $x\alpha+y\beta$ has weight $2x-y$. Counting the twelve root spaces and the two-dimensional Cartan subalgebra gives multiplicities one at weights $\pm2$, four at $\pm1$, and four at zero. Therefore

$$
\mathfrak g\downarrow\mathfrak{sl}(2)_\alpha
=d_2\oplus4d_1\oplus3d_0.
$$

Under $\mathfrak{sl}(2)_\beta$, the weight is $-3x+2y$. The multiplicities are two at $\pm3$, one at $\pm2$, two at $\pm1$, and four at zero. Hence

$$
\mathfrak g\downarrow\mathfrak{sl}(2)_\beta
=2d_3\oplus d_2\oplus3d_0.
$$

The dimensions are respectively $3+4\cdot2+3=14$ and $2\cdot4+3+3=14$, verifying both direct-sum decompositions of the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
