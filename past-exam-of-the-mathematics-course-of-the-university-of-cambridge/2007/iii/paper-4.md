# Paper 4

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper4.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper4.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)

## 1

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

All brackets belong to the line $\mathbb Cc$, and $[p,q]=c$ shows this line is exactly the first derived algebra. Since $c$ is central, the [derived series of a Lie algebra](../../../lie-algebra.md#derived-series-of-a-lie-algebra) is

$$
\boxed{\mathfrak g^{(0)}=\mathfrak g,\qquad
\mathfrak g^{(1)}=\mathbb Cc,\qquad\mathfrak g^{(2)}=0.}
$$

The [lower central series of a Lie algebra](../../../lie-algebra.md#lower-central-series-of-a-lie-algebra) is likewise

$$
\boxed{\gamma_1\mathfrak g=\mathfrak g,\qquad
\gamma_2\mathfrak g=\mathbb Cc,\qquad\gamma_3\mathfrak g=0.}
$$

For completeness, the [center of a Lie algebra](../../../lie-algebra.md#center-of-a-lie-algebra) is $\mathbb Cc$: an element $ap+bq+dc$ commutes with $p$ only if $b=0$, and with $q$ only if $a=0$. The [upper central series of a Lie algebra](../../../lie-algebra.md#upper-central-series-of-a-lie-algebra) is therefore $0\subset\mathbb Cc\subset\mathfrak g$, because the quotient by $\mathbb Cc$ is abelian. Thus the [Heisenberg Lie algebra](../../../lie-algebra.md#heisenberg-lie-algebra) is **nilpotent of class two and solvable of derived length two**. These properties are not mutually exclusive.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Let $V$ be a nonzero finite-dimensional [Irreducible Lie algebra representation](../../../lie-algebra.md#irreducible-lie-algebra-representation). Since $c$ is central, its action is a scalar $\lambda I$ by the [Schur lemma](../../../representation-theory.md#schur-s-lemma). Taking the trace of $[\rho(p),\rho(q)]=\rho(c)$ gives $0=\lambda\dim V$, so $\lambda=0$.

The actions of $p,q$ now commute. Choose an [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $a$ of $\rho(p)$. Its nonzero [eigenspace](../../../linear-operator-theory.md#eigenspace) is preserved by $\rho(q)$, which has an [eigenvector](../../../linear-operator-theory.md#eigenvector) there, with some [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $b$. The span of this common [eigenvector](../../../linear-operator-theory.md#eigenvector) is invariant under all of $\mathfrak g$. Irreducibility forces it to be the whole representation. Consequently

$$
\boxed{V=\mathbb C,\qquad \rho(p)=a,\quad\rho(q)=b,\quad\rho(c)=0,
\qquad(a,b)\in\mathbb C^2.}
$$

Conversely each such assignment is a one-dimensional [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) and hence irreducible. Distinct pairs give nonisomorphic representations. This classifies all finite-dimensional irreducible representations; none is faithful because all annihilate $c$.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Use the [Polynomial representation of the Heisenberg Lie algebra](../../../lie-algebra.md#polynomial-representation-of-the-heisenberg-lie-algebra) on $V=\mathbb C[x]$:

$$
\boxed{\rho(p)=\frac d{dx},\qquad\rho(q)f=xf,\qquad\rho(c)=I.}
$$

The product rule gives $[d/dx,x]f=f$, verifying the required bracket, and the identity commutes with both operators.

For irreducibility, let $W$ be a nonzero [invariant subspace](../../../representation-theory.md#invariant-subspace) and choose a nonzero [polynomial](../../../polynomial.md) of degree $d$ in it. Its $d$th derivative is a nonzero constant, so $1\in W$. Repeated multiplication by $x$ then puts every [monomial](../../../polynomial.md#monomial) in $W$, giving $W=\mathbb C[x]$.

For faithfulness, suppose $a\rho(p)+b\rho(q)+dI=0$. Applying this operator to $1$ gives $bx+d=0$, so $b=d=0$. Applying what remains to $x$ gives $a=0$. The representation is therefore **faithful and irreducible**. It is necessarily infinite-dimensional, by the finite-dimensional classification just proved.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

On $\mathbb C^3$ take the [matrix units](../../../vector-space.md#matrix-unit)

$$
\boxed{\rho(p)=E_{12},\qquad\rho(q)=E_{23},\qquad\rho(c)=E_{13}.}
$$

Their products give $[E_{12},E_{23}]=E_{13}$, while $E_{13}$ commutes with each of the other two. Thus this is a [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation). The three images are [linearly independent](../../../vector-space.md#linear-independence), so its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is zero: it is **faithful and finite-dimensional**. It is reducible, as expected from the classification in part ii; for example, the first coordinate line is invariant.

## 2

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Put $\bar i=2n+2-i$ and $o=n+1$. A [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) is

$$
\mathfrak t=\{H(t)=\operatorname{diag}(t_1,\ldots,t_n,0,-t_n,\ldots,-t_1)\},
\qquad e_i(H(t))=t_i.
$$

The defining matrix condition says $A_{ij}=-A_{\bar j,\bar i}$. Using the [matrix units](../../../vector-space.md#matrix-unit), the nonzero [root spaces](../../../semisimple-lie-algebra.md#root-space) have the following generators:

$$
\begin{array}{c|c}
\text{root}&\text{generator}\\\hline
e_i-e_j\ (i\ne j)&E_{ij}-E_{\bar j,\bar i}\\
e_i+e_j\ (i<j)&E_{i,\bar j}-E_{j,\bar i}\\
-e_i-e_j\ (i<j)&E_{\bar j,i}-E_{\bar i,j}\\
e_i&E_{i,o}-E_{o,\bar i}\\
-e_i&E_{o,i}-E_{\bar i,o}
\end{array}
$$

Commuting each generator with $H(t)$ gives its stated [weight](../../../semisimple-lie-algebra.md#weight-representation-theory). Together with $H_i=E_{ii}-E_{\bar i,\bar i}$, these matrices span the [Special orthogonal Lie algebra](../../../semisimple-lie-algebra.md#special-orthogonal-lie-algebra); there are $n+2n^2=n(2n+1)$ independent generators. Thus its decomposition as a [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) module is

$$
\boxed{\mathfrak g=\mathfrak t\oplus\bigoplus_{\alpha\in R}\mathfrak g_\alpha,
\quad\dim\mathfrak g_\alpha=1,\quad
R=\{\pm e_i\pm e_j:i<j\}\cup\{\pm e_i\}.}
$$

This is the [Bn root system](../../../semisimple-lie-algebra.md#bn-root-system). The upper-triangular generators select the [positive roots](../../../semisimple-lie-algebra.md#positive-root)

$$
\boxed{R^+=\{e_i-e_j,e_i+e_j:i<j\}\cup\{e_i:1\le i\le n\}.}
$$

Its [simple roots](../../../semisimple-lie-algebra.md#simple-root) and [highest root](../../../semisimple-lie-algebra.md#highest-root), for $n\ge2$, are

$$
\boxed{\alpha_i=e_i-e_{i+1}\ (i<n),\quad\alpha_n=e_n,
\qquad\theta=e_1+e_2=\alpha_1+2\alpha_2+\cdots+2\alpha_n.}
$$

To see the simplicity assertion, $e_i=\alpha_i+\cdots+\alpha_n$, while $e_i-e_j=\alpha_i+\cdots+\alpha_{j-1}$ and $e_i+e_j=\alpha_i+\cdots+\alpha_{j-1}+2\alpha_j+\cdots+2\alpha_n$. The coefficient pattern for $\theta$ dominates those of every [positive root](../../../semisimple-lie-algebra.md#positive-root).

Normalize the inner product so the $e_i$ are orthonormal. The [simple coroots](../../../semisimple-lie-algebra.md#simple-coroot) are $\alpha_i^\vee=\alpha_i$ for $i<n$ and $\alpha_n^\vee=2e_n$. Solving $\langle\omega_j,\alpha_i^\vee\rangle=\delta_{ij}$ gives the [fundamental weights](../../../semisimple-lie-algebra.md#fundamental-weight)

$$
\boxed{\omega_j=e_1+\cdots+e_j\ (j<n),\qquad
\omega_n=\frac12(e_1+\cdots+e_n).}
$$

In the half-sum of [positive roots](../../../semisimple-lie-algebra.md#positive-root), the coordinate $e_i$ occurs with total coefficient $2(n-i)+1$. Hence the [Weyl vector](../../../semisimple-lie-algebra.md#half-sum-of-positive-roots) is

$$
\boxed{\rho=\frac12\sum_{\alpha\in R^+}\alpha
=\sum_{i=1}^n\left(n-i+\frac12\right)e_i=\sum_{j=1}^n\omega_j.}
$$

The [Dynkin diagram](../../../semisimple-lie-algebra.md#dynkin-diagram) is a chain $\alpha_1,\ldots,\alpha_n$, with single bonds up to $\alpha_{n-1}$ and a double last bond pointing towards the short root $\alpha_n$. In the [Extended Dynkin diagram](../../../semisimple-lie-algebra.md#extended-dynkin-diagram), add $\alpha_0=-\theta$. For $n\ge3$, $(\alpha_0,\alpha_2)=-1$ and its inner product with every other [simple root](../../../semisimple-lie-algebra.md#simple-root) is zero, so it attaches to $\alpha_2$ by a single bond. For $n=2$, both long nodes $0,1$ attach by double bonds to short node $2$. These rules give the [Bn Dynkin diagram and affine extension](../../../semisimple-lie-algebra.md#bn-dynkin-diagram-and-affine-extension) drawn below.

For rank one, $R=\{\pm e_1\}$, $\alpha_1=\theta=e_1$, $\omega_1=e_1/2$, and $\rho=e_1/2$. The finite diagram is one node; its affine extension has two equal-length nodes joined by a double bond, without a short-root arrow.

<a id="2/i/image-finite-and-extended-b-type-dynkin-diagrams-with-short-root-arrows-and-low-rank-exceptions"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-4-dynkin-diagrams.png)

**[Figure 1](#2/i/image-finite-and-extended-b-type-dynkin-diagrams-with-short-root-arrows-and-low-rank-exceptions). Finite and extended B-type Dynkin diagrams with short-root arrows and low-rank exceptions**.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

We construct the [exceptional isomorphism between sp4 and so5](../../../semisimple-lie-algebra.md#exceptional-isomorphism-between-sp4-and-so5). Let $W=\mathbb C^4$ have a [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form) alternating form $\Omega$ and [symplectic basis](../../../linear-algebra.md#symplectic-basis) $a_1,b_1,a_2,b_2$. Define the [symplectic contraction of an exterior square](../../../linear-algebra.md#symplectic-contraction-of-an-exterior-square)

$$
\kappa:\Lambda^2W\to\mathbb C,\qquad\kappa(u\wedge v)=\Omega(u,v),
\qquad E=\ker\kappa.
$$

It is equivariant for the [symplectic Lie algebra](../../../semisimple-lie-algebra.md#symplectic-lie-algebra), and $\dim E=5$. Identify $\Lambda^4W$ with $\mathbb C$ using $a_1\wedge b_1\wedge a_2\wedge b_2$. Wedge product then gives a symmetric [bilinear form](../../../linear-algebra.md#bilinear-form) $B(\xi,\eta)=\xi\wedge\eta$ on $\Lambda^2W$. It is [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form), as the wedge-basis vectors pair with their complementary pairs.

The bivector $\tau=a_1\wedge b_1+a_2\wedge b_2$ is invariant under $\mathfrak{sp}(W)$, satisfies $B(\tau,\tau)=2$, and has $B(\xi,\tau)=\kappa(\xi)$. Consequently $E=\tau^\perp$ and $B|_E$ is [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form). The [exterior-power Lie algebra representation](../../../lie-algebra.md#exterior-power-lie-algebra-representation) preserves wedge product and the volume form, so restriction gives a homomorphism

$$
\Phi:\mathfrak{sp}_4\longrightarrow\mathfrak{so}(E,B).
$$

We check injectivity directly. If $X$ acts trivially on $E$, it also annihilates the invariant line $\mathbb C\tau$, hence acts trivially on all of $\Lambda^2W$. In any basis $w_1,\ldots,w_4$, the equation $X(w_i\wedge w_j)=0$ forces every off-diagonal coefficient $X_{ki}$ to vanish: choose $j$ distinct from $i,k$ and inspect the coefficient of $w_k\wedge w_j$. Thus $X$ is diagonal. Its diagonal entries $x_i$ satisfy $x_i+x_j=0$ for every pair, which forces them all to be zero. Therefore $\Phi$ is injective.

A symplectic matrix has infinitesimal block form $\left(\begin{smallmatrix}A&B\\C&-A^T\end{smallmatrix}\right)$ with $B,C$ symmetric, so $\dim\mathfrak{sp}_4=4+3+3=10$. Also $\dim\mathfrak{so}(E,B)=5\cdot4/2=10$. Injectivity and equal [dimensions](../../../vector-space.md#dimension-vector-space) make $\Phi$ an isomorphism. Every [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form) complex symmetric form in [dimension](../../../vector-space.md#dimension-vector-space) five is equivalent by a change of basis to the given antidiagonal form, so

$$
\boxed{\mathfrak{so}_5\cong\mathfrak{sp}_4.}
$$

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Identify the [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) with its coordinate vector $t=(t_1,\ldots,t_n)$ using the invariant inner product. A [root reflection](../../../semisimple-lie-algebra.md#root-reflection) is

$$
s_\alpha(t)=t-\frac{2(\alpha,t)}{(\alpha,\alpha)}\alpha.
$$

For every root of the [Bn root system](../../../semisimple-lie-algebra.md#bn-root-system), the explicit formulas are

$$
\boxed{\begin{array}{c|c}
\alpha&\text{changed coordinates of }s_\alpha(t)\\\hline
\pm e_i&t_i\mapsto-t_i\\
\pm(e_i-e_j)&(t_i,t_j)\mapsto(t_j,t_i)\\
\pm(e_i+e_j)&(t_i,t_j)\mapsto(-t_j,-t_i)
\end{array}}
$$

All unlisted coordinates stay fixed, and opposite roots define the same reflection. These reflections give all coordinate permutations and independent sign changes. Therefore the [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) is

$$
\boxed{W\cong(\mathbb Z/2\mathbb Z)^n\rtimes S_n,\qquad |W|=2^nn!.}
$$

Its action on $\mathfrak t$ is the group of signed permutation matrices.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

Label the [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) vertices by $1,\ldots,n,0,\bar n,\ldots,\bar1$, with [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) $e_1,\ldots,e_n,0,-e_n,\ldots,-e_1$. The [crystal of the defining odd-orthogonal representation](../../../semisimple-lie-algebra.md#crystal-of-the-defining-odd-orthogonal-representation) is the chain

$$
1\xrightarrow{1}2\xrightarrow{2}\cdots\xrightarrow{n-1}n
\xrightarrow{n}0\xrightarrow{n}\bar n
\xrightarrow{n-1}\overline{n-1}\longrightarrow\cdots\xrightarrow{1}\bar1.
$$

Each arrow of color $i$ subtracts the [simple root](../../../semisimple-lie-algebra.md#simple-root) $\alpha_i$. The two arrows through zero form the length-two short-root string.

Here is a complete grid description of the [tensor product of crystals](../../../semisimple-lie-algebra.md#tensor-product-of-crystals), valid for arbitrary $n$. Place the vertex $a\otimes b$ in row $a$, column $b$, in the above chain order; there are $(2n+1)^2$ vertices. Let $\varepsilon_i(a)$ and $\varphi_i(a)$ count incoming and outgoing steps along the color-$i$ string. For $i<n$, the two strings are $i\to i+1$ and $\overline{i+1}\to\bar i$, each of length one. For $i=n$, the string is $n\to0\to\bar n$, with pairs $(\varepsilon_n,\varphi_n)$ equal to $(0,2),(1,1),(2,0)$. Other vertices have both counts zero.

Using the [crystal tensor-product rule](../../../semisimple-lie-algebra.md#crystal-tensor-product-rule), draw every color-$i$ edge by

$$
\boxed{\widetilde f_i(a\otimes b)=
\begin{cases}\widetilde f_i(a)\otimes b,&\varphi_i(a)>\varepsilon_i(b),\\
a\otimes\widetilde f_i(b),&\varphi_i(a)\le\varepsilon_i(b).
\end{cases}}
$$

The first case is a downward arrow to the next row and the second a rightward arrow to the next column; omit an arrow when its indicated factor has no outgoing edge. Thus the rule specifies every vertex and every arrow of the general tensor-square diagram, including the boundary nodes. The figure displays the resulting entire grid for $n=3$, alongside the vector crystal; the generator can draw any positive rank.

The raising rule chooses the first factor when $\varphi_i(a)\ge\varepsilon_i(b)$ and the second otherwise. For $n\ge2$, its only highest vertices are

$$
\boxed{1\otimes1:\ 2e_1,\qquad
1\otimes2:\ e_1+e_2,\qquad
1\otimes\bar1:\ 0.}
$$

Indeed a highest tensor must have highest first factor, hence $a=1$. For colors $i>1$, the second factor cannot have an incoming edge. For color one, its incoming count must be at most $\varphi_1(1)=1$. Inspecting the strings leaves precisely $b=1,2,\bar1$.

These three connected components encode the [Irreducible Lie algebra representations](../../../lie-algebra.md#irreducible-lie-algebra-representation)

$$
\boxed{V\otimes V\cong S^2_0V\oplus\Lambda^2V\oplus\mathbb C,
\quad\text{highest weights }2e_1,\ e_1+e_2,\ 0.}
$$

Here $S^2_0V$ is the traceless [symmetric square](../../../linear-algebra.md#symmetric-square), $\Lambda^2V$ is the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra), and the invariant symmetric form supplies the trivial summand. Their [dimensions](../../../vector-space.md#dimension-vector-space) are $n(2n+3)$, $n(2n+1)$, and one, summing to $(2n+1)^2$. In fundamental-weight notation the [highest weights](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) are $2\omega_1,\omega_2,0$ for $n\ge3$, but $2\omega_1,2\omega_2,0$ for $n=2$.

For $n=1$ the vector crystal is $1\xrightarrow{1}0\xrightarrow{1}\bar1$. The same tensor rule gives highest vertices $1\otimes1,1\otimes0,1\otimes\bar1$, of [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) $2e_1,e_1,0$, or $4\omega_1,2\omega_1,0$, respectively. Its summand [dimensions](../../../vector-space.md#dimension-vector-space) are $5,3,1$.

<a id="2/iv/image-the-b3-vector-crystal-and-all-49-vertices-and-arrows-of-its-tensor-square"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-4-crystals.png)

**[Figure 2](#2/iv/image-the-b3-vector-crystal-and-all-49-vertices-and-arrows-of-its-tensor-square). The B3 vector crystal and all 49 vertices and arrows of its tensor square**.

## 3

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Let $\mathfrak g$ be a complex [semisimple Lie algebra](../../../semisimple-lie-algebra.md), choose a [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) and a [positive root](../../../semisimple-lie-algebra.md#positive-root) system $R^+$, and let $\lambda$ be a dominant integral [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation). Write $L(\lambda)$ for the corresponding finite-dimensional irreducible representation, $\alpha^\vee=2\alpha/(\alpha,\alpha)$ for a [coroot](../../../semisimple-lie-algebra.md#coroot), and $\rho=\tfrac12\sum_{\alpha\in R^+}\alpha$ for the [Weyl vector](../../../semisimple-lie-algebra.md#half-sum-of-positive-roots). The [Weyl dimension formula](../../../semisimple-lie-algebra.md#weyl-dimension-formula) is

$$
\boxed{\dim L(\lambda)=\prod_{\alpha\in R^+}
\frac{\langle\lambda+\rho,\alpha^\vee\rangle}{\langle\rho,\alpha^\vee\rangle}.}
$$

The bracket denotes the natural pairing of [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) with [coroots](../../../semisimple-lie-algebra.md#coroot). The normalization of an invariant inner product cancels from each ratio, so the formula can equivalently use roots instead of [coroots](../../../semisimple-lie-algebra.md#coroot) in both numerator and denominator.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Number the [simple roots](../../../semisimple-lie-algebra.md#simple-root) of the [G2 root system](../../../semisimple-lie-algebra.md#g2-root-system) so that $\alpha_1$ is short and $\alpha_2$ is long. In the Euclidean plane choose

$$
\alpha_1=(1,0),\qquad\alpha_2=(-3/2,\sqrt3/2).
$$

Their squared lengths are one and three, and their angle is $150$ degrees. The six [positive roots](../../../semisimple-lie-algebra.md#positive-root) are

$$
\alpha_1,\quad\alpha_2,\quad\alpha_1+\alpha_2,\quad2\alpha_1+\alpha_2,
\quad3\alpha_1+\alpha_2,\quad3\alpha_1+2\alpha_2.
$$

Together with their negatives these form the twelve-root diagram: two regular hexagons of radii one and $\sqrt3$, rotated by $30$ degrees relative to one another. Solving the [fundamental weight](../../../semisimple-lie-algebra.md#fundamental-weight) equations gives

$$
\boxed{\omega_1=2\alpha_1+\alpha_2=(1/2,\sqrt3/2),\qquad
\omega_2=3\alpha_1+2\alpha_2=(0,\sqrt3).}
$$

In particular $\omega_1$ is the highest short root and $\omega_2$ the highest long root. The root diagram below marks both [weights](../../../semisimple-lie-algebra.md#weight-representation-theory).

To evaluate the [Weyl dimension formula](../../../semisimple-lie-algebra.md#weyl-dimension-formula), put $a=n_1$, $b=n_2$ and $\lambda=a\omega_1+b\omega_2$. The [Weyl vector](../../../semisimple-lie-algebra.md#half-sum-of-positive-roots) is $\rho=\omega_1+\omega_2$. In the order of [positive roots](../../../semisimple-lie-algebra.md#positive-root) listed above, their [coroots](../../../semisimple-lie-algebra.md#coroot) have simple-coroot coefficient pairs

$$
(1,0),\quad(0,1),\quad(1,3),\quad(2,3),\quad(1,1),\quad(1,2).
$$

For example the short root $\alpha_1+\alpha_2$ has [coroot](../../../semisimple-lie-algebra.md#coroot) $\alpha_1^\vee+3\alpha_2^\vee$, while the long root $3\alpha_1+2\alpha_2$ has [coroot](../../../semisimple-lie-algebra.md#coroot) $\alpha_1^\vee+2\alpha_2^\vee$. Pairing with $\lambda+\rho$ and dividing by the same factors at $a=b=0$ gives the [G2 dimension polynomial](../../../semisimple-lie-algebra.md#g2-dimension-polynomial)

$$
\boxed{\dim L(a\omega_1+b\omega_2)=
\frac{(a+1)(b+1)(a+b+2)(a+2b+3)(a+3b+4)(2a+3b+5)}{120}.}
$$

The denominator is $1\cdot1\cdot2\cdot3\cdot4\cdot5$. As checks, the fundamental representations have [dimensions](../../../vector-space.md#dimension-vector-space) seven and fourteen, and $a=b=0$ gives the trivial representation of [dimension](../../../vector-space.md#dimension-vector-space) one.

<a id="3/ii/image-the-twelve-g2-roots-and-the-short-first-fundamental-weights-omega-one-and-omega-two"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-4-g2-roots.png)

**[Figure 3](#3/ii/image-the-twelve-g2-roots-and-the-short-first-fundamental-weights-omega-one-and-omega-two). The twelve G2 roots and the short-first fundamental weights omega one and omega two**.

## 4

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Give $\mathfrak g$ its [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) and use the [tensor product of Lie algebra representations](../../../lie-algebra.md#tensor-product-of-lie-algebra-representations). Define the [action map of a Lie algebra representation](../../../lie-algebra.md#action-map-of-a-lie-algebra-representation)

$$
\boxed{a:\mathfrak g\otimes V\longrightarrow V,\qquad a(x\otimes v)=xv.}
$$

For $y\in\mathfrak g$, the action on the source is $y(x\otimes v)=[y,x]\otimes v+x\otimes yv$. The defining representation identity then gives

$$
a(y(x\otimes v))=[y,x]v+x(yv)=y(xv)=y\,a(x\otimes v).
$$

Thus $a$ is a [Lie algebra representation homomorphism](../../../lie-algebra.md#lie-algebra-representation-homomorphism).

If $V$ is nontrivial and simple, the action is not identically zero, so the image of $a$ is a nonzero submodule. Simplicity forces $a$ to be surjective. For a finite-dimensional $V$ and a [semisimple Lie algebra](../../../semisimple-lie-algebra.md), the [Weyl complete reducibility theorem](../../../semisimple-lie-algebra.md#weyl-complete-reducibility-theorem) provides an invariant complement $U$ to $\ker a$ in $\mathfrak g\otimes V$. The restriction $a|_U$ is then an isomorphism onto $V$, giving

$$
\boxed{\mathfrak g\otimes V\cong\ker a\oplus V.}
$$

This proves the requested summand assertion in the finite-dimensional setting.

If finite dimensionality is not implicit, the final assertion needs that hypothesis: the [action summand can fail for an infinite-dimensional simple module](../../../lie-algebra.md#action-summand-can-fail-for-an-infinite-dimensional-simple-module). Here is an explicit counterexample. Take $\mathfrak g=\mathfrak{sl}_2$ with $[h,e]=2e$, $[h,f]=-2f$, $[e,f]=h$, and the [Verma module](../../../semisimple-lie-algebra.md#verma-module) of [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) $-2$:

$$
V=\bigoplus_{m\ge0}\mathbb Cv_m,\qquad
fv_m=v_{m+1},\quad hv_m=(-2-2m)v_m,\quad ev_m=-m(m+1)v_{m-1}.
$$

The lowering coefficient never vanishes for $m>0$, so an [invariant subspace](../../../representation-theory.md#invariant-subspace), using the distinct $h$-weights to isolate a basis vector and then raising, contains $v_0$ and hence all of $V$. Thus $V$ is simple.

In $\mathfrak{sl}_2\otimes V$, a vector of [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) $-2$ is $A e\otimes v_1+B h\otimes v_0$. Applying $e$ gives $-2(A+B)e\otimes v_0$, so its highest vectors are precisely the multiples of $w=e\otimes v_1-h\otimes v_0$. But $w=f(e\otimes v_0)$, and $e\otimes v_0$ has [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) zero, absent from $V$. Every homomorphism $r:\mathfrak g\otimes V\to V$ therefore kills this vector and then kills $w$. Any embedded copy of $V$ would send its highest vector to a nonzero multiple of $w$, so it cannot admit a projection back to $V$. This rules out a direct summand, not merely a splitting of the particular action map.

## 5

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

Let $h$ be the standard Cartan element of the [sl2 Lie algebra](../../../semisimple-lie-algebra.md#sl2-lie-algebra), with $[h,e]=2e$ and $[h,f]=-2f$. For a finite-dimensional representation, its [formal character](../../../semisimple-lie-algebra.md#formal-character-of-a-weight-module) records its [weight multiplicities](../../../semisimple-lie-algebra.md#weight-multiplicity):

$$
\boxed{\chi_V(q)=\sum_{j\in\mathbb Z}(\dim V_j)q^j,\qquad
V_j=\{v:hv=jv\}.}
$$

The [classification of finite-dimensional sl2 representations](../../../semisimple-lie-algebra.md#classification-of-finite-dimensional-sl2-representations) and the [Weyl complete reducibility theorem](../../../semisimple-lie-algebra.md#weyl-complete-reducibility-theorem) give $V=\bigoplus_{m\ge0}a_mL_m$, with finitely many nonzero $a_m$. Each $L_m$ has [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) $m,m-2,\ldots,-m$, each of multiplicity one. Therefore

$$
\chi_V(q)=\sum_{m\ge0}a_m(q^m+q^{m-2}+\cdots+q^{-m}),
\qquad c_j=\sum_{\substack{m\ge |j|\\m\equiv j\ (2)}}a_m.
$$

In particular $c_j=c_{-j}$, and for $j\ge0$ one has $c_j-c_{j+2}=a_j\ge0$. This proves [parity unimodality of an sl2 character](../../../semisimple-lie-algebra.md#parity-unimodality-of-an-sl2-character): **within each parity, the coefficients increase towards zero and decrease away from zero**. For a representation whose [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) have a single parity, deleting the intervening zero coefficients gives a symmetric unimodal sequence.

The parity convention is necessary for the printed assertion. If unimodality means the full coefficient sequence at every consecutive integer exponent, it is false: the standard two-dimensional representation has character $q+q^{-1}$, whose coefficients at exponents $-1,0,1$ are $1,0,1$. The statement established above is unimodality on cosets of the [root lattice](../../../semisimple-lie-algebra.md#root-lattice) for $\mathfrak{sl}_2$, and is the version needed in part ii. Infinite-dimensional representations need not even have Laurent-polynomial characters.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Assume $0\le k\le n$ with $n,k$ integers, as required for the quantum binomial expression. Let $L_{n-1}$ be the $n$-dimensional irreducible [sl2 Lie algebra](../../../semisimple-lie-algebra.md#sl2-lie-algebra) representation, with one-dimensional [weight spaces](../../../semisimple-lie-algebra.md#weight-space) of [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) $n-1-2j$, $0\le j<n$. The [exterior-power Lie algebra representation](../../../lie-algebra.md#exterior-power-lie-algebra-representation) on $\Lambda^kL_{n-1}$ has character

$$
C_{n,k}(q)=\sum_{0\le j_1<\cdots<j_k<n}
q^{k(n-1)-2(j_1+\cdots+j_k)}.
$$

This is already a [Laurent polynomial](../../../polynomial.md#laurent-polynomial) with nonnegative integer coefficients.

To identify it with the requested quotient, introduce $t=q^{-2}$ and the [Gaussian binomial coefficient](../../../combinatorics.md#gaussian-binomial-coefficient)

$$
G_{n,k}(t)=\sum_{0\le j_1<\cdots<j_k<n}
 t^{j_1+\cdots+j_k-k(k-1)/2}.
$$

Splitting the subsets according to whether $n-1$ is included proves

$$
G_{n,k}=G_{n-1,k}+t^{n-k}G_{n-1,k-1},\qquad
G_{n,0}=G_{n,n}=1.
$$

The product $\prod_{j=1}^k(1-t^{n-k+j})/(1-t^j)$ satisfies the same recurrence: after factoring common numerator and denominator terms, the needed identity is $(1-t^{n-k})+t^{n-k}(1-t^k)=1-t^n$. Induction on $n$ therefore proves the product identity, including its polynomiality.

Since the [quantum integer](../../../algebra.md#quantum-integer) is $[a]_q=q^{a-1}(1-q^{-2a})/(1-q^{-2})$, taking the quotient of the products gives

$$
\boxed{\left[\begin{matrix}n\\k\end{matrix}\right]_q
=q^{k(n-k)}G_{n,k}(q^{-2})
=C_{n,k}(q)=\chi_{\Lambda^kL_{n-1}}(q).}
$$

Thus this is the [symmetric quantum binomial coefficient](../../../combinatorics.md#symmetric-quantum-binomial-coefficient). All its [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) have parity $k(n-k)$, because the exponent in the exterior-power sum differs from $k(n-k)$ by an even integer. Applying part i to this finite-dimensional representation proves **symmetric unimodality in steps of two**. Equivalently, the ordinary [polynomial](../../../polynomial.md) $G_{n,k}(t)$ has a unimodal coefficient sequence at consecutive powers of $t$.

Again, the full integer-exponent coefficient sequence in $q$, including the absent parity, need not be unimodal: for $n=2,k=1$ the answer is $q+q^{-1}$. This counterexample makes precise the convention under which the claimed quantum unimodality holds. The cases $k=0$ or $k=n$ give the constant one.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
