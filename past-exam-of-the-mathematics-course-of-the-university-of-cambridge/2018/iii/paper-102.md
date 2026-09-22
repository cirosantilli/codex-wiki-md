# Paper 102

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_102.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_102.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)

## 1

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a finite-dimensional complex [Lie algebra](../../../lie-algebra.md) $\mathfrak g$, the following three conditions are equivalent descriptions of a [semisimple Lie algebra](../../../semisimple-lie-algebra.md).

First, its [solvable radical](../../../lie-algebra.md#radical-of-a-lie-algebra) is zero. An [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra) is a linear subspace $I$ satisfying $[\mathfrak g,I]\subseteq I$. A [solvable Lie algebra](../../../lie-algebra.md#solvable-lie-algebra) is one whose [derived series](../../../group-theory.md#derived-series), defined by $I^{(0)}=I$ and $I^{(r+1)}=[I^{(r)},I^{(r)}]$, eventually becomes zero. The [solvable radical](../../../lie-algebra.md#radical-of-a-lie-algebra) is the largest solvable [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra); its vanishing is equivalent to the absence of nonzero solvable ideals.

Second, the [Killing form](../../../lie-algebra.md#killing-form)

$$
\kappa(u,v)=\operatorname{tr}(\operatorname{ad}u\operatorname{ad}v)
$$

is a [nondegenerate bilinear form](../../../linear-algebra.md#nondegenerate-bilinear-form): if $\kappa(u,v)=0$ for every $v$, then $u=0$. Here $\operatorname{ad}u(v)=[u,v]$ is the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra), and $\operatorname{tr}$ is the [trace](../../../linear-algebra.md#matrix-trace). This equivalence is the [Cartan criterion for semisimplicity](../../../lie-algebra.md#cartan-criterion-for-semisimplicity).

Third, $\mathfrak g$ is a [direct sum of Lie algebras](../../../lie-algebra.md#direct-sum-of-lie-algebras) that are nonabelian [simple Lie algebras](../../../semisimple-lie-algebra.md#simple-lie-algebra). A [simple Lie algebra](../../../semisimple-lie-algebra.md#simple-lie-algebra) is nonabelian and has no [ideals of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra) other than zero and itself. Thus the three equivalent criteria are

$$
\boxed{\operatorname{rad}\mathfrak g=0\quad\Longleftrightarrow\quad\kappa\text{ nondegenerate}\quad\Longleftrightarrow\quad\mathfrak g=\bigoplus_j\mathfrak g_j\text{ with each }\mathfrak g_j\text{ simple}.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [derived series](../../../group-theory.md#derived-series) gives a direct test, with no structural theorem needed. By bilinearity and antisymmetry of the [Lie bracket](../../../lie-algebra.md#lie-bracket), every bracket in $\mathfrak h$ is a multiple of $z$, and $z=[x,y]$ actually occurs. Therefore

$$
\mathfrak h^{(1)}=[\mathfrak h,\mathfrak h]=\mathbb Cz,\qquad
\mathfrak h^{(2)}=[\mathbb Cz,\mathbb Cz]=0.
$$

Consequently this [Heisenberg Lie algebra](../../../lie-algebra.md#heisenberg-lie-algebra) is a nonzero [solvable Lie algebra](../../../lie-algebra.md#solvable-lie-algebra). It is an [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra) in itself, since $[\mathfrak h,\mathfrak h]\subseteq\mathfrak h$. Its [solvable radical](../../../lie-algebra.md#radical-of-a-lie-algebra) is therefore all of $\mathfrak h$, contradicting the first criterion in part (a). Hence

$$
\boxed{\mathfrak h\text{ is not semisimple}.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

A two-dimensional [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) already provides a counterexample. In the basis $e_1,e_2$ of $V=\mathbb C^2$, define

$$
\rho(x)=\begin{pmatrix}0&1\\0&0\end{pmatrix},\qquad
\rho(y)=\rho(z)=0.
$$

The commutator $[\rho(x),\rho(y)]$ is zero, agreeing with $\rho(z)$; the other defining [Lie brackets](../../../lie-algebra.md#lie-bracket) also map to zero. Thus $\rho$ is a [Lie algebra homomorphism](../../../lie-algebra.md#lie-algebra-homomorphism), although it is not a [Faithful Lie algebra representation](../../../lie-algebra.md#faithful-lie-algebra-representation).

The line $L=\mathbb Ce_1$ is an [invariant subspace](../../../representation-theory.md#invariant-subspace). Any complementary line has the form $\mathbb C(e_2+a e_1)$ for some $a\in\mathbb C$. But

$$
\rho(x)(e_2+a e_1)=e_1\notin\mathbb C(e_2+a e_1),
$$

so no complementary line is an [invariant subspace](../../../representation-theory.md#invariant-subspace). Equivalently, every invariant line is killed by $\rho(x)$: its restriction to a line is a scalar, and its square is zero, forcing that scalar to be zero. A decomposition into two invariant lines would then force $\rho(x)=0$, a contradiction. This representation is therefore not a [semisimple representation](../../../representation-theory.md#semisimple-representation). Thus

$$
\boxed{\text{Not every finite-dimensional representation of }\mathfrak h\text{ is completely reducible}.}
$$

## 2

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use the [coroot](../../../semisimple-lie-algebra.md#coroot) normalization $\alpha^\vee=2\alpha/(\alpha,\alpha)$, with the pairing understood via the [root system](../../../semisimple-lie-algebra.md#root-system) and its invariant [inner product](../../../linear-algebra.md#inner-product). A [dominant integral weight](../../../semisimple-lie-algebra.md#dominant-integral-weight), called a [dominant weight](../../../semisimple-lie-algebra.md#dominant-weight) here, is a functional $\lambda\in\mathfrak t^*$ such that

$$
\boxed{\langle\lambda,\alpha_i^\vee\rangle\in\mathbb Z_{\geq0}\quad\text{for every simple root }\alpha_i.}
$$

Equivalently, $\lambda=\sum_i n_i\omega_i$ with $n_i\in\mathbb Z_{\geq0}$, where the [fundamental weights](../../../semisimple-lie-algebra.md#fundamental-weight) satisfy $\langle\omega_i,\alpha_j^\vee\rangle=\delta_{ij}$. If dominance and integrality are defined separately, dominance means the inequalities and membership in the [weight lattice](../../../semisimple-lie-algebra.md#weight-lattice) means integrality.

A [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector) is a nonzero [weight vector](../../../semisimple-lie-algebra.md#weight-vector) $v\in V_\lambda$, so $h\cdot v=\lambda(h)v$ for all $h\in\mathfrak t$, annihilated by every positive [root space](../../../semisimple-lie-algebra.md#root-space):

$$
\boxed{v\ne0,\quad h\cdot v=\lambda(h)v,\quad\mathfrak g_\beta\cdot v=0\quad(\beta\in\Phi^+).}
$$

The last condition is equivalently annihilation by the [raising operators](../../../semisimple-lie-algebra.md#raising-operator) for the [simple roots](../../../semisimple-lie-algebra.md#simple-root).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Fix a [simple root](../../../semisimple-lie-algebra.md#simple-root) $\alpha_i$ and choose generators $e_i,f_i,h_i$ of the [sl2 subalgebra associated with a root](../../../semisimple-lie-algebra.md#sl2-subalgebra-associated-with-a-root), with $h_i=\alpha_i^\vee$ and

$$
[h_i,e_i]=2e_i,\qquad[h_i,f_i]=-2f_i,\qquad[e_i,f_i]=h_i.
$$

The [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector) satisfies $e_i v=0$ and $h_i v=m_i v$, where $m_i=\langle\lambda,\alpha_i^\vee\rangle$. The [classification of finite-dimensional sl2 representations](../../../semisimple-lie-algebra.md#classification-of-finite-dimensional-sl2-representations) already implies that $m_i$ is a nonnegative integer. One can also see the necessary integrality directly from the [lowering operator](../../../semisimple-lie-algebra.md#lowering-operator).

Indeed, $f_i^k v$, if nonzero, has $h_i$ eigenvalue $m_i-2k$. These distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue) cannot occur indefinitely in a finite-dimensional space, so there is a largest $r\geq0$ with $f_i^r v\ne0$. The [sl2 Lie algebra](../../../semisimple-lie-algebra.md#sl2-lie-algebra) relations imply, by induction on $k$,

$$
e_i f_i^k v=k(m_i-k+1)f_i^{k-1}v.
$$

For $k=r+1$ the left side is zero, hence $(r+1)(m_i-r)f_i^r v=0$. Thus $m_i=r\in\mathbb Z_{\geq0}$. Since this holds for every [simple root](../../../semisimple-lie-algebra.md#simple-root),

$$
\boxed{\lambda\text{ is a dominant integral weight}.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Choose the given [short root](../../../semisimple-lie-algebra.md#short-root) $\alpha$ as a [simple root](../../../semisimple-lie-algebra.md#simple-root), and let $\beta$ be the long [simple root](../../../semisimple-lie-algebra.md#simple-root). This entails no loss of generality: the [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) is transitive on the [short roots](../../../semisimple-lie-algebra.md#short-root) of the [G2 root system](../../../semisimple-lie-algebra.md#g2-root-system). The relevant [Cartan integers](../../../semisimple-lie-algebra.md#cartan-integer) are $\langle\beta,\alpha^\vee\rangle=-3$ and $\langle\alpha,\beta^\vee\rangle=-1$. The [positive roots](../../../semisimple-lie-algebra.md#positive-root) are

$$
\alpha,\ \beta,\ \alpha+\beta,\ 2\alpha+\beta,\ 3\alpha+\beta,\ 3\alpha+2\beta.
$$

Under $\mathfrak m_\alpha\cong\mathfrak{sl}_2$, the [root space](../../../semisimple-lie-algebra.md#root-space) for $m\alpha+n\beta$ has $h_\alpha$ eigenvalue $2m-3n$. The subalgebra $\mathfrak m_\alpha$ itself is the three-dimensional irreducible $V(2)$ in the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra).

The four [root spaces](../../../semisimple-lie-algebra.md#root-space) along the [root string](../../../semisimple-lie-algebra.md#root-string) $\beta,\alpha+\beta,2\alpha+\beta,3\alpha+\beta$ have eigenvalues $-3,-1,1,3$. Consecutive spaces are connected by nonzero [raising operators](../../../semisimple-lie-algebra.md#raising-operator) and [lowering operators](../../../semisimple-lie-algebra.md#lowering-operator), so their sum is $V(3)$. The negative [root string](../../../semisimple-lie-algebra.md#root-string) supplies another $V(3)$. The [root spaces](../../../semisimple-lie-algebra.md#root-space) for $\pm(3\alpha+2\beta)$ have eigenvalue zero, and neither adding nor subtracting $\alpha$ gives a root; they are two copies of $V(0)$. Finally, the one-dimensional space $\ker\alpha\subset\mathfrak t$ commutes with $\mathfrak m_\alpha$, giving one more $V(0)$. We have accounted for all $14$ dimensions, and therefore the [G2 adjoint branching to a short-root sl2 subalgebra](../../../semisimple-lie-algebra.md#g2-adjoint-branching-to-a-short-root-sl2-subalgebra) is

$$
\boxed{\mathfrak g\cong V(3)^{\oplus2}\oplus V(2)\oplus V(0)^{\oplus3}.}
$$

For a nonzero [root vector](../../../semisimple-lie-algebra.md#root-vector) $x\in\mathfrak g_\alpha$, its [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) action is a nonzero scalar multiple of the [raising operator](../../../semisimple-lie-algebra.md#raising-operator) on each summand. On each irreducible $V(n)$ this operator has a one-dimensional [kernel](../../../linear-algebra.md#kernel-of-a-linear-map), including $V(0)$. Since the [Lie algebra centralizer](../../../lie-algebra.md#centralizer-of-an-element-of-a-lie-algebra) is that [kernel](../../../linear-algebra.md#kernel-of-a-linear-map),

$$
\boxed{\dim Z_{\mathfrak g}(x)=2+1+3=6.}
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Suppose first that $x\ne0$, and let $E$ be the real span of the [root system](../../../semisimple-lie-algebra.md#root-system), of dimension equal to the [rank of a semisimple Lie algebra](../../../semisimple-lie-algebra.md#rank-of-a-semisimple-lie-algebra) $\ell$. The images of the roots span $E/\mathbb R\alpha$, so select roots $\beta_1,\ldots,\beta_{\ell-1}$ whose images form a basis of this quotient.

For each $i$, take the highest endpoint $\gamma_i^+$ of the $\alpha$ [root string](../../../semisimple-lie-algebra.md#root-string) through $\beta_i$, and the highest endpoint $\gamma_i^-$ of the [root string](../../../semisimple-lie-algebra.md#root-string) through $-\beta_i$. By construction, $\gamma_i^\pm+\alpha$ is not a root. Moreover $\gamma_i^\pm\ne-\alpha$, since their images in $E/\mathbb R\alpha$ are nonzero. The [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition) and its bracket rule therefore give

$$
[\mathfrak g_{\gamma_i^\pm},x]=0.
$$

These $2(\ell-1)$ roots are distinct: their quotient images are the two signs of a basis, which are distinct. Their one-dimensional [root spaces](../../../semisimple-lie-algebra.md#root-space) consequently contribute $2(\ell-1)$ independent vectors to the [Lie algebra centralizer](../../../lie-algebra.md#centralizer-of-an-element-of-a-lie-algebra).

In addition, the $\ell-1$ dimensional subspace $\ker\alpha\subset\mathfrak t$ commutes with $x$, because $[h,x]=\alpha(h)x$. The line $\mathbb Cx\subset\mathfrak g_\alpha$ also commutes with $x$. These contributions are independent by the [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition); in particular none of the selected endpoint roots is $\alpha$. Thus the [centralizer lower bound for a root vector](../../../lie-algebra.md#centralizer-lower-bound-for-a-root-vector) is

$$
\boxed{\dim Z_{\mathfrak g}(x)\geq2(\ell-1)+(\ell-1)+1=3\ell-2.}
$$

If $x=0$, then $Z_{\mathfrak g}(x)=\mathfrak g$. The [root system](../../../semisimple-lie-algebra.md#root-system) contains the $2\ell$ distinct roots $\pm\alpha_i$, so $\dim\mathfrak g=\ell+|\Phi|\geq3\ell$, which also proves the desired inequality. The argument includes rank one, where the list of $\beta_i$ is empty.

## 3

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Write an element of the diagonal [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) as

$$
H(t)=\operatorname{diag}(t_1,t_2,t_3,-t_1,-t_2,-t_3),\qquad
\varepsilon_i(H(t))=t_i.
$$

The [root system](../../../semisimple-lie-algebra.md#root-system) of this [Special orthogonal Lie algebra](../../../semisimple-lie-algebra.md#special-orthogonal-lie-algebra) is

$$
\boxed{\Phi=\{\pm\varepsilon_i\pm\varepsilon_j:1\leq i<j\leq3\}.}
$$

Thus the maps requested are $H(t)\mapsto\pm t_i\pm t_j$, with the two signs independent. This is the [D3 root system](../../../semisimple-lie-algebra.md#d3-root-system), with twelve roots.

For a direct check, the defining matrix identity gives the block form $X=\begin{pmatrix}A&B\\C&-A^T\end{pmatrix}$ with $B^T=-B$ and $C^T=-C$. If $E_{ij}$ denotes a [matrix unit](../../../vector-space.md#matrix-unit), the [root space](../../../semisimple-lie-algebra.md#root-space) for $\varepsilon_i-\varepsilon_j$ is spanned by $E_{ij}-E_{j+3,i+3}$; those for $\varepsilon_i+\varepsilon_j$ and $-\varepsilon_i-\varepsilon_j$ are spanned respectively by $E_{i,j+3}-E_{j,i+3}$ and $E_{i+3,j}-E_{j+3,i}$. Commuting these with $H(t)$ gives exactly the displayed maps.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Choose the [root basis](../../../semisimple-lie-algebra.md#fundamental-system-of-a-root-system)

$$
\boxed{\alpha_1=\varepsilon_1-\varepsilon_2,\qquad
\alpha_2=\varepsilon_2-\varepsilon_3,\qquad
\alpha_3=\varepsilon_2+\varepsilon_3.}
$$

In the usual invariant [inner product](../../../linear-algebra.md#inner-product), each [simple root](../../../semisimple-lie-algebra.md#simple-root) has squared length $2$, while $(\alpha_1,\alpha_2)=(\alpha_1,\alpha_3)=-1$ and $(\alpha_2,\alpha_3)=0$. The labeled [Dynkin diagram](../../../semisimple-lie-algebra.md#dynkin-diagram) is therefore the following chain, with a single bond between adjacent nodes:

$$
\underset{\alpha_2}{\circ}\;\text{---}\;\underset{\alpha_1}{\circ}\;\text{---}\;\underset{\alpha_3}{\circ}.
$$

It is type $D_3$, equivalently the [A3 root system](../../../semisimple-lie-algebra.md#a3-root-system). To check the [root basis](../../../semisimple-lie-algebra.md#fundamental-system-of-a-root-system) explicitly, the corresponding [positive roots](../../../semisimple-lie-algebra.md#positive-root) are $\alpha_1,\alpha_2,\alpha_3,\alpha_1+\alpha_2,\alpha_1+\alpha_3,\alpha_1+\alpha_2+\alpha_3$; these and their negatives are all twelve roots.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $s_i=w_{\alpha_i}$. The [root reflection](../../../semisimple-lie-algebra.md#root-reflection) formula is $s_i(\gamma)=\gamma-\langle\gamma,\alpha_i^\vee\rangle\alpha_i$. Applying the [Cartan integers](../../../semisimple-lie-algebra.md#cartan-integer) from part (b), the images of the chosen [simple roots](../../../semisimple-lie-algebra.md#simple-root) are

$$
\boxed{\begin{array}{c|ccc}
 &\alpha_1&\alpha_2&\alpha_3\\\hline
s_1&-\alpha_1&\alpha_1+\alpha_2&\alpha_1+\alpha_3\\
s_2&\alpha_1+\alpha_2&-\alpha_2&\alpha_3\\
s_3&\alpha_1+\alpha_3&\alpha_2&-\alpha_3
\end{array}.}
$$

In particular, the two end-node [Weyl reflections](../../../semisimple-lie-algebra.md#weyl-reflection) fix the opposite end node.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

An [automorphism of a root system](../../../semisimple-lie-algebra.md#automorphism-of-a-root-system) outside the [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) is the sign change

$$
\boxed{\tau(\varepsilon_1)=\varepsilon_1,\qquad
\tau(\varepsilon_2)=\varepsilon_2,\qquad
\tau(\varepsilon_3)=-\varepsilon_3.}
$$

It preserves the set $\{\pm\varepsilon_i\pm\varepsilon_j\}$, fixes $\alpha_1$, and interchanges $\alpha_2$ and $\alpha_3$. It therefore realizes the nontrivial symmetry of the [Dynkin diagram](../../../semisimple-lie-algebra.md#dynkin-diagram) while preserving the chosen [root basis](../../../semisimple-lie-algebra.md#fundamental-system-of-a-root-system).

To verify that $\tau\notin W$, note that $s_1$ swaps $\varepsilon_1,\varepsilon_2$, $s_2$ swaps $\varepsilon_2,\varepsilon_3$, and $s_3$ swaps $\varepsilon_2,\varepsilon_3$ while changing both their signs. Every product of these generators is a signed permutation with an even number of sign changes, whereas $\tau$ has one sign change. Thus it cannot be a [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) element. The parity here concerns sign changes, rather than the determinant of the permutation.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The [Dynkin diagram](../../../semisimple-lie-algebra.md#dynkin-diagram) in part (b) is a three-node chain, hence $D_3=A_3$. By the classification of complex [semisimple Lie algebras](../../../semisimple-lie-algebra.md) by their [root systems](../../../semisimple-lie-algebra.md#root-system), this gives the [Isomorphism between so6 and sl4](../../../semisimple-lie-algebra.md#isomorphism-between-so6-and-sl4):

$$
\boxed{\mathfrak{so}_6\cong\mathfrak{sl}_4.}
$$

There is also a concrete realization. On $U=\mathbb C^4$, choose a nonzero alternating four-form $\mathrm{vol}$. The six-dimensional [exterior square](../../../linear-algebra.md#exterior-square) $\Lambda^2U$ carries the [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form) [symmetric bilinear form](../../../linear-algebra.md#symmetric-bilinear-form) $B$ specified by

$$
B(u\wedge v,w\wedge z)=\mathrm{vol}(u,v,w,z).
$$

It is symmetric because exchanging two pairs entails four transpositions, and it is nondegenerate because each basis bivector pairs nontrivially with its complementary pair. The [special linear Lie algebra](../../../semisimple-lie-algebra.md#special-linear-lie-algebra) acts by $A(u\wedge v)=Au\wedge v+u\wedge Av$. Its action on $\Lambda^4U$ is multiplication by $\operatorname{tr}A=0$, so it preserves $B$. We obtain a nonzero [Lie algebra homomorphism](../../../lie-algebra.md#lie-algebra-homomorphism) $\mathfrak{sl}_4\to\mathfrak{so}(\Lambda^2U,B)$. Its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is an [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra), hence zero because $\mathfrak{sl}_4$ is a [simple Lie algebra](../../../semisimple-lie-algebra.md#simple-lie-algebra). Both sides have dimension $15$, so this homomorphism is a [Lie algebra isomorphism](../../../lie-algebra.md#lie-algebra-isomorphism).

## 4

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For a [dominant integral weight](../../../semisimple-lie-algebra.md#dominant-integral-weight) $\lambda$, let $V(\lambda)$ be the finite-dimensional irreducible [highest-weight representation](../../../semisimple-lie-algebra.md#highest-weight-representation) with [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) $\lambda$. Set $\rho=\frac12\sum_{\alpha\in\Phi^+}\alpha$, the [half-sum of positive roots](../../../semisimple-lie-algebra.md#half-sum-of-positive-roots). With $\alpha^\vee$ the [coroot](../../../semisimple-lie-algebra.md#coroot) of $\alpha$, the [Weyl dimension formula](../../../semisimple-lie-algebra.md#weyl-dimension-formula) is

$$
\boxed{\dim V(\lambda)=\prod_{\alpha\in\Phi^+}
\frac{\langle\lambda+\rho,\alpha^\vee\rangle}
{\langle\rho,\alpha^\vee\rangle}.}
$$

Here $\Phi^+$ is the [positive system of a root system](../../../semisimple-lie-algebra.md#positive-system-of-a-root-system) specified by the chosen [root basis](../../../semisimple-lie-algebra.md#fundamental-system-of-a-root-system). The [fundamental weights](../../../semisimple-lie-algebra.md#fundamental-weight) are the basis dual to the simple [coroots](../../../semisimple-lie-algebra.md#coroot): $\langle\omega_i,\alpha_j^\vee\rangle=\delta_{ij}$. Thus $\lambda=\sum_i a_i\omega_i$ with nonnegative integers $a_i$. The denominators are positive; equivalently one can use $(\lambda+\rho,\alpha)/(\rho,\alpha)$ in each factor, since the coroot normalization cancels.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Use the [C2 root system](../../../semisimple-lie-algebra.md#c2-root-system) realization in an orthonormal basis $\varepsilon_1,\varepsilon_2$ with [simple roots](../../../semisimple-lie-algebra.md#simple-root) $\alpha_1=\varepsilon_1-\varepsilon_2$ and $\alpha_2=2\varepsilon_2$. This numbers the [short root](../../../semisimple-lie-algebra.md#short-root) first, as required. The [fundamental weights](../../../semisimple-lie-algebra.md#fundamental-weight) and [half-sum of positive roots](../../../semisimple-lie-algebra.md#half-sum-of-positive-roots) are

$$
\omega_1=\varepsilon_1,\qquad\omega_2=\varepsilon_1+\varepsilon_2,\qquad
\rho=2\varepsilon_1+\varepsilon_2,
$$

so $\lambda+\rho=(a+b+2)\varepsilon_1+(b+1)\varepsilon_2$. For the four [positive roots](../../../semisimple-lie-algebra.md#positive-root), the factors of the [Weyl dimension formula](../../../semisimple-lie-algebra.md#weyl-dimension-formula) are

$$
\begin{array}{c|c|c}
\alpha&\alpha^\vee&
\langle\lambda+\rho,\alpha^\vee\rangle/\langle\rho,\alpha^\vee\rangle\\\hline
\varepsilon_1-\varepsilon_2&\varepsilon_1-\varepsilon_2&a+1\\
2\varepsilon_2&\varepsilon_2&b+1\\
\varepsilon_1+\varepsilon_2&\varepsilon_1+\varepsilon_2&(a+2b+3)/3\\
2\varepsilon_1&\varepsilon_1&(a+b+2)/2
\end{array}.
$$

Multiplying yields the [Weyl dimension formula for C2](../../../semisimple-lie-algebra.md#weyl-dimension-formula-for-c2):

$$
\boxed{\dim V(a\omega_1+b\omega_2)=\frac{(a+1)(b+1)(a+b+2)(a+2b+3)}6.}
$$

As checks, $V(\omega_1)$ has dimension $4$, $V(\omega_2)$ dimension $5$, and $V(2\omega_1)$ dimension $10$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

In the defining representation of the [symplectic Lie algebra](../../../semisimple-lie-algebra.md#symplectic-lie-algebra) $\mathfrak{sp}_4$, the weights are $\varepsilon_1,\varepsilon_2,-\varepsilon_1,-\varepsilon_2$. Their [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation), for the [root basis](../../../semisimple-lie-algebra.md#fundamental-system-of-a-root-system) of part (b), is therefore

$$
\boxed{\operatorname{highest\ weight}(V)=\varepsilon_1=\omega_1.}
$$

The flip on the [tensor square](../../../linear-algebra.md#tensor-square) commutes with the action of $\mathfrak{sp}_4$, giving $V\otimes V=\operatorname{Sym}^2V\oplus\Lambda^2V$ with dimensions $10$ and $6$.

If $v_1$ is a [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector) of weight $\varepsilon_1$, then $v_1\otimes v_1$ is a [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector) of weight $2\omega_1$ in the [symmetric square](../../../linear-algebra.md#symmetric-square). By [Weyl complete reducibility theorem](../../../semisimple-lie-algebra.md#weyl-complete-reducibility-theorem), this ensures an irreducible summand $V(2\omega_1)$ occurs. Its dimension is $10$ by part (b), exhausting the [symmetric square](../../../linear-algebra.md#symmetric-square).

Let $\omega$ denote the preserved [symplectic form](../../../symplectic-geometry.md#symplectic-form). The [symplectic contraction of an exterior square](../../../linear-algebra.md#symplectic-contraction-of-an-exterior-square) is the nonzero equivariant map

$$
c:\Lambda^2V\longrightarrow\mathbb C,\qquad c(v\wedge w)=\omega(v,w),
$$

where the target is a [trivial Lie algebra representation](../../../lie-algebra.md#trivial-lie-algebra-representation). Thus its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) has dimension $5$. Choose a weight vector $v_2$ of weight $\varepsilon_2$ in a [symplectic basis](../../../linear-algebra.md#symplectic-basis), with $\omega(v_1,v_2)=0$. The vector $v_1\wedge v_2$ belongs to this [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) and has weight $\varepsilon_1+\varepsilon_2=\omega_2$. It is a [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector): none of $\omega_2+\alpha$, for $\alpha\in\Phi^+$, is a weight of $\Lambda^2V$, whose weights are $\pm\varepsilon_1\pm\varepsilon_2$ and zero. Hence the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) contains $V(\omega_2)$; its dimension $5$ exhausts the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map). [Weyl complete reducibility theorem](../../../semisimple-lie-algebra.md#weyl-complete-reducibility-theorem) supplies a complementary invariant line $V(0)$.

The resulting [tensor-square decomposition of the defining sp4 representation](../../../semisimple-lie-algebra.md#tensor-square-decomposition-of-the-defining-sp4-representation) is

$$
\boxed{V\otimes V\cong V(2\omega_1)\oplus V(\omega_2)\oplus V(0),\qquad16=10+5+1.}
$$

## 5

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The [formal character of a weight module](../../../semisimple-lie-algebra.md#formal-character-of-a-weight-module) is $\operatorname{ch}V=\sum_\mu(\dim V_\mu)e^\mu$, where $e^\mu$ are formal basis symbols in the [group algebra](../../../associative-algebra.md#group-algebra) of the [weight lattice](../../../semisimple-lie-algebra.md#weight-lattice), satisfying $e^\mu e^\nu=e^{\mu+\nu}$. For a finite-dimensional irreducible [highest-weight representation](../../../semisimple-lie-algebra.md#highest-weight-representation), the [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) has [weight multiplicity](../../../semisimple-lie-algebra.md#weight-multiplicity) one. Another standard result is that [weight multiplicities](../../../semisimple-lie-algebra.md#weight-multiplicity) are invariant under the [Weyl group](../../../semisimple-lie-algebra.md#weyl-group): $\dim V_{w\mu}=\dim V_\mu$.

A [minuscule representation](../../../semisimple-lie-algebra.md#minuscule-representation) has all its weights in a single [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) orbit. Since the [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) $\lambda$ is present, that orbit is $W\lambda$, and the invariance just stated shows every point of it is present with multiplicity one. Consequently the [formal character of a minuscule representation](../../../semisimple-lie-algebra.md#formal-character-of-a-minuscule-representation) is

$$
\boxed{\operatorname{ch}V(\lambda)=\sum_{\mu\in W\lambda}e^\mu,\qquad\dim V(\lambda)=|W\lambda|.}
$$

The sum is over distinct weights, rather than over all elements of $W$: summing $e^{w\lambda}$ over $w\in W$ would count each weight $|\operatorname{Stab}_W(\lambda)|$ times.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Use the [coroot](../../../semisimple-lie-algebra.md#coroot) $\alpha^\vee$ in the pairing. The original PDF retains this mark, which is lost in the local TeX transcription. Fix any [positive root](../../../semisimple-lie-algebra.md#positive-root) $\alpha$, and put $n=\langle\lambda,\alpha^\vee\rangle$. For a [dominant integral weight](../../../semisimple-lie-algebra.md#dominant-integral-weight), $n$ is a nonnegative integer; positive [coroots](../../../semisimple-lie-algebra.md#coroot) are nonnegative integral combinations of simple [coroots](../../../semisimple-lie-algebra.md#coroot).

Let $v_\lambda$ be a [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector), and restrict to the [sl2 subalgebra associated with a root](../../../semisimple-lie-algebra.md#sl2-subalgebra-associated-with-a-root) $\alpha$. It is killed by its [raising operator](../../../semisimple-lie-algebra.md#raising-operator) $e_\alpha$ and has $h_\alpha$ eigenvalue $n$. If $n\geq1$, its [lowering operator](../../../semisimple-lie-algebra.md#lowering-operator) produces a nonzero vector: otherwise $[e_\alpha,f_\alpha]v_\lambda=n v_\lambda$ would vanish. Therefore $\lambda-\alpha$ is a weight.

Choose a [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) invariant positive-definite [inner product](../../../linear-algebra.md#inner-product) on the real weight space. All weights of a [minuscule representation](../../../semisimple-lie-algebra.md#minuscule-representation) have the same norm, since they belong to $W\lambda$. But

$$
\|\lambda-\alpha\|^2-\|\lambda\|^2
=-2(\lambda,\alpha)+(\alpha,\alpha)
=(1-n)(\alpha,\alpha).
$$

If $n\geq2$, this is negative, a contradiction. Thus for every [positive root](../../../semisimple-lie-algebra.md#positive-root),

$$
\boxed{\langle\lambda,\alpha^\vee\rangle\in\{0,1\},\quad\text{in particular }\langle\lambda,\alpha^\vee\rangle\leq1.}
$$

When $n=1$, the lower weight is precisely the [Weyl reflection](../../../semisimple-lie-algebra.md#weyl-reflection) $s_\alpha\lambda=\lambda-\alpha$, consistent with the orbit condition.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

We first prove the useful lemma that [dominant root-lattice highest weights have zero weight](../../../semisimple-lie-algebra.md#dominant-root-lattice-highest-weights-have-zero-weight). Write $Q=\mathbb Z\Phi$ for the [root lattice](../../../semisimple-lie-algebra.md#root-lattice), and let a [dominant integral weight](../../../semisimple-lie-algebra.md#dominant-integral-weight) $\lambda\in Q$ be the [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) of a finite-dimensional irreducible representation.

First, $\lambda$ is a nonnegative integral combination of [simple roots](../../../semisimple-lie-algebra.md#simple-root). Indeed, write $\lambda=\lambda_+-\lambda_-$, separating its positive and negative coefficients in the [root basis](../../../semisimple-lie-algebra.md#fundamental-system-of-a-root-system). The two parts have disjoint supports, and distinct [simple roots](../../../semisimple-lie-algebra.md#simple-root) have nonpositive [inner product](../../../linear-algebra.md#inner-product), so $(\lambda_+,\lambda_-)\leq0$. If $\lambda_-\ne0$, then

$$
(\lambda,\lambda_-)=(\lambda_+,\lambda_-)-(\lambda_-,\lambda_-)<0.
$$

On the other hand, dominance gives $(\lambda,\alpha_i)\geq0$ for each [simple root](../../../semisimple-lie-algebra.md#simple-root), hence $(\lambda,\lambda_-)\geq0$. This contradiction proves $\lambda_-=0$.

Now suppose a nonzero weight $\mu=\sum_i m_i\alpha_i$ has all $m_i\in\mathbb Z_{\geq0}$. The identity

$$
0<(\mu,\mu)=\sum_i m_i(\mu,\alpha_i)
$$

shows that some $i$ satisfies $m_i>0$ and $\langle\mu,\alpha_i^\vee\rangle>0$. We use the standard [sl2 Lie algebra](../../../semisimple-lie-algebra.md#sl2-lie-algebra) fact that its [lowering operator](../../../semisimple-lie-algebra.md#lowering-operator) is injective on any positive $h$ eigenspace in a finite-dimensional representation. This follows from the [classification of finite-dimensional sl2 representations](../../../semisimple-lie-algebra.md#classification-of-finite-dimensional-sl2-representations): in each irreducible $V(n)$, the only weight killed by the [lowering operator](../../../semisimple-lie-algebra.md#lowering-operator) is the lowest weight $-n\leq0$.

Consequently a nonzero vector of weight $\mu$ lowers to a nonzero vector of weight $\mu-\alpha_i$. Its simple-root coefficients remain nonnegative and their sum decreases by one. Starting at $\lambda$, repeated lowering must therefore reach the zero weight. Notice that intermediate weights need not remain dominant; positivity of the chosen coroot pairing is enough at each step.

For a [minuscule representation](../../../semisimple-lie-algebra.md#minuscule-representation), every weight belongs to $W\lambda$, so the zero weight just obtained lies in this orbit. Every [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) element is invertible, and $w\lambda=0$ forces $\lambda=0$. This proves that [minuscule weights in the root lattice are zero](../../../semisimple-lie-algebra.md#minuscule-weights-in-the-root-lattice-are-zero). Under the assumption $X=Q$, every possible [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) lies in $Q$, hence

$$
\boxed{X=\mathbb Z\Phi\ \Longrightarrow\ \text{the only minuscule irreducible representation is }V(0),\text{ the trivial one}.}
$$

Here $V(0)$ is the one-dimensional [trivial Lie algebra representation](../../../lie-algebra.md#trivial-lie-algebra-representation), by the classification of finite-dimensional irreducible [highest-weight representations](../../../semisimple-lie-algebra.md#highest-weight-representation).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
