# Paper 302

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_302.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_302.pdf)

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
  - [f](#1/f)
    - [Solution](#1/f/solution)
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
    - [i](#3/d/i)
      - [Solution](#3/d/i/solution)
    - [ii](#3/d/ii)
      - [Solution](#3/d/ii/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The matrices are rotations about the third coordinate axis. Direct multiplication gives

$$
g(\theta)g(\varphi)=g(\theta+\varphi\bmod 2\pi),
\qquad g(0)=I,
\qquad g(\theta)^{-1}=g(-\theta),
$$

and $g(\theta)^{\mathsf T}g(\theta)=I$. Thus they form a [one-parameter subgroup](../../../lie-theory.md#one-parameter-subgroup) of the [orthogonal group](../../../linear-algebra.md#orthogonal-group) $O(3)$, isomorphic to the [circle group](../../../lie-theory.md#circle-group).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

If $X$ belongs to the [Special orthogonal Lie algebra](../../../semisimple-lie-algebra.md#special-orthogonal-lie-algebra), which is also the Lie algebra of $O(3)$, then $e^{tX}\in O(3)$ near $t=0$. Differentiating

$$
e^{tX^{\mathsf T}}e^{tX}=I
$$

at zero gives $X^{\mathsf T}+X=0$. Conversely, the [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) of every real [skew-symmetric matrix](../../../linear-algebra.md#skew-symmetric-matrix) is orthogonal. Hence

$$
\boxed{\mathfrak o(3)=\{X\in M_3(\mathbb R):X^{\mathsf T}=-X\}.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For $A\in O(3)$ and $X^{\mathsf T}=-X$,

$$
(AXA^{\mathsf T})^{\mathsf T}=AX^{\mathsf T}A^{\mathsf T}=-AXA^{\mathsf T},
$$

so $\operatorname{Ad}_A$ maps $\mathfrak o(3)$ into itself. Moreover,

$$
\operatorname{Ad}_{AB}(X)
=ABX(AB)^{\mathsf T}
=A(BXB^{\mathsf T})A^{\mathsf T}
=(\operatorname{Ad}_A\circ\operatorname{Ad}_B)(X).
$$

It also sends the identity to the identity linear map, so $A\mapsto\operatorname{Ad}_A$ is the [Adjoint representation of a Lie group](../../../lie-theory.md#adjoint-representation-of-a-lie-group).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For a smooth [Lie-group representation](../../../lie-theory.md#lie-group-representation) $D:G\to GL(V)$, define its [derived representation](../../../lie-theory.md#derived-representation)

$$
dD(X)=\left.\frac d{dt}\right|_{t=0}D(e^{tX}).
$$

Differentiation makes $dD$ linear. Applying $D$ to the group commutator curve

$$
e^{tX}e^{sY}e^{-tX}e^{-sY}
$$

and taking the mixed derivative at $(0,0)$ gives

$$
dD([X,Y])=[dD(X),dD(Y)].
$$

**Thus $dD:\mathfrak g\to\mathfrak{gl}(V)$ is a [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation).**

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Differentiate $\operatorname{Ad}_{e^{tX}}Y=e^{tX}Ye^{-tX}$ at zero. This gives the [Adjoint representation of a Lie algebra](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra)

$$
\operatorname{ad}_X(Y)=[X,Y]=XY-YX.
$$

The [Jacobi identity](../../../lie-algebra.md#jacobi-identity) is exactly

$$
[\operatorname{ad}_X,\operatorname{ad}_Y]
=\operatorname{ad}_{[X,Y]},
$$

so this is a Lie-algebra representation on $\mathfrak o(3)$.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

The [Exponential map of a Lie group](../../../lie-theory.md#exponential-map-of-a-lie-group) sends $X\in\mathfrak o(3)$ to $e^X\in SO(3)$ and is a local diffeomorphism at zero. Every element of $SO(3)$ is an exponential of a skew-symmetric matrix, but no determinant-$-1$ element of $O(3)$ is an exponential because $\det e^X=e^{\operatorname{tr}X}=1$.

A representation $d:\mathfrak o(3)\to\mathfrak{gl}(V)$ always integrates uniquely to the simply connected covering group $\operatorname{Spin}(3)\simeq SU(2)$. It descends to $SO(3)$ exactly when the nontrivial element in the kernel of $SU(2)\to SO(3)$ acts trivially. Extending it further to disconnected $O(3)$ requires an additional parity operator compatible with conjugation by a reflection. Thus the Lie-algebra representation alone need not define a representation of all of $O(3)$.

## 2

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Define the [ladder operators](../../../semisimple-lie-algebra.md#ladder-operator) $J_\pm=J_1\pm iJ_2$. The [SU(2) Lie algebra](../../../semisimple-lie-algebra.md#su-2-lie-algebra) relations imply

$$
[J_3,J_\pm]=\pm J_\pm,
\qquad
[J_+,J_-]=2J_3.
$$

Thus $d(J_\pm)v_m$ has weight $m\pm1$ when nonzero. Starting from a maximum-weight vector $v_I$, repeated lowering gives weights

$$
I,I-1,\ldots,-I.
$$

The norm formula derived from the [Casimir element](../../../semisimple-lie-algebra.md#casimir-element),

$$
\lVert J_-|I,m\rangle\rVert^2=(I+m)(I-m+1),
$$

shows that lowering stops precisely at $m=-I$. Therefore $2I$ is a nonnegative integer and the irreducible representation has dimension $2I+1$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

With normalized states and $J_-^\dagger=J_+$,

$$
J_-|I,m\rangle
=\sqrt{(I+m)(I-m+1)}\,|I,m-1\rangle.
$$

Put $n=I-m$. Iterating from the highest-weight state gives

$$
(d(J_-))^n|I,I\rangle
=\sqrt{\prod_{r=0}^{n-1}(2I-r)(r+1)}\,|I,m\rangle
=\sqrt{\frac{(2I)!(I-m)!}{(I+m)!}}\,|I,m\rangle.
$$

Hence

$$
A(I,m)=\sqrt{\frac{(I+m)!}{(2I)!(I-m)!}},
$$

where the factorial arguments are integers because $I\pm m\in\mathbb Z_{\geq0}$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The transformed generators are

$$
J'_1=-J_1,
\qquad J'_2=J_2,
\qquad J'_3=-J_3.
$$

For example,

$$
[J'_1,J'_2]=[-J_1,J_2]=-iJ_3=iJ'_3.
$$

The other two cyclic commutators work identically, so

$$
[J'_i,J'_j]=i\epsilon_{ijk}J'_k.
$$

Conjugation by $C$ is therefore an [automorphism of a Lie algebra](../../../lie-algebra.md#automorphism-of-a-lie-algebra).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Since $CJ_3C^{-1}=-J_3$, the operator $C$ sends a weight-$m$ state to a weight-$-m$ state. Also

$$
CJ_-C^{-1}=-(J_1+iJ_2)=-J_+.
$$

For the spin-one normalization,

$$
|1,0\rangle=\frac1{\sqrt2}J_-|1,1\rangle,
\qquad
|1,-1\rangle=\frac1{\sqrt2}J_-|1,0\rangle.
$$

Write $C|1,1\rangle=a|1,-1\rangle$. Using $C|1,0\rangle=|1,0\rangle$ in the first relation gives $a=-1$, and applying $C$ to the second gives the other phase. Therefore, in the stated phase convention,

$$
C|\pi^+\rangle=-|\pi^-\rangle,
\qquad
C|\pi^-\rangle=-|\pi^+\rangle.
$$

A simultaneous phase redefinition of the charged pion states changes both displayed signs but not their physical interchange under [charge conjugation](../../../quantum-field-theory.md#charge-conjugation).

## 3

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) $\mathfrak h$ of a complex semisimple Lie algebra is a maximal commuting subalgebra consisting of semisimple elements. A nonzero functional $\alpha\in\mathfrak h^*$ is a root when its space in the [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition)

$$
\mathfrak g_\alpha
=\{X:[H,X]=\alpha(H)X\text{ for every }H\in\mathfrak h\}
$$

is nonzero. A [Cartan-Weyl basis](../../../semisimple-lie-algebra.md#cartan-weyl-basis) combines a basis of $\mathfrak h$ with root vectors $E_\alpha\in\mathfrak g_\alpha$.

A choice of regular hyperplane divides roots into positive and negative roots. The [simple roots](../../../semisimple-lie-algebra.md#simple-root) are the positive roots that are not sums of two positive roots; they form a basis of the real root span. The [Cartan matrix](../../../semisimple-lie-algebra.md#cartan-matrix) is

$$
A_{ij}=\frac{2(\alpha_i,\alpha_j)}{(\alpha_j,\alpha_j)},
$$

up to the equivalent transposed indexing convention.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $\beta$ be a positive root. If it is not simple, it is a sum of two positive roots. Repeating this decomposition terminates because the height with respect to a regular positive functional strictly decreases, and it writes

$$
\beta=\sum_i n_i\alpha_i,
\qquad n_i\in\mathbb Z_{\geq0},
$$

with at least one $n_i>0$. Equivalently, one may repeatedly choose a simple root $\alpha_i$ with $(\beta,\alpha_i)>0$ and use the [root string](../../../semisimple-lie-algebra.md#root-string) to replace $\beta$ by the root $\beta-\alpha_i$.

For uniqueness, the simple roots are linearly independent. Therefore two such expansions have identical coefficients. Here “positive integer coefficients” must allow zero coefficients: a simple root itself has coefficient one on its own basis vector and zero on the others.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The matrix is the [Cartan matrix of type A3](../../../semisimple-lie-algebra.md#cartan-matrix-of-type-a3). The positive roots are

$$
\alpha_1,
\quad\alpha_2,
\quad\alpha_3,
\quad\alpha_1+\alpha_2,
\quad\alpha_2+\alpha_3,
\quad\alpha_1+\alpha_2+\alpha_3.
$$

Together with their negatives they form

$$
\Phi=\{\pm\alpha_1,\pm\alpha_2,\pm\alpha_3,
\pm(\alpha_1+\alpha_2),\pm(\alpha_2+\alpha_3),
\pm(\alpha_1+\alpha_2+\alpha_3)\},
$$

so $|\Phi|=12$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/i">i</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/i/solution">Solution</h5>

↑ **Parent:** [I](#3/d/i)

In [Dynkin label](../../../semisimple-lie-algebra.md#dynkin-label) coordinates, subtracting $\alpha_i$ subtracts row $i$ of the stated Cartan matrix. Starting from $(1,0,0)$ gives the weight chain

$$
(1,0,0)
\xrightarrow{-\alpha_1}(-1,1,0)
\xrightarrow{-\alpha_2}(0,-1,1)
\xrightarrow{-\alpha_3}(0,0,-1).
$$

These are the four weights of the defining representation of $A_3\cong\mathfrak{sl}_4$.

<h4 id="3/d/ii">ii</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/d/ii)

The highest weight $(0,1,0)$ gives the six-dimensional second [exterior power](../../../linear-algebra.md#exterior-power) of the defining representation. Adding each unordered pair of the four defining weights from part i gives

$$
\begin{gathered}
(0,1,0),\qquad
(1,-1,1),\qquad
(1,0,-1),\\
(-1,0,1),\qquad
(-1,1,-1),\qquad
(0,-1,0).
\end{gathered}
$$

There are no multiplicities, in agreement with the assumption in the question.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

For equal-length candidate roots, the required inner products are

$$
\alpha_1\mathbin\cdot\alpha_2=-1,
\qquad
\alpha_2\mathbin\cdot\alpha_3=-1,
\qquad
\alpha_1\mathbin\cdot\alpha_3=0,
\qquad
\lVert\alpha_i\rVert^2=2.
$$

Set A is invalid because $\alpha_1\mathbin\cdot\alpha_3=-1$ rather than zero; indeed its three vectors sum to zero and are not linearly independent. Set B has all the displayed inner products and is linearly independent, so it is valid. Set C is the standard realization

$$
e_1-e_2,
\quad e_2-e_3,
\quad e_3-e_4
$$

of the [A3 root system](../../../semisimple-lie-algebra.md#a3-root-system) and is also valid.

## 4

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Require

$$
(\partial_\mu+A'_\mu)(g\phi)=g(\partial_\mu+A_\mu)\phi
$$

for every $\phi$. Expanding and cancelling $g\partial_\mu\phi$ gives

$$
(\partial_\mu g)+A'_\mu g=gA_\mu.
$$

Right multiplication by $g^{-1}$ yields the [gauge-field transformation law](../../../relativistic-quantum-field.md#gauge-field-transformation-law)

$$
\boxed{A'_\mu=gA_\mu g^{-1}-(\partial_\mu g)g^{-1}.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The first term $gA_\mu g^{-1}$ lies in $\mathfrak g$ because the [adjoint action](../../../lie-theory.md#adjoint-representation-of-a-lie-group) preserves the Lie algebra. For the second, fix $x$ and consider the group curve $s\mapsto g(x+s e_\mu)g(x)^{-1}$ through the identity. Its tangent at zero is $(\partial_\mu g)g^{-1}$, so this is also in $\mathfrak g$. Since a [Lie algebra](../../../lie-algebra.md) is a vector space, $A'_\mu\in\mathfrak g$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Direct expansion gives

$$
[D_\mu,D_\nu]\phi
=\{\partial_\mu A_\nu-\partial_\nu A_\mu+[A_\mu,A_\nu]\}\phi
=F_{\mu\nu}\phi.
$$

Since $D'_\mu(g\phi)=gD_\mu\phi$,

$$
F'_{\mu\nu}(g\phi)
=[D'_\mu,D'_\nu](g\phi)
=g[D_\mu,D_\nu]\phi
=gF_{\mu\nu}\phi.
$$

Therefore the non-Abelian [gauge field strength](../../../relativistic-quantum-field.md#gauge-field-strength) transforms covariantly:

$$
\boxed{F'_{\mu\nu}=gF_{\mu\nu}g^{-1}.}
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The [Killing form](../../../lie-algebra.md#killing-form) is invariant under the adjoint action:

$$
\kappa(\operatorname{Ad}_gX,\operatorname{Ad}_gY)=\kappa(X,Y).
$$

Together with $F'_{\mu\nu}=\operatorname{Ad}_gF_{\mu\nu}$, this immediately gives

$$
\kappa(F'_{\mu\nu},F'^{\mu\nu})
=\kappa(F_{\mu\nu},F^{\mu\nu}),
$$

so every positive integral power $\mathcal L_1$ is gauge invariant.

The [adjoint covariant derivative](../../../relativistic-quantum-field.md#adjoint-covariant-derivative) obeys

$$
(D'_\mu F'_{\nu\rho})
=g(D_\mu F_{\nu\rho})g^{-1}.
$$

This follows either by substituting the transformation laws or by applying the covariance of $D'_\mu$ to an adjoint-valued field. A second use of invariance of the Killing form gives

$$
\kappa(D'_\mu F'_{\nu\rho},D'^{\mu}F'^{\nu\rho})
=\kappa(D_\mu F_{\nu\rho},D^{\mu}F^{\nu\rho}),
$$

which proves gauge invariance of $\mathcal L_2$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
