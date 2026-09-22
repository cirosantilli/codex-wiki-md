# Paper 302

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_302.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_302.pdf)

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
    - [i](#1/d/i)
      - [Solution](#1/d/i/solution)
    - [ii](#1/d/ii)
      - [Solution](#1/d/ii/solution)
    - [iii](#1/d/iii)
      - [Solution](#1/d/iii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
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
    - [v](#4/a/v)
      - [Solution](#4/a/v/solution)
    - [vi](#4/a/vi)
      - [Solution](#4/a/vi/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
    - [iii](#4/b/iii)
      - [Solution](#4/b/iii/solution)
  - [c](#4/c)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)
    - [iii](#4/c/iii)
      - [Solution](#4/c/iii/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)

## 1

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [Lie group](../../../lie-theory.md#lie-group) is a [smooth manifold](../../../differential-geometry.md#smooth-manifold) $G$ equipped with smooth maps $m:G\times G\to G$, $m(g,h)=gh$, and $\iota:G\to G$, $\iota(g)=g^{-1}$, for which multiplication is associative, there is an identity $e$, and every $g$ has the inverse $g^{-1}$. In equations,

$$
(gh)k=g(hk),\qquad eg=ge=g,\qquad gg^{-1}=g^{-1}g=e.
$$

**Thus the [group axioms](../../../group.md#group-axioms) and the smooth structure are compatible.**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

In a coordinate chart centred at the identity, smooth multiplication has a [local group law](../../../lie-theory.md#local-group-law)

$$
z^k=F^k(y,x)=x^k+y^k+B^k{}_{ij}y^ix^j+O(3).
$$

The identity gives $F(0,x)=x$ and $F(y,0)=y$, while [associativity](../../../group.md#associative-property) gives the functional equation $F(u,F(y,x))=F(F(u,y),x)$. Smooth inversion determines coordinates $\bar x$ with $F(\bar x,x)=F(x,\bar x)=0$. Changes of local coordinates alter the symmetric part of $B^k{}_{ij}$, whereas its antisymmetric part supplies the coordinate-independent [Lie bracket](../../../lie-algebra.md#lie-bracket) on the tangent space at the identity.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Write $g(x)=I+x^iT_i+O(x^2)$ in a [matrix representation](../../../representation-theory.md#matrix-representation) and $[T_i,T_j]=c^k{}_{ij}T_k$. Direct multiplication gives

$$
g(y)^{-1}g(x)^{-1}g(y)g(x)
=I+y^ix^j[T_i,T_j]+O(3),
$$

so

$$
w^k=c^k{}_{ij}y^ix^j+O(3)=-c^k{}_{ij}x^iy^j+O(3).
$$

The cancellation of the constant and linear terms explains why the [group commutator](../../../group.md#group-commutator) first detects the [Lie bracket](../../../lie-algebra.md#lie-bracket) at quadratic order.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The matrix is invertible precisely when $a\ne0$, and

$$
\begin{pmatrix}a&b\\0&1\end{pmatrix}^{-1}
=\begin{pmatrix}a^{-1}&-a^{-1}b\\0&1\end{pmatrix}.
$$

The largest group is therefore

$$
G=\left\{\begin{pmatrix}a&b\\0&1\end{pmatrix}:a\in\mathbb R^*,\ b\in\mathbb R\right\},
$$

the [real affine group](../../../lie-theory.md#orientation-preserving-affine-group-of-the-real-line) $\mathbb R\rtimes\mathbb R^*$ under $(a,b)(a',b')=(aa',b+ab')$.

<h4 id="1/d/i">i</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/i/solution">Solution</h5>

↑ **Parent:** [I](#1/d/i)

As a [smooth manifold](../../../differential-geometry.md#smooth-manifold), $G\cong\mathbb R^*\times\mathbb R$. It has two [connected components](../../../geometry-and-topology.md#connected-component), distinguished by the sign of $a$: each of $a>0$ and $a<0$ is connected, and a continuous path in $G$ cannot cross $a=0$.

<h4 id="1/d/ii">ii</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/d/ii)

The defining two-dimensional [group representation](../../../representation-theory.md#group-representation) is [reducible](../../../representation-theory.md#reducible-representation), because the line $\mathbb Re_1$ is an [invariant subspace](../../../representation-theory.md#invariant-subspace):

$$
\begin{pmatrix}a&b\\0&1\end{pmatrix}e_1=ae_1.
$$

For $b\ne0$, the complementary line $\mathbb Re_2$ is not invariant, so this representation need not split as a [direct sum](../../../vector-space.md#direct-sum) of one-dimensional representations.

<h4 id="1/d/iii">iii</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/d/iii)

The map $(a,b)\mapsto\operatorname{sgn}(a)$ is a surjective [group homomorphism](../../../group-theory.md#group-homomorphism) with kernel $H_0$, so $H_0$ is a [normal subgroup](../../../group-theory.md#normal-subgroup) and $G/H_0\cong C_2$. The subgroup $H_1$ is not normal: for a translation $t=(1,c)$,

$$
t(a,0)t^{-1}=(a,c(1-a)),
$$

which leaves $H_1$ when $a\ne1$ and $c\ne0$. Finally, $(a,b)\mapsto a$ is a surjective homomorphism onto $\mathbb R^*$ with kernel $H_2$, so $H_2\triangleleft G$ and the [quotient group](../../../group-theory.md#quotient-group) $G/H_2\cong\mathbb R^*$.

## 2

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

With $\eta=\operatorname{diag}(1,-1,-1)$, the defining condition for the $(1+2)$-dimensional [Lorentz group](../../../special-relativity.md#lorentz-group) is

$$
\Lambda^T\eta\Lambda=\eta.
$$

Taking [determinants](../../../linear-algebra.md#determinant) gives $(\det\Lambda)^2=1$, hence $\det\Lambda=\pm1$. The norm of the zeroth column gives

$$
(\Lambda^0{}_0)^2-(\Lambda^1{}_0)^2-(\Lambda^2{}_0)^2=1,
$$

so $|\Lambda^0{}_0|\geq1$. The [Proper orthochronous Lorentz group](../../../special-relativity.md#proper-orthochronous-lorentz-group) is the component with $\det\Lambda=1$ and $\Lambda^0{}_0\geq1$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Identify $x=(x^0,x^1,x^2)$ with the real symmetric matrix

$$
X=\phi(x)=\begin{pmatrix}x^0+x^1&x^2\\x^2&x^0-x^1\end{pmatrix},
\qquad \det X=(x^0)^2-(x^1)^2-(x^2)^2.
$$

For $A\in SL(2,\mathbb R)$, define $X\mapsto AXA^T$. This linear action preserves $\det X$, so it defines $\rho(A)\in SO^+(1,2)$, and $\rho(AB)=\rho(A)\rho(B)$. Its kernel is $\{\pm I\}$ and it is onto, hence it is a two-to-one [covering homomorphism](../../../group-theory.md#covering-homomorphism) rather than an [isomorphism](../../../algebra.md#isomorphism). Consequently $PSL(2,\mathbb R)=SL(2,\mathbb R)/\{\pm I\}\cong SO^+(1,2)$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The connected $(1+2)$-dimensional [Poincaré group](../../../special-relativity.md#poincare-group) is

$$
ISO^+(1,2)=\mathbb R^{1,2}\rtimes SO^+(1,2),
\qquad
(a,\Lambda)(b,M)=(a+\Lambda b,\Lambda M).
$$

The [semidirect product](../../../group-theory.md#semidirect-product) records that Lorentz transformations act nontrivially on translations, which is what organizes momentum orbits. For a representative momentum $p$, its [little group](../../../special-relativity.md#little-group) is the stabilizer $G_p=\{\Lambda\in SO^+(1,2):\Lambda p=p\}$. [Wigner's classification](../../../special-relativity.md#wigner-s-classification) constructs irreducible particle representations by inducing a unitary irreducible representation of $G_p$ along the Lorentz orbit of $p$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

For a massive positive-energy orbit, choose $p_*=(m,0,0)$ with $m>0$. Its [little group](../../../special-relativity.md#little-group) is $SO(2)$, whose [unitary irreducible representations](../../../representation-theory.md#unitary-irreducible-representation) are the characters $e^{is\theta}$. Induction gives one-particle states $|p,s\rangle$ on the mass shell $p^2=m^2$, $p^0>0$, labeled by mass and spin. For the Poincare group itself, single-valuedness gives $s\in\mathbb Z$; its double cover permits half-integers, and its universal cover permits any real $s$, producing [anyonic spin](../../../topological-quantum-matter.md#anyon) in $(2+1)$ dimensions.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

For the positive-energy massless orbit choose $k=(E,E,0)$. Its connected [little group](../../../special-relativity.md#little-group) is the one-parameter group of null rotations, isomorphic to $(\mathbb R,+)$. Its unitary irreducible representations are the characters $t\mapsto e^{i\rho t}$, $\rho\in\mathbb R$, and induction gives the massless one-particle representations. The physically usual finite-component representation has trivial little-group action, $\rho=0$; there is no $SO(2)$ helicity subgroup for a null momentum in $(2+1)$ dimensions.

## 3

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [special unitary group](../../../topological-group.md#special-unitary-group) is $SU(2)=\{U\in M_2(\mathbb C):U^\dagger U=I,\ \det U=1\}$. Differentiating these equations at the identity shows that its [Lie algebra](../../../lie-algebra.md) is

$$
\mathfrak{su}(2)=\{X:X^\dagger=-X,\ \operatorname{tr}X=0\}.
$$

For $T_i=-i\sigma_i/2$, the [Pauli-matrix](../../../algebra.md#pauli-matrices) identity $[\sigma_i,\sigma_j]=2i\epsilon_{ijk}\sigma_k$ gives

$$
[T_i,T_j]=\epsilon_{ijk}T_k,
$$

so the [structure constants](../../../lie-algebra.md#structure-constant-of-a-lie-algebra) in this basis are $c^k{}_{ij}=\epsilon_{ijk}$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [Cartan-Weyl basis](../../../semisimple-lie-algebra.md#cartan-weyl-basis) obeys

$$
[H,E_\pm]=\pm2E_\pm,\qquad [E_+,E_-]=H.
$$

For a highest-weight vector $|\Lambda\rangle$, $E_+|\Lambda\rangle=0$ and $H|\Lambda\rangle=\Lambda|\Lambda\rangle$. Successive nonzero [lowerings](../../../semisimple-lie-algebra.md#lowering-operator) give the [weight basis](../../../semisimple-lie-algebra.md#weight-vector)

$$
|\Lambda-2k\rangle\ \propto\ E_-^k|\Lambda\rangle,
\qquad k=0,1,\ldots,\Lambda.
$$

Finite dimensionality requires the [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) $\Lambda$ to be a nonnegative integer. The weights are $\Lambda,\Lambda-2,\ldots,-\Lambda$, each with multiplicity one, so $\dim d_\Lambda=\Lambda+1$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

In the defining representation,

$$
H=\begin{pmatrix}1&0\\0&-1\end{pmatrix},\quad
E_+=\begin{pmatrix}0&1\\0&0\end{pmatrix},\quad
E_-=\begin{pmatrix}0&0\\1&0\end{pmatrix}.
$$

Multiplying the three factors in the [disentangling identity](../../../semisimple-lie-algebra.md#disentangling-identity) and comparing with $e^{i\theta\sigma_1/2}$ gives

$$
\alpha=\gamma=\tan\frac\theta2,
\qquad
\exp\!\left(\frac{i\beta H}{2}\right)
=\begin{pmatrix}\cos(\theta/2)&0\\0&\sec(\theta/2)\end{pmatrix}.
$$

This factorization is the coordinate patch where $\cos(\theta/2)\ne0$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Since $-\theta T_1=i\theta\sigma_1/2$, the same [disentangling identity](../../../semisimple-lie-algebra.md#disentangling-identity) applies in every [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation). The rightmost $E_+$ kills $|\Lambda\rangle$, the leftmost $E_-$ kills $\langle\Lambda|$, and the middle factor acts by its highest weight. Therefore

$$
\boxed{\langle\Lambda|e^{-\theta d(T_1)}|\Lambda\rangle
=\left(\cos\frac\theta2\right)^\Lambda.}
$$

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Because $d(T_1)$ commutes with itself and is anti-Hermitian,

$$
\langle\varphi|\theta\rangle
=\langle\Lambda|e^{\varphi d(T_1)}e^{-\theta d(T_1)}|\Lambda\rangle
=\langle\Lambda|e^{-(\theta-\varphi)d(T_1)}|\Lambda\rangle.
$$

Applying the preceding highest-weight matrix coefficient yields

$$
\boxed{\langle\varphi|\theta\rangle
=\left[\cos\frac{\theta-\varphi}{2}\right]^\Lambda}.
$$

## 4

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

For simple roots $\alpha_i$, the [Cartan matrix](../../../semisimple-lie-algebra.md#cartan-matrix) is

$$
A_{ij}=\langle\alpha_i,\alpha_j^\vee\rangle
=\frac{2(\alpha_i,\alpha_j)}{(\alpha_j,\alpha_j)}.
$$

Its diagonal entries are two, while its off-diagonal entries encode the angles and relative lengths in the [Dynkin diagram](../../../semisimple-lie-algebra.md#dynkin-diagram).

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

The [fundamental weights](../../../semisimple-lie-algebra.md#fundamental-weight) $\omega_i$ are the basis dual to the simple coroots:

$$
\boxed{\langle\omega_i,\alpha_j^\vee\rangle=\delta_{ij}.}
$$

<h4 id="4/a/iii">iii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/a/iii)

The [Dynkin labels](../../../semisimple-lie-algebra.md#dynkin-label) of a weight $\lambda$ are

$$
[\lambda^1,\ldots,\lambda^r],
\qquad
\lambda^i=\langle\lambda,\alpha_i^\vee\rangle,
$$

so $\lambda=\sum_i\lambda^i\omega_i$.

<h4 id="4/a/iv">iv</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#4/a/iv)

A [dominant weight](../../../semisimple-lie-algebra.md#dominant-weight) has nonnegative Dynkin labels. A [dominant integral weight](../../../semisimple-lie-algebra.md#dominant-integral-weight) additionally lies in the [weight lattice](../../../semisimple-lie-algebra.md#weight-lattice), so all those labels are nonnegative integers.

<h4 id="4/a/v">v</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/v/solution">Solution</h5>

↑ **Parent:** [V](#4/a/v)

The [highest weight of a representation](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) is the weight $\Lambda$ of a nonzero [weight vector](../../../semisimple-lie-algebra.md#weight-vector) annihilated by every positive-root operator. Every other weight is obtained from $\Lambda$ by subtracting a nonnegative integer combination of [simple roots](../../../semisimple-lie-algebra.md#simple-root). A finite-dimensional irreducible representation of a complex semisimple Lie algebra is determined by its dominant integral highest weight.

<h4 id="4/a/vi">vi</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/vi/solution">Solution</h5>

↑ **Parent:** [Vi](#4/a/vi)

Pairing $\alpha_i=\sum_jc_{ij}\omega_j$ with $\alpha_k^\vee$ gives $c_{ik}=A_{ik}$. Hence the relation between the two bases is

$$
\boxed{\alpha_i=\sum_jA_{ij}\omega_j}.
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

With $A_{ij}=2(\alpha_i,\alpha_j)/(\alpha_j,\alpha_j)$ and roots labeled from left to right, the three [Cartan matrices](../../../semisimple-lie-algebra.md#cartan-matrix) are

$$
A(A_3)=\begin{pmatrix}2&-1&0\\-1&2&-1\\0&-1&2\end{pmatrix},\quad
A(B_3)=\begin{pmatrix}2&-1&0\\-1&2&-2\\0&-1&2\end{pmatrix},\quad
A(C_3)=\begin{pmatrix}2&-1&0\\-1&2&-1\\0&-2&2\end{pmatrix}.
$$

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

All roots of $A_3$ have the same length, so $|\alpha_2|/|\alpha_3|=1$. In $B_3$, $\alpha_2$ is long and $\alpha_3$ short, giving $\sqrt2$. In $C_3$ their roles are reversed, giving $1/\sqrt2$. These ratios also follow from $A_{23}/A_{32}=|\alpha_2|^2/|\alpha_3|^2$.

<h4 id="4/b/iii">iii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/b/iii)

Disconnected nodes in a [Dynkin diagram](../../../semisimple-lie-algebra.md#dynkin-diagram) represent orthogonal roots, so $\angle(\alpha_1,\alpha_3)=90^\circ$ in all three cases. A single edge gives $120^\circ$, hence $\angle(\alpha_1,\alpha_2)=120^\circ$ and, for $A_3$, also $\angle(\alpha_2,\alpha_3)=120^\circ$. The double edge in both $B_3$ and $C_3$ gives $\angle(\alpha_2,\alpha_3)=135^\circ$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

Starting from $[1,0,0]$ and applying the simple-root [lowerings](../../../semisimple-lie-algebra.md#lowering-operator) gives the four weights

$$
[1,0,0],\quad[-1,1,0],\quad[0,-1,1],\quad[0,0,-1].
$$

Each has [weight multiplicity](../../../semisimple-lie-algebra.md#weight-multiplicity) one, so $d_1$ is the four-dimensional defining representation of $A_3\cong\mathfrak{sl}_4(\mathbb C)$.

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

The representation with highest weight $[0,0,1]$ is the [dual representation](../../../representation-theory.md#dual-representation) of $d_1$. Its weights are the negatives of those of $d_1$:

$$
[0,0,1],\quad[0,1,-1],\quad[1,-1,0],\quad[-1,0,0].
$$

**Thus $\dim d_2=4$.**

<h4 id="4/c/iii">iii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/c/iii)

For $B_3\cong\mathfrak{so}_7(\mathbb C)$, the highest weight $[0,0,1]$ is the [spinor representation](../../../semisimple-lie-algebra.md#spin-representation). Its eight weights, all of multiplicity one, are

$$
\begin{gathered}
[0,0,1],\ [0,1,-1],\ [1,-1,1],\ [1,0,-1],\\
[-1,0,1],\ [-1,1,-1],\ [0,-1,1],\ [0,0,-1].
\end{gathered}
$$

Equivalently, in an orthonormal basis they are $(\pm e_1\pm e_2\pm e_3)/2$ with independent signs. Hence $\dim d_3=8$.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The tensor product of the defining representation and its dual is the endomorphism representation. Splitting an endomorphism into its [matrix trace](../../../linear-algebra.md#matrix-trace) and traceless part gives

$$
d_1\otimes d_2\cong\mathbf4\otimes\overline{\mathbf4}
=\mathbf1\oplus\mathbf{15}.
$$

In [Dynkin labels](../../../semisimple-lie-algebra.md#dynkin-label), the two irreducible summands have highest weights $[0,0,0]$ and $[1,0,1]$.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Applying $P[a,b,c]=[b,a,b+c]$ to the eight weights of $d_3$ gives

$$
\begin{gathered}
[0,0,1],\ [1,0,0],\ [-1,1,0],\ [0,1,-1],\\
[0,-1,1],\ [1,-1,0],\ [-1,0,0],\ [0,0,-1].
\end{gathered}
$$

This is exactly the union of the weight sets of $d_1$ and $d_2$. It expresses the [branching rule](../../../lie-algebra.md#branching-rule) for the standard inclusion $D_3\cong A_3\subset B_3$: the eight-dimensional spinor representation of $\mathfrak{so}_7$ restricts to the two four-dimensional chiral spinor representations of $\mathfrak{so}_6\cong\mathfrak{sl}_4$,

$$
\mathbf8\downarrow_{A_3}=\mathbf4\oplus\overline{\mathbf4}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
