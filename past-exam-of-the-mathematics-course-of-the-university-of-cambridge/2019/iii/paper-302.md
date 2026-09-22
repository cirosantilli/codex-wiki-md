# Paper 302

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_302.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_302.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [Lie group](../../../lie-theory.md#lie-group) is a [group](../../../group.md) that is also a [smooth manifold](../../../differential-geometry.md#smooth-manifold), with [differentiable](../../../analysis.md#differentiable-function) multiplication and inversion. A [Lie algebra](../../../lie-algebra.md) is a [vector space](../../../vector-space.md) with a bilinear alternating [Lie bracket](../../../lie-algebra.md#lie-bracket) satisfying the [Jacobi identity](../../../lie-algebra.md#jacobi-identity).

For a [Matrix Lie group](../../../lie-theory.md#matrix-lie-group) $G$, put $\mathfrak g=T_I G$. If $X,Y\in\mathfrak g$, the matrix [commutator](../../../lie-algebra.md#commutator) $[X,Y]=XY-YX$ again lies in $\mathfrak g$: the group commutator $e^{tX}e^{sY}e^{-tX}e^{-sY}$ lies in $G$, and the coefficient of $ts$ in its [matrix logarithm](../../../vector-space.md#matrix-logarithm) is $[X,Y]$. Bilinearity and antisymmetry are immediate, while associativity of matrix multiplication gives the Jacobi identity. Thus $T_I G$, with the commutator bracket, is the [Lie algebra of a matrix Lie group](../../../lie-algebra.md#lie-algebra-of-a-matrix-lie-group) $\mathcal L(G)$.

The [special linear group](../../../group-theory.md#special-linear-group) $SL(2,\mathbb R)$ is the inverse image of the regular value $1$ under the smooth [determinant](../../../linear-algebra.md#determinant) map, and multiplication and inversion are smooth. Differentiating $\det(I+tA)=1+t\operatorname{tr}A+O(t^2)$ shows that

$$
\mathcal L(SL(2,\mathbb R))=\mathfrak{sl}_2(\mathbb R)
=\left\{\begin{pmatrix}a&b\\c&-a\end{pmatrix}:a,b,c\in\mathbb R\right\}.
$$

The [Cayley-Hamilton theorem](../../../mathematics.md#cayley-hamilton-theorem) applied to a trace-zero two-by-two matrix gives

$$
\boxed{A^2=-\det(A)I_2.}
$$

The [exponential map of a matrix Lie group](../../../lie-theory.md#exponential-map-of-a-matrix-lie-group) is the [matrix exponential](../../../linear-operator-theory.md#matrix-exponential)

$$
\operatorname{Exp}(A)=e^A=\sum_{n=0}^{\infty}\frac{A^n}{n!}.
$$

Since $\det(e^A)=e^{\operatorname{tr}A}=1$, its image lies in $SL(2,\mathbb R)$. Put $d=\det A$. The identity $A^2=-dI$ sums the series explicitly. If $d>0$, with $r=\sqrt d$,

$$
e^A=\cos r\,I+\frac{\sin r}{r}A,
\qquad \operatorname{tr}(e^A)=2\cos r\geq-2.
$$

If $d=0$, the trace is $2$, while if $d<0$, with $r=\sqrt{-d}$,

$$
e^A=\cosh r\,I+\frac{\sinh r}{r}A,
\qquad \operatorname{tr}(e^A)=2\cosh r\geq2.
$$

Hence

$$
\boxed{\operatorname{tr}(\operatorname{Exp}A)\geq-2.}
$$

But $\operatorname{diag}(-2,-1/2)\in SL(2,\mathbb R)$ has trace $-5/2$. It is therefore outside the image, so **the exponential map is not surjective**.

## 2

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) $\mathfrak h$ of a finite-dimensional complex [semisimple Lie algebra](../../../semisimple-lie-algebra.md) is a maximal abelian subalgebra consisting of semisimple elements. The [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition) is

$$
\mathfrak g=\mathfrak h\oplus\bigoplus_{\alpha\in\Phi}\mathfrak g_\alpha,
\qquad
\mathfrak g_\alpha=\{X:[H,X]=\alpha(H)X\text{ for all }H\in\mathfrak h\},
$$

and the nonzero functionals $\alpha$ are the roots. A [Cartan-Weyl basis](../../../semisimple-lie-algebra.md#cartan-weyl-basis) consists of a basis $H_i$ of $\mathfrak h$ and root vectors $E_\alpha\in\mathfrak g_\alpha$. Its brackets have the form

$$
[H_i,H_j]=0,qquad [H_i,E_\alpha]=\alpha(H_i)E_\alpha,qquad
[E_\alpha,E_{-\alpha}]=H_\alpha,
$$

and $[E_\alpha,E_\beta]=N_{\alpha\beta}E_{\alpha+\beta}$ when $\alpha+\beta$ is a root, and zero when $\alpha+\beta$ is neither a root nor zero.

For the complexified [so4 Lie algebra](../../../semisimple-lie-algebra.md#so4-lie-algebra), take $H^1=T^{(12)}$ and $H^2=T^{(34)}$. Write

$$
A_1^\pm=T^{(13)}\pm T^{(24)},
\qquad
A_2^\pm=T^{(14)}\pm T^{(23)}.
$$

Direct use of the stated commutation relations gives

$$
\begin{array}{c|rrrr}
&A_1^+&A_1^-&A_2^+&A_2^-\\ \hline
\operatorname{ad}H^1&A_2^-&-A_2^+&A_1^-&-A_1^+\\
\operatorname{ad}H^2&-A_2^-&-A_2^+&A_1^-&A_1^+
\end{array}.
$$

The simultaneous [eigenvectors](../../../linear-operator-theory.md#eigenvector), hence the step generators, may be chosen as

$$
\begin{aligned}
E_{++}&=A_2^+-iA_1^-,& \alpha_{++}&=(i,i),\\
E_{+-}&=A_2^-+iA_1^+,& \alpha_{+-}&=(i,-i),\\
E_{-+}&=A_2^--iA_1^+,& \alpha_{-+}&=(-i,i),\\
E_{--}&=A_2^++iA_1^-,& \alpha_{--}&=(-i,-i).
\end{aligned}
$$

Thus the roots relative to $(H^1,H^2)$ are $(\pm i,\pm i)$. Replacing $H^a$ by $-iH^a$ gives the usual real coordinates $(\pm1,\pm1)$. The only nonzero brackets between step generators, apart from those obtained by antisymmetry, are

$$
\boxed{[E_{++},E_{--}]=4i(H^1+H^2),
\qquad [E_{+-},E_{-+}]=4i(H^1-H^2).}
$$

An [isomorphism](../../../algebra.md#isomorphism) of Lie algebras is a bijective [linear map](../../../vector-space.md#linear-map) preserving the Lie bracket. Define

$$
\begin{aligned}
J_1^\pm&=-\tfrac12(T^{(23)}\pm T^{(14)}),\\
J_2^\pm&=-\tfrac12(T^{(31)}\pm T^{(24)}),\\
J_3^\pm&=-\tfrac12(T^{(12)}\pm T^{(34)}).
\end{aligned}
$$

Then

$$
[J_i^\pm,J_j^\pm]=\epsilon_{ijk}J_k^\pm,
\qquad [J_i^+,J_j^-]=0.
$$

The two spans are commuting copies of the complexified $\mathfrak{su}_2$, and together contain all six basis elements of $\mathfrak{so}_4$. [Chiral decomposition of the complexified so4 Lie algebra](../../../semisimple-lie-algebra.md#chiral-decomposition-of-the-complexified-so4-lie-algebra) therefore gives

$$
\boxed{\mathfrak{so}_4(\mathbb C)\cong
\mathfrak{su}_2(\mathbb C)\oplus\mathfrak{su}_2(\mathbb C).}
$$

Under this isomorphism the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) is the direct sum of the adjoint representations of the two factors:

$$
\boxed{\mathbf6=(\mathbf3,\mathbf1)\oplus(\mathbf1,\mathbf3).}
$$

## 3

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The [root lattice](../../../semisimple-lie-algebra.md#root-lattice) is $Q=\sum_i\mathbb Z\alpha^{(i)}$. The [weight lattice](../../../semisimple-lie-algebra.md#weight-lattice) is

$$
P=\{\lambda:\langle\lambda,(\alpha^{(i)})^\vee\rangle\in\mathbb Z\text{ for every }i\}.
$$

Because every [Cartan integer](../../../semisimple-lie-algebra.md#cartan-integer) $\langle\alpha^{(j)},(\alpha^{(i)})^\vee\rangle$ is integral, $Q\subseteq P$. The [Dynkin labels](../../../semisimple-lie-algebra.md#dynkin-label) of $\lambda$ are

$$
[m_1,\ldots,m_r],
\qquad m_i=\langle\lambda,(\alpha^{(i)})^\vee\rangle.
$$

There are three isomorphism classes of complex simple rank-three Lie algebras: types [A3 root system](../../../semisimple-lie-algebra.md#a3-root-system)$A_3$, [B3 root system](../../../semisimple-lie-algebra.md#b3-root-system)$B_3$, and [C3 root system](../../../semisimple-lie-algebra.md#c3-root-system)$C_3$. Use the convention $A_{ij}=\langle\alpha^{(i)},(\alpha^{(j)})^\vee\rangle$, and order the chain as $1$--$2$--$3$ with $|\alpha^{(1)}|=|\alpha^{(2)}|$.


- For $A_3$, all roots have the same length and the diagram has two single edges. Its [Cartan matrix](../../../semisimple-lie-algebra.md#cartan-matrix) and angles are


$$
A_{A_3}=\begin{pmatrix}2&-1&0\\-1&2&-1\\0&-1&2\end{pmatrix},
\qquad
\theta_{12}=\theta_{23}=120^\circ,quad\theta_{13}=90^\circ,quad
\frac{|\alpha^{(2)}|}{|\alpha^{(3)}|}=1.
$$


- For $B_3$, take $\alpha^{(1)}=e_1-e_2$, $\alpha^{(2)}=e_2-e_3$, and $\alpha^{(3)}=e_3$. The double-edge arrow points to the short third root, and


$$
A_{B_3}=\begin{pmatrix}2&-1&0\\-1&2&-2\\0&-1&2\end{pmatrix},
\qquad
\theta_{12}=120^\circ,quad\theta_{23}=135^\circ,quad\theta_{13}=90^\circ,quad
\frac{|\alpha^{(2)}|}{|\alpha^{(3)}|}=\sqrt2.
$$


- For $C_3$, take $\alpha^{(1)}=e_1-e_2$, $\alpha^{(2)}=e_2-e_3$, and $\alpha^{(3)}=2e_3$. The double-edge arrow points to the short second root, and


$$
A_{C_3}=\begin{pmatrix}2&-1&0\\-1&2&-1\\0&-2&2\end{pmatrix},
\qquad
\theta_{12}=120^\circ,quad\theta_{23}=135^\circ,quad\theta_{13}=90^\circ,quad
\frac{|\alpha^{(2)}|}{|\alpha^{(3)}|}=\frac1{\sqrt2}.
$$

The Dynkin labels of a finite-dimensional [irreducible representation](../../../representation-theory.md#irreducible-representation) are those of its [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation). Thus $[1,0,0]$ means the [fundamental representation](../../../semisimple-lie-algebra.md#fundamental-representation) $V(\omega_1)$. The weights, written in Dynkin labels and in a lowering order, are

$$
\begin{array}{c|l|c}
\text{type}&\text{weight labels}&\dim V(\omega_1)\\ \hline
A_3&[1,0,0],[-1,1,0],[0,-1,1],[0,0,-1]&4\\
B_3&[1,0,0],[-1,1,0],[0,-1,2],[0,0,0],[0,1,-2],[1,-1,0],[-1,0,0]&7\\
C_3&[1,0,0],[-1,1,0],[0,-1,1],[0,1,-1],[1,-1,0],[-1,0,0]&6
\end{array}.
$$

For $A_3$ these are the weights of the defining representation of $\mathfrak{sl}_4$; for $B_3$ they are $\{\pm e_1,\pm e_2,\pm e_3,0\}$ in the vector representation of $\mathfrak{so}_7$; for $C_3$ they are $\{\pm e_1,\pm e_2,\pm e_3\}$ in the defining representation of $\mathfrak{sp}_6$. Hence the requested dimensions are **$4$, $7$, and $6$**, respectively.

## 4

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $G$ be a simple [Lie group](../../../lie-theory.md#lie-group), let $T^a$ be Hermitian matrices for a finite-dimensional [unitary representation](../../../representation-theory.md#unitary-representation) $R$, and normalize

$$
[T^a,T^b]=if^{ab}{}_cT^c,
\qquad \operatorname{tr}(T^aT^b)=T(R)\delta^{ab}.
$$

A matter field $\psi$ transforms locally as $\psi'(x)=U(x)\psi(x)$, where $U(x)=e^{ig\epsilon^a(x)T^a}$. An ordinary derivative of $\psi$ does not transform covariantly because it differentiates $U$. Introduce a [gauge field](../../../relativistic-quantum-field.md#gauge-field) $A_\mu=A_\mu^aT^a$ and the [gauge covariant derivative](../../../relativistic-quantum-field.md#gauge-covariant-derivative)

$$
D_\mu=\partial_\mu-igA_\mu.
$$

Demanding $D_\mu'\psi'=U D_\mu\psi$ determines the [Yang-Mills gauge transformation](../../../relativistic-quantum-field.md#yang-mills-gauge-transformation)

$$
A_\mu'=UA_\mu U^{-1}-\frac{i}{g}(\partial_\mu U)U^{-1}.
$$

To first order in $\epsilon$,

$$
\boxed{\delta A_\mu=\partial_\mu\epsilon+ig[\epsilon,A_\mu],
\qquad
\delta A_\mu^a=\partial_\mu\epsilon^a+g f^{bc}{}_aA_\mu^b\epsilon^c.}
$$

The [gauge field strength](../../../relativistic-quantum-field.md#gauge-field-strength) is defined by $[D_\mu,D_\nu]=-igF_{\mu\nu}$:

$$
F_{\mu\nu}
=\partial_\mu A_\nu-\partial_\nu A_\mu-ig[A_\mu,A_\nu],
$$

or, in components,

$$
F_{\mu\nu}^a
=\partial_\mu A_\nu^a-\partial_\nu A_\mu^a
+g f^{bc}{}_aA_\mu^bA_\nu^c.
$$

Covariance of the commutator gives

$$
F_{\mu\nu}'=UF_{\mu\nu}U^{-1},
\qquad
\delta F_{\mu\nu}=ig[\epsilon,F_{\mu\nu}].
$$

The commutator term distinguishes [Yang-Mills theory](../../../relativistic-quantum-field.md#yang-mills-theory) from an [Abelian gauge theory](../../../relativistic-quantum-field.md#abelian-gauge-theory) and produces cubic and quartic gauge-boson interactions.

For a [Dirac field](../../../relativistic-quantum-field.md#dirac-field) of mass $m$ in $R$, the Lagrangian is

$$
\boxed{\mathcal L
=-\frac14F_{\mu\nu}^aF^{a\mu\nu}
+\bar\psi(i\gamma^\mu D_\mu-m)\psi.}
$$

Equivalently, the gauge term is proportional to $-\operatorname{tr}(F_{\mu\nu}F^{\mu\nu})$. The [cyclic property of the trace](../../../linear-algebra.md#cyclic-property-of-the-trace) and $F'_{\mu\nu}=UF_{\mu\nu}U^{-1}$ make it invariant. Unitarity gives $\bar\psi'=\bar\psi U^{-1}$, while $D_\mu'\psi'=UD_\mu\psi$, so both the matter kinetic term and mass term are invariant. A complex scalar $\phi$ in a unitary representation may instead be coupled through

$$
\mathcal L_\phi=(D_\mu\phi)^\dagger D^\mu\phi-V(\phi),
$$

provided the [scalar potential](../../../quantum-field-theory.md#scalar-potential) $V$ is $G$-invariant.

The simplicity assumption means that the [Lie algebra](../../../lie-algebra.md) $\mathfrak g$ is nonabelian and has no proper nonzero [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra). Its [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) is therefore irreducible, and every invariant symmetric bilinear form is proportional to the [Killing form](../../../lie-algebra.md#killing-form). Consequently the pure gauge kinetic term has one overall [gauge coupling](../../../relativistic-quantum-field.md#gauge-coupling) for a simple factor. The theory has no independent Abelian gauge direction; if the gauge algebra were a direct sum of simple and Abelian ideals, each factor could instead carry its own coupling. A simple group may still have a discrete center, but this does not add a gauge boson because gauge bosons are indexed by the Lie algebra.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
