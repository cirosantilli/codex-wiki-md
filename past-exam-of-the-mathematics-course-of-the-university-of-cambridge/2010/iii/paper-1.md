# Paper 1

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper1.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper1.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
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

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The defining rule for a [derivation of a Lie algebra](../../../lie-algebra.md#derivation-of-a-lie-algebra) is linear in the operator, so $\operatorname{Der}(\mathfrak g)$ is a [vector subspace](../../../vector-space.md#vector-subspace) of the [general linear Lie algebra](../../../lie-algebra.md#general-linear-lie-algebra) $\mathfrak{gl}(\mathfrak g)$. Its [Lie bracket](../../../lie-algebra.md#lie-bracket) is the operator [commutator](../../../lie-algebra.md#commutator). If $D,E$ are [derivations of a Lie algebra](../../../lie-algebra.md#derivation-of-a-lie-algebra), expand both compositions:

$$
\begin{aligned}
DE[x,y]&=[DEx,y]+[Ex,Dy]+[Dx,Ey]+[x,DEy],\\
ED[x,y]&=[EDx,y]+[Dx,Ey]+[Ex,Dy]+[x,EDy].
\end{aligned}
$$

Subtracting cancels the mixed terms and gives

$$
[D,E][x,y]=[[D,E]x,y]+[x,[D,E]y].
$$

Thus $[D,E]$ is again a [derivation of a Lie algebra](../../../lie-algebra.md#derivation-of-a-lie-algebra), proving that the [derivation Lie algebra](../../../lie-algebra.md#derivation-lie-algebra) is a [Lie subalgebra](../../../lie-algebra.md#lie-subalgebra) of $\mathfrak{gl}(\mathfrak g)$. This calculation works in every [characteristic of a field](../../../algebra.md#characteristic-of-a-field).

The [Jacobi identity](../../../lie-algebra.md#jacobi-identity) states $[x,[y,z]]=[[x,y],z]+[y,[x,z]]$. It first shows that $\operatorname{ad}_x$ is a [derivation of a Lie algebra](../../../lie-algebra.md#derivation-of-a-lie-algebra), and then gives

$$
[\operatorname{ad}_x,\operatorname{ad}_y](z)=[x,[y,z]]-[y,[x,z]]=[[x,y],z].
$$

The map $x\mapsto\operatorname{ad}_x$ is linear, so this identity proves it is a [Lie algebra homomorphism](../../../lie-algebra.md#lie-algebra-homomorphism).

Finally, for any [derivation of a Lie algebra](../../../lie-algebra.md#derivation-of-a-lie-algebra) $D$,

$$
[D,\operatorname{ad}_x](y)=D[x,y]-[x,Dy]=[Dx,y].
$$

Consequently

$$
\boxed{[D,\operatorname{ad}_x]=\operatorname{ad}_{Dx},\qquad[\operatorname{Der}(\mathfrak g),\operatorname{ad}\mathfrak g]\subseteq\operatorname{ad}\mathfrak g.}
$$

This proves that the [inner derivations of a Lie algebra](../../../lie-algebra.md#inner-derivation-of-a-lie-algebra) form an [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra) in $\operatorname{Der}(\mathfrak g)$.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Equip $E$ with the [inner product](../../../linear-algebra.md#inner-product) defining the [root system](../../../semisimple-lie-algebra.md#root-system), so the [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) acts by [orthogonal transformations](../../../linear-algebra.md#orthogonal-transformation). As usual, the [root system](../../../semisimple-lie-algebra.md#root-system) spans its ambient space $E$. Let $U\subseteq E$ be an [invariant subspace](../../../representation-theory.md#invariant-subspace) for the [reflection representation of a Weyl group](../../../semisimple-lie-algebra.md#reflection-representation-of-a-weyl-group). Its [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) is also invariant.

For a [root](../../../semisimple-lie-algebra.md#root-of-a-root-system) $\alpha$, the [Weyl reflection](../../../semisimple-lie-algebra.md#weyl-reflection) satisfies

$$
s_\alpha(u)=u-\frac{2(u,\alpha)}{(\alpha,\alpha)}\alpha.
$$

If $(u,\alpha)=0$ for every $u\in U$, then $\alpha\in U^\perp$. Otherwise choose $u\in U$ with $(u,\alpha)\ne0$. Both $u$ and $s_\alpha(u)$ belong to $U$, and their difference is a nonzero multiple of $\alpha$, so $\alpha\in U$. Hence

$$
R=(R\cap U)\sqcup(R\cap U^\perp).
$$

The two sets are mutually [orthogonal](../../../linear-algebra.md#orthogonal-vectors) and individually closed under their root reflections. If both were nonempty, this would decompose $R$ into two [orthogonal](../../../linear-algebra.md#orthogonal-vectors) [root systems](../../../semisimple-lie-algebra.md#root-system), contradicting that it is an [irreducible root system](../../../semisimple-lie-algebra.md#irreducible-root-system). All roots therefore lie in one of the two subspaces. Because they span $E$, either $U=E$ or $U^\perp=E$, the latter giving $U=0$. Thus the reflection representation is an [irreducible representation](../../../representation-theory.md#irreducible-representation).

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use the traceless diagonal [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) of the [special linear Lie algebra](../../../semisimple-lie-algebra.md#special-linear-lie-algebra) $\mathfrak{sl}_n(\mathbb C)$. Write $\varepsilon_i(\operatorname{diag}(h_1,\ldots,h_n))=h_i$, so $\sum_i\varepsilon_i=0$. The standard coordinate vectors $e_i$ are [weight vectors](../../../semisimple-lie-algebra.md#weight-vector) of weights $\varepsilon_i$, and the [tensor product of Lie algebra representations](../../../lie-algebra.md#tensor-product-of-lie-algebra-representations) has basis

$$
e_i\otimes(e_j\wedge e_k),\qquad 1\le i\le n,\quad j<k.
$$

The [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) of this basis vector is $\varepsilon_i+\varepsilon_j+\varepsilon_k$. There are two possibilities:

$$
\boxed{\begin{array}{c|c|c}
\text{weight}&\text{indices}&\text{weight-space dimension}\\\hline
2\varepsilon_a+\varepsilon_b&a\ne b&1\\
\varepsilon_a+\varepsilon_b+\varepsilon_c&a<b<c&3
\end{array}}
$$

The first has basis $e_a\otimes(e_a\wedge e_b)$, with the wedge ordered if necessary. In the second, the tensor's first factor can be any one of the three indicated coordinate vectors. No two different listed coefficient patterns restrict to the same functional on the traceless diagonal [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra): their difference would have to be a multiple of $(1,\ldots,1)$, but its coefficient sum is zero. All unlisted [weight spaces](../../../semisimple-lie-algebra.md#weight-space) are zero. As a check,

$$
n(n-1)+3\binom n3=\frac{n^2(n-1)}2=\dim(V\otimes\Lambda^2V).
$$

For $n=3$, the distinct-index [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) is zero and has multiplicity three.

To determine the irreducible summands, take the upper triangular [raising operators](../../../semisimple-lie-algebra.md#raising-operator). The vector $v_1=e_1\otimes(e_1\wedge e_2)$ is killed by every such operator and has [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) $2\varepsilon_1+\varepsilon_2=\omega_1+\omega_2$. The [exterior product](../../../linear-algebra.md#exterior-product) map

$$
A:V\otimes\Lambda^2V\longrightarrow\Lambda^3V,\qquad A(v\otimes(u\wedge w))=v\wedge u\wedge w
$$

is a [Lie algebra representation homomorphism](../../../lie-algebra.md#lie-algebra-representation-homomorphism). It has an equivariant right inverse

$$
\iota(e_a\wedge e_b\wedge e_c)=\frac13\left[e_a\otimes(e_b\wedge e_c)-e_b\otimes(e_a\wedge e_c)+e_c\otimes(e_a\wedge e_b)\right].
$$

Indeed $A\iota=I$. The vector $\iota(e_1\wedge e_2\wedge e_3)$ is a [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector) of [weight](../../../semisimple-lie-algebra.md#weight-representation-theory) $\varepsilon_1+\varepsilon_2+\varepsilon_3$.

The [Weyl complete reducibility theorem](../../../semisimple-lie-algebra.md#weyl-complete-reducibility-theorem) and [highest-weight representation](../../../semisimple-lie-algebra.md#highest-weight-representation) theory show that $v_1$ generates an irreducible summand in $\ker A$. To check that it exhausts this [kernel](../../../linear-algebra.md#kernel-of-a-linear-map), use the [Weyl dimension formula](../../../semisimple-lie-algebra.md#weyl-dimension-formula) with the partition $(2,1,0,\ldots,0)$:

$$
\dim L(\omega_1+\omega_2)=\prod_{i<j}\frac{\lambda_i-\lambda_j+j-i}{j-i}
=2\prod_{j=3}^n\frac{j+1}{j-1}\prod_{j=3}^n\frac{j-1}{j-2}
=\frac{n(n^2-1)}3.
$$

This equals $\dim\ker A=n\binom n2-\binom n3$. The [exterior-power Lie algebra representation](../../../lie-algebra.md#exterior-power-lie-algebra-representation) $\Lambda^3V$ is irreducible, with [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) $\omega_3$ for $n\ge4$, and is the one-dimensional trivial representation for $n=3$. Therefore the [tensor product of the standard representation with its exterior square](../../../lie-algebra.md#tensor-product-of-the-standard-representation-with-its-exterior-square) gives

$$
\boxed{V\otimes\Lambda^2V\cong\begin{cases}
L(\omega_1+\omega_2)\oplus L(\omega_3),&n\ge4,\\
L(\omega_1+\omega_2)\oplus L(0),&n=3.
\end{cases}}
$$

Each summand occurs once; their [dimensions](../../../vector-space.md#dimension-vector-space) are $n(n^2-1)/3$ and $\binom n3$.

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Write an element of the [symplectic Lie algebra](../../../semisimple-lie-algebra.md#symplectic-lie-algebra) in $n\times n$ blocks. Direct multiplication in $AJ+JA^T=0$ gives

$$
A=\begin{pmatrix}P&Q\\R&-P^T\end{pmatrix},\qquad Q^T=Q,\quad R^T=R.
$$

The diagonal [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) consists of $H=\operatorname{diag}(h_1,\ldots,h_n,-h_1,\ldots,-h_n)$. Define $\varepsilon_i(H)=h_i$. Under the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra), the off-diagonal [matrix units](../../../vector-space.md#matrix-unit) in $P$ have [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) $\varepsilon_i-\varepsilon_j$; the symmetric entries in $Q$ have [weights](../../../semisimple-lie-algebra.md#weight-representation-theory) $\varepsilon_i+\varepsilon_j$, including $2\varepsilon_i$ on the diagonal; those in $R$ have the negatives of these weights. All nonzero [root spaces](../../../semisimple-lie-algebra.md#root-space) are one-dimensional, while the zero [weight space](../../../semisimple-lie-algebra.md#weight-space) is the diagonal [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra). Thus the [Cn root system](../../../semisimple-lie-algebra.md#cn-root-system) is

$$
\boxed{R=\{\pm\varepsilon_i\pm\varepsilon_j:i<j\}\cup\{\pm2\varepsilon_i:1\le i\le n\}.}
$$

Choose the [positive roots](../../../semisimple-lie-algebra.md#positive-root) and [simple roots](../../../semisimple-lie-algebra.md#simple-root) as

$$
\boxed{R^+=\{\varepsilon_i-\varepsilon_j,\varepsilon_i+\varepsilon_j:i<j\}\cup\{2\varepsilon_i\},\qquad
\Delta=\{\alpha_i=\varepsilon_i-\varepsilon_{i+1}:i<n\}\cup\{\alpha_n=2\varepsilon_n\}.}
$$

Their [highest root](../../../semisimple-lie-algebra.md#highest-root) and [Weyl vector](../../../semisimple-lie-algebra.md#half-sum-of-positive-roots) are

$$
\boxed{\theta=2\varepsilon_1=2\alpha_1+\cdots+2\alpha_{n-1}+\alpha_n,\qquad
\rho=\frac12\sum_{\alpha\in R^+}\alpha=\sum_{i=1}^n(n-i+1)\varepsilon_i.}
$$

For the last identity, each pair $i<j$ contributes $2\varepsilon_i$ before division by two, and the long positive root contributes another $\varepsilon_i$ afterward. Successive [simple roots](../../../semisimple-lie-algebra.md#simple-root) have equal length except for $\alpha_n$, whose squared length is twice that of $\alpha_{n-1}$. The [Cn Dynkin diagram](../../../semisimple-lie-algebra.md#cn-dynkin-diagram) is a chain with a double last bond, whose arrow points toward $\alpha_{n-1}$, the short root:<a id="4/a/image-the-cn-dynkin-diagram-with-its-simple-root-labels-and-arrow-toward-the-short-root"></a>


![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-1-cn-dynkin.png)

**[Figure 1](#4/a/image-the-cn-dynkin-diagram-with-its-simple-root-labels-and-arrow-toward-the-short-root). The Cn Dynkin diagram with its simple-root labels and arrow toward the short root**.

The displayed schematic is for $n\ge4$; omit intermediate nodes for $n=2,3$. For $n=1$ the diagram has just the single node $\alpha_1=2\varepsilon_1$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $V=\mathbb C^4$ with its [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form) [alternating bilinear form](../../../linear-algebra.md#alternating-bilinear-form). Its inverse-form bivector $\Omega\in\Lambda^2V$ is invariant under the [symplectic Lie algebra](../../../semisimple-lie-algebra.md#symplectic-lie-algebra), and $\Omega\wedge\Omega\ne0$. Choose $\operatorname{vol}=\Omega\wedge\Omega/2$. The [exterior product](../../../linear-algebra.md#exterior-product) defines a [symmetric bilinear form](../../../linear-algebra.md#symmetric-bilinear-form) on $\Lambda^2V$ by

$$
\xi\wedge\eta=B(\xi,\eta)\operatorname{vol}.
$$

It is symmetric because two-forms commute under the wedge product. It is [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form) because each basis wedge $e_i\wedge e_j$ pairs with its complementary basis wedge. Since $B(\Omega,\Omega)=2$, the five-dimensional [orthogonal complement](../../../hilbert-space.md#orthogonal-complement)

$$
W=\Omega^\perp=\Lambda_0^2V
$$

also has a [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form) [symmetric bilinear form](../../../linear-algebra.md#symmetric-bilinear-form). This is the [primitive exterior square](../../../linear-algebra.md#primitive-exterior-square), equivalently the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) of [symplectic contraction of an exterior square](../../../linear-algebra.md#symplectic-contraction-of-an-exterior-square).

Every element of $\mathfrak{sp}_4$ fixes $\Omega$ and preserves volume, since its [trace](../../../linear-algebra.md#matrix-trace) is zero. The induced [exterior-power Lie algebra representation](../../../lie-algebra.md#exterior-power-lie-algebra-representation) consequently preserves $W$ and satisfies $B(A\xi,\eta)+B(\xi,A\eta)=0$. Thus it gives a [Lie algebra homomorphism](../../../lie-algebra.md#lie-algebra-homomorphism)

$$
\varphi:\mathfrak{sp}_4\longrightarrow\mathfrak{so}(W,B).
$$

We check [injectivity](../../../algebra.md#injective-function) explicitly. If $A$ acts as zero on $W$, it also kills $\Omega$, and therefore acts as zero on all of $\Lambda^2V=W\oplus\mathbb C\Omega$. For three distinct indices $i,j,k$, the coefficient of $e_k\wedge e_j$ in $A(e_i\wedge e_j)$ is $A_{ki}$, so all off-diagonal entries of $A$ vanish. Its action on $e_i\wedge e_j$ is then $(A_{ii}+A_{jj})e_i\wedge e_j$. All these sums vanish, which in characteristic zero forces every diagonal entry to vanish. Hence $A=0$.

Finally,

$$
\dim\mathfrak{sp}_4=4+3+3=10=\frac{5\cdot4}{2}=\dim\mathfrak{so}(W,B).
$$

The injective [Lie algebra homomorphism](../../../lie-algebra.md#lie-algebra-homomorphism) is therefore surjective. Over $\mathbb C$, every [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form) [symmetric bilinear form](../../../linear-algebra.md#symmetric-bilinear-form) admits a basis in which its matrix is the identity, so this constructs the [exceptional isomorphism between sp4 and so5](../../../semisimple-lie-algebra.md#exceptional-isomorphism-between-sp4-and-so5):

$$
\boxed{\mathfrak{sp}_4(\mathbb C)\cong\mathfrak{so}_5(\mathbb C).}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Identify the diagonal [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) with $\mathbb C^n$ through its coordinates $(h_1,\ldots,h_n)$, and identify real roots with coordinate vectors using the invariant Euclidean [inner product](../../../linear-algebra.md#inner-product). A [Weyl reflection](../../../semisimple-lie-algebra.md#weyl-reflection) is $s_\alpha(h)=h-2(h,\alpha)\alpha/(\alpha,\alpha)$. It does not change when $\alpha$ is replaced by $-\alpha$. For the [Cn root system](../../../semisimple-lie-algebra.md#cn-root-system), its explicit actions are

$$
\boxed{\begin{array}{c|c}
\text{root, up to sign}&\text{changed coordinates}\\\hline
2\varepsilon_i&h_i\mapsto-h_i\\
\varepsilon_i-\varepsilon_j&(h_i,h_j)\mapsto(h_j,h_i)\\
\varepsilon_i+\varepsilon_j&(h_i,h_j)\mapsto(-h_j,-h_i)
\end{array}}
$$

Every coordinate not displayed stays fixed. Thus each generating [Weyl reflection](../../../semisimple-lie-algebra.md#weyl-reflection) is a signed permutation, so the [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) is contained in the [signed symmetric group](../../../lie-theory.md#hyperoctahedral-group). Conversely, the first row supplies each independent sign change and the second supplies every coordinate [transposition](../../../combinatorics.md#transposition-permutation); these generate the entire [signed symmetric group](../../../lie-theory.md#hyperoctahedral-group). This proves the [Cn Weyl group](../../../semisimple-lie-algebra.md#cn-weyl-group) identification, including its size:

$$
\boxed{W\cong(\mathbb Z/2\mathbb Z)^n\rtimes S_n,\qquad |W|=2^nn!.}
$$

## 5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Suppose that $H$ is not a [discrete subgroup](../../../topological-group.md#discrete-subgroup). The identity is then an accumulation point of nonidentity subgroup elements: translate any failure of isolation to the identity. Choose $h_j\in H\setminus\{e\}$ with $h_j\to e$, and use a [local exponential chart](../../../lie-theory.md#local-exponential-chart) to write $h_j=\exp X_j$, where $X_j\ne0$ and $X_j\to0$ in the real [Lie algebra](../../../lie-algebra.md) $\mathfrak g$.

Choose a [norm](../../../functional-analysis.md#norm) on this finite-dimensional [vector space](../../../vector-space.md). By [compactness](../../../topology.md#compact-space) of its unit sphere, pass to a subsequence with $X_j/\|X_j\|\to X$, where $\|X\|=1$. For an arbitrary real $t$, choose an [integer](../../../number-theory.md#integer) $m_j$ nearest to $t/\|X_j\|$. Then $m_j\|X_j\|\to t$ and

$$
h_j^{m_j}=\exp(m_jX_j)\longrightarrow\exp(tX).
$$

Every left-hand element belongs to $H$, including for negative $m_j$. Closedness gives $\exp(tX)\in H$. Since $t$ was arbitrary and $X\ne0$, the [limit directions of a closed subgroup](../../../lie-theory.md#limit-directions-of-a-closed-subgroup) provide a nontrivial [one-parameter subgroup](../../../lie-theory.md#one-parameter-subgroup) in $H$. Its derivative at zero is $X$, so it cannot be the constant subgroup.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Define

$$
\mathfrak h=\{X\in\mathfrak g:\exp(tX)\in H\text{ for every }t\in\mathbb R\}.
$$

It contains zero, and $X\in\mathfrak h$ implies $aX\in\mathfrak h$ for every real scalar $a$, by replacing $t$ with $at$.

For $X,Y\in\mathfrak h$, we prove closure under addition using the [Lie product formula in a Lie group](../../../lie-theory.md#lie-product-formula-in-a-lie-group). In the [local exponential chart](../../../lie-theory.md#local-exponential-chart), let $Z(s)=\log(\exp(sX)\exp(sY))$. Smooth multiplication has differential $(U,V)\mapsto U+V$ at the identity, so [Taylor's theorem](../../../calculus.md#taylor-theorem) gives

$$
Z(s)=s(X+Y)+O(s^2).
$$

For each fixed real $t$ and all sufficiently large positive [integers](../../../number-theory.md#integer) $m$,

$$
\left[\exp(tX/m)\exp(tY/m)\right]^m=\exp\bigl(mZ(t/m)\bigr)
\longrightarrow\exp(t(X+Y)).
$$

Every term belongs to $H$, and $H$ is closed, proving $X+Y\in\mathfrak h$. Thus $\mathfrak h$ is a real [vector subspace](../../../vector-space.md#vector-subspace). It is also closed: if $X_j\to X$ with $X_j\in\mathfrak h$, continuity of the [Exponential map of a Lie group](../../../lie-theory.md#exponential-map-of-a-lie-group) gives $\exp(tX)\in H$ for each $t$.

For the [Lie bracket](../../../lie-algebra.md#lie-bracket), use the [Adjoint representation of a Lie group](../../../lie-theory.md#adjoint-representation-of-a-lie-group). Conjugating a [one-parameter subgroup](../../../lie-theory.md#one-parameter-subgroup) gives

$$
\exp(sX)\exp(tY)\exp(-sX)=\exp\bigl(t\operatorname{Ad}_{\exp(sX)}Y\bigr)\in H.
$$

Consequently $\operatorname{Ad}_{\exp(sX)}Y\in\mathfrak h$. For $s\ne0$, linearity puts $\bigl(\operatorname{Ad}_{\exp(sX)}Y-Y\bigr)/s$ in $\mathfrak h$. Its limit as $s\to0$ is $\operatorname{ad}_XY=[X,Y]$. Closedness of $\mathfrak h$ therefore gives $[X,Y]\in\mathfrak h$, proving that the [Lie algebra of a closed subgroup](../../../lie-theory.md#lie-algebra-of-a-closed-subgroup) is a [Lie subalgebra](../../../lie-algebra.md#lie-subalgebra) of $\mathfrak g$.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Choose a real [vector subspace](../../../vector-space.md#vector-subspace) $\mathfrak m$ complementary to $\mathfrak h$, so $\mathfrak g=\mathfrak m\oplus\mathfrak h$. The smooth map

$$
F:\mathfrak m\times\mathfrak h\longrightarrow G,\qquad F(U,V)=\exp U\exp V
$$

has differential $(U,V)\mapsto U+V$ at $(0,0)$, an [isomorphism](../../../algebra.md#isomorphism). The [inverse function theorem](../../../calculus.md#inverse-function-theorem) makes $F$ a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) from a sufficiently small product neighborhood onto an open neighborhood of the identity in $G$.

There is a neighborhood of zero in $\mathfrak m$ in which $\exp U\in H$ implies $U=0$. Otherwise choose nonzero $U_j\in\mathfrak m$ tending to zero with $\exp U_j\in H$. A normalized subsequence tends to a unit vector $U\in\mathfrak m$. The [limit directions of a closed subgroup](../../../lie-theory.md#limit-directions-of-a-closed-subgroup) from part (a) give $U\in\mathfrak h$, contradicting $\mathfrak m\cap\mathfrak h=0$. Shrink the product neighborhood so that this exclusion holds throughout its first factor.

If $F(U,V)\in H$, then $\exp V\in H$ by the definition of $\mathfrak h$, and hence $\exp U=F(U,V)\exp(-V)\in H$. The exclusion forces $U=0$. Conversely, every $F(0,V)=\exp V$ belongs to $H$. Thus the [local product coordinates for a closed subgroup](../../../lie-theory.md#local-product-coordinates-for-a-closed-subgroup) identify $H$ near the identity exactly with the smooth coordinate slice $U=0$.

Left translation by each element of $H$ gives the same description around that element, so $H$ is an [embedded submanifold](../../../differential-geometry.md#embedded-submanifold) of $G$ in its subspace topology. The multiplication and inversion maps of $G$ restrict to smooth maps on this [embedded submanifold](../../../differential-geometry.md#embedded-submanifold), making $H$ a [Lie group](../../../lie-theory.md#lie-group) and an embedded [Lie subgroup](../../../lie-theory.md#lie-subgroup). Its tangent space at the identity is $\mathfrak h$, because $d\exp_0$ is the identity on this coordinate slice. It remains closed by hypothesis. This proves the [closed-subgroup theorem](../../../lie-theory.md#closed-subgroup-theorem), with no prior smoothness assumption on $H$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
