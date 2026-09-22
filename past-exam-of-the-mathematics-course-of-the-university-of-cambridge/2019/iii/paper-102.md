# Paper 102

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_102.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_102.pdf)

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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)

## 1

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

An [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra) is a [vector subspace](../../../vector-space.md#vector-subspace) $I\subseteq\mathfrak g$ such that $[\mathfrak g,I]\subseteq I$. The [derived series of a Lie algebra](../../../lie-algebra.md#derived-series-of-a-lie-algebra) is defined by $\mathfrak g^{(0)}=\mathfrak g$ and $\mathfrak g^{(r+1)}=[\mathfrak g^{(r)},\mathfrak g^{(r)}]$.

Suppose that $I$ is an ideal and $x\in\mathfrak g$, $u,v\in I$. The [Jacobi identity](../../../lie-algebra.md#jacobi-identity) gives

$$
[x,[u,v]]=[[x,u],v]+[u,[x,v]].
$$

Both terms on the right lie in $[I,I]$, because $[x,u],[x,v]\in I$. Thus $[I,I]$ is again an ideal. Starting from the ideal $\mathfrak g$ and applying this observation inductively proves that **every term $\mathfrak g^{(r)}$ of the derived series is an ideal of $\mathfrak g$**.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A [simple Lie algebra](../../../semisimple-lie-algebra.md#simple-lie-algebra) is a nonabelian [Lie algebra](../../../lie-algebra.md) whose only [ideals of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra) are $0$ and the whole algebra.

Use the standard basis $e,f,h$ of the [sl2 Lie algebra](../../../semisimple-lie-algebra.md#sl2-lie-algebra), with

$$
[h,e]=2e,\qquad [h,f]=-2f,\qquad [e,f]=h.
$$

Let $I\ne0$ be an ideal and choose $0\ne x=ae+bf+ch\in I$. Since $I$ is invariant under the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra), it is invariant under the [linear operator](../../../vector-space.md#linear-operator) $\operatorname{ad}h$. The three basis vectors are [eigenvectors](../../../linear-operator-theory.md#eigenvector) of $\operatorname{ad}h$ with distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $2,-2,0$. Applying the corresponding polynomial spectral projections to $x$ shows that $I$ contains at least one nonzero multiple of $e$, $f$, or $h$.

If $e\in I$, then $[f,e]=-h\in I$ and $[f,h]=2f\in I$; the cases $f\in I$ and $h\in I$ are identical after taking brackets with the other basis vectors. Hence $e,f,h\in I$, so $I=\mathfrak{sl}_2(\mathbb C)$. Therefore **$\mathfrak{sl}_2(\mathbb C)$ is simple**.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [Killing form](../../../lie-algebra.md#killing-form) of a finite-dimensional [Lie algebra](../../../lie-algebra.md) $\mathfrak g$ is the [symmetric bilinear form](../../../linear-algebra.md#symmetric-bilinear-form)

$$
\kappa(x,y)=\operatorname{tr}(\operatorname{ad}x\,\operatorname{ad}y).
$$

The cyclicity of the [trace](../../../linear-algebra.md#matrix-trace) makes it invariant:

$$
\kappa([x,y],z)=\kappa(x,[y,z]).
$$

Consequently its [radical of a bilinear form](../../../linear-algebra.md#radical-of-a-bilinear-form) $R=\{x:\kappa(x,\mathfrak g)=0\}$ is an ideal, since $x\in R$ implies $\kappa([y,x],z)=\kappa(x,[z,y])=0$ for all $y,z\in\mathfrak g$.

If $\mathfrak g$ is simple, then $R$ is either $0$ or $\mathfrak g$. In the second case the Killing form vanishes identically, so the stated solvability criterion makes $\mathfrak g$ a [solvable Lie algebra](../../../lie-algebra.md#solvable-lie-algebra). A nonabelian simple Lie algebra cannot be solvable: its first derived algebra is a nonzero ideal and hence equals $\mathfrak g$, after which the derived series never reaches zero. Thus $R=0$, and **the Killing form of a simple Lie algebra is nondegenerate**.

## 2

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Write an element of the diagonal [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra) as

$$
t=\operatorname{diag}(t_1,t_2,t_3,-t_1,-t_2,-t_3)
$$

and define the [linear functionals](../../../linear-algebra.md#linear-functional) $\varepsilon_i(t)=t_i$. The [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition) of the [symplectic Lie algebra](../../../semisimple-lie-algebra.md#symplectic-lie-algebra) $\mathfrak{sp}_6(\mathbb C)$ then has the [C3 root system](../../../semisimple-lie-algebra.md#c3-root-system)

$$
\boxed{\Phi=\{\pm\varepsilon_i\pm\varepsilon_j:1\leq i<j\leq3\}\cup\{\pm2\varepsilon_i:1\leq i\leq3\}.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

A convenient [root basis](../../../semisimple-lie-algebra.md#fundamental-system-of-a-root-system) is

$$
\boxed{\alpha_1=\varepsilon_1-\varepsilon_2,\qquad
\alpha_2=\varepsilon_2-\varepsilon_3,\qquad
\alpha_3=2\varepsilon_3.}
$$

The corresponding [Cartan matrix](../../../semisimple-lie-algebra.md#cartan-matrix) is

$$
\left(\langle\alpha_i,\alpha_j^\vee\rangle\right)_{ij}
=\begin{pmatrix}
2&-1&0\\
-1&2&-1\\
0&-2&2
\end{pmatrix}.
$$

Thus the [Dynkin diagram](../../../semisimple-lie-algebra.md#dynkin-diagram) is the three-node $C_3$ chain, with a double edge between $\alpha_2$ and $\alpha_3$ and its arrow pointing toward the shorter root $\alpha_2$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The [Weyl reflection](../../../semisimple-lie-algebra.md#weyl-reflection) formula $s_i(\beta)=\beta-\langle\beta,\alpha_i^\vee\rangle\alpha_i$, together with the [Cartan matrix](../../../semisimple-lie-algebra.md#cartan-matrix), gives

$$
\begin{array}{c|ccc}
&\alpha_1&\alpha_2&\alpha_3\\ \hline
s_1&-\alpha_1&\alpha_1+\alpha_2&\alpha_3\\
s_2&\alpha_1+\alpha_2&-\alpha_2&2\alpha_2+\alpha_3\\
s_3&\alpha_1&\alpha_2+\alpha_3&-\alpha_3
\end{array}.
$$

These are **the images of every simple root under each simple reflection**.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

With the Euclidean inner product used above, the simple [coroots](../../../semisimple-lie-algebra.md#coroot) are

$$
\boxed{\alpha_1^\vee=\varepsilon_1-\varepsilon_2,\qquad
\alpha_2^\vee=\varepsilon_2-\varepsilon_3,\qquad
\alpha_3^\vee=\varepsilon_3.}
$$

Indeed, if a positive root is $\beta=\sum_i n_i\alpha_i$, then

$$
\beta^\vee=\sum_i n_i\frac{(\alpha_i,\alpha_i)}{(\beta,\beta)}\alpha_i^\vee,
$$

whose coefficients are nonnegative. The negative roots give the negatives of these combinations, so the displayed coroots form a [fundamental system of a root system](../../../semisimple-lie-algebra.md#fundamental-system-of-a-root-system) for the [dual root system](../../../semisimple-lie-algebra.md#dual-root-system).

Duality reverses root lengths. The dual of $C_3$ is therefore the [B3 root system](../../../semisimple-lie-algebra.md#b3-root-system): its [Dynkin diagram](../../../semisimple-lie-algebra.md#dynkin-diagram) is again a three-node chain with a double final edge, but its arrow points toward the now-short root $\alpha_3^\vee$.

## 3

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For $t\in\mathfrak t$, the [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition) gives its [centralizer](../../../group-theory.md#centralizer)

$$
\mathfrak z_{\mathfrak g}(t)
=\mathfrak t\oplus\bigoplus_{\alpha(t)=0}\mathfrak g_\alpha.
$$

Every root space is one-dimensional, so this centralizer has the minimum possible dimension $\ell=\dim\mathfrak t$ exactly when no summand on the right occurs. By the [Regular element criterion in a Cartan subalgebra](../../../semisimple-lie-algebra.md#regular-element-criterion-in-a-cartan-subalgebra),

$$
\boxed{t\text{ is regular}\iff \alpha(t)\ne0\text{ for every root }\alpha.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Choose a [positive system of a root system](../../../semisimple-lie-algebra.md#positive-system-of-a-root-system) in which $\alpha$ is a [simple root](../../../semisimple-lie-algebra.md#simple-root); this is possible after applying an element of the [Weyl group](../../../semisimple-lie-algebra.md#weyl-group). Let $\theta$ be the [highest root](../../../semisimple-lie-algebra.md#highest-root). Since the rank is greater than one, $\theta\ne\alpha$, and the maximality of $\theta$ implies that $\theta+\alpha$ is not a root.

For $0\ne x\in\mathfrak g_\alpha$, the $(\ell-1)$-dimensional space $\ker\alpha\subset\mathfrak t$ centralizes $x$. The line $\mathbb Cx$ also centralizes $x$, and $[x,\mathfrak g_\theta]\subseteq\mathfrak g_{\alpha+\theta}=0$. These independent spaces give

$$
\dim\mathfrak z_{\mathfrak g}(x)\geq(\ell-1)+1+1=\ell+1.
$$

Hence **a nonzero simple-root vector is not regular when $\ell>1$**.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Put $h_0=\psi(h)$ and $e_0=\psi(e)=\sum_{i=1}^{\ell}e_i$, where $0\ne e_i\in\mathfrak g_{\alpha_i}$. Since $[h_0,e_0]=2e_0$ and the [root spaces](../../../semisimple-lie-algebra.md#root-space) are a [direct sum](../../../vector-space.md#direct-sum), $\alpha_i(h_0)=2$ for every simple root. Every root has simple-root coefficients of one sign, so no root vanishes on $h_0$. The [Regular element criterion in a Cartan subalgebra](../../../semisimple-lie-algebra.md#regular-element-criterion-in-a-cartan-subalgebra) therefore shows that **$h_0$ is regular**.

Restrict the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) of $\mathfrak g$ along $\psi$. By [complete reducibility of semisimple Lie algebra representations](../../../semisimple-lie-algebra.md#weyl-s-theorem-on-complete-reducibility), it is a direct sum of finite-dimensional [sl2 Lie algebra](../../../semisimple-lie-algebra.md#sl2-lie-algebra) modules. The $h_0$-eigenvalues on a root space are twice the heights of the roots, so they are all even. Each irreducible summand consequently has even highest weight, contains exactly one zero-weight vector, and has a one-dimensional kernel for the raising operator $e_0$ by the [classification of finite-dimensional sl2 representations](../../../semisimple-lie-algebra.md#classification-of-finite-dimensional-sl2-representations).

Because $h_0$ is regular, its zero-weight space in $\mathfrak g$ is precisely $\mathfrak t$ and has dimension $\ell$. There are therefore exactly $\ell$ irreducible summands, whence

$$
\dim\ker(\operatorname{ad}e_0)=\ell.
$$

Thus **$e_0$ is regular**; equivalently it is a [principal nilpotent element](../../../semisimple-lie-algebra.md#principal-nilpotent-element) in the given [Principal sl2 subalgebra](../../../semisimple-lie-algebra.md#principal-sl2-subalgebra).

## 4

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For a dominant integral [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation) $\lambda$, the [Weyl dimension formula](../../../semisimple-lie-algebra.md#weyl-dimension-formula) is

$$
\boxed{\dim V(\lambda)=\prod_{\alpha\in\Phi^+}
\frac{\langle\lambda+\rho,\alpha^\vee\rangle}
{\langle\rho,\alpha^\vee\rangle},}
$$

where $\Phi^+$ is the chosen [positive system of a root system](../../../semisimple-lie-algebra.md#positive-system-of-a-root-system), $\alpha^\vee$ is a [coroot](../../../semisimple-lie-algebra.md#coroot), and $\rho$ is the [Weyl vector](../../../semisimple-lie-algebra.md#half-sum-of-positive-roots).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For the [B2 root system](../../../semisimple-lie-algebra.md#b2-root-system) with $\alpha_1$ short, the positive roots are

$$
\alpha_1,\quad\alpha_2,\quad\alpha_1+\alpha_2,\quad2\alpha_1+\alpha_2.
$$

Substituting $\lambda=a\omega_1+b\omega_2$ into the [Weyl dimension formula for B2](../../../semisimple-lie-algebra.md#weyl-dimension-formula-for-b2) gives

$$
\boxed{\dim V(a\omega_1+b\omega_2)
=\frac{(a+1)(b+1)(a+b+2)(a+2b+3)}6.}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let $V=V(\omega_2)$ be the five-dimensional defining representation of the [so5 Lie algebra](../../../semisimple-lie-algebra.md#so5-lie-algebra). The [tensor square](../../../linear-algebra.md#tensor-square) splits into its [symmetric square](../../../linear-algebra.md#symmetric-square) and [exterior square](../../../linear-algebra.md#exterior-square):

$$
V\otimes V=S^2V\oplus\Lambda^2V.
$$

The invariant symmetric form spans a trivial subrepresentation of $S^2V$, while its traceless complement is the irreducible $V(2\omega_2)$ of dimension $14$. The identification $\Lambda^2V\cong\mathfrak{so}_5$ makes the exterior square the ten-dimensional [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra), whose highest weight is the highest root $2\omega_1$. Therefore the [Tensor-square decomposition of the defining so5 representation](../../../semisimple-lie-algebra.md#tensor-square-decomposition-of-the-defining-so5-representation) is

$$
\boxed{V\otimes V\cong V(0)\oplus V(2\omega_1)\oplus V(2\omega_2).}
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The [Poincaré-Birkhoff-Witt theorem](../../../lie-algebra.md#poincare-birkhoff-witt-theorem) shows that the weights of the [Verma module](../../../semisimple-lie-algebra.md#verma-module) $M(\omega_2)$ are

$$
\boxed{\omega_2-Q_+
=\{\omega_2-n_1\alpha_1-n_2\alpha_2:n_1,n_2\in\mathbb Z_{\geq0}\},}
$$

with multiplicities given by the corresponding [Kostant partition function](../../../semisimple-lie-algebra.md#kostant-partition-function).

The [Dynkin labels](../../../semisimple-lie-algebra.md#dynkin-label) of $\omega_2$ are $(0,1)$. Hence the two simple-root [singular vectors](../../../semisimple-lie-algebra.md#singular-vector) are $f_1v_{\omega_2}$, of weight $\omega_2-\alpha_1$, and $f_2^2v_{\omega_2}$, of weight $\omega_2-2\alpha_2$. They generate the [Maximal proper submodule of a dominant integral Verma module](../../../semisimple-lie-algebra.md#maximal-proper-submodule-of-a-dominant-integral-verma-module). Its set of weights is consequently

$$
\boxed{(\omega_2-\alpha_1-Q_+)\ \cup\ (\omega_2-2\alpha_2-Q_+).}
$$

## 5

↑ **Parent:** [Paper 102](paper-102.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Let $C(\Delta)$ be the [fundamental chamber of a root system](../../../semisimple-lie-algebra.md#fundamental-chamber-of-a-root-system) determined by $\Delta$. Every positive root is a nonnegative linear combination of the simple roots, so every point in the interior of $C(\Delta)$ pairs strictly positively with every positive root. In particular, the interior meets none of the reflecting hyperplanes belonging to the subsystem $\Phi_0$ of roots of maximal length.

The connected set $C(\Delta)$ therefore lies in one chamber of the [long-root subsystem](../../../semisimple-lie-algebra.md#long-root-subsystem). Let $\Delta_0$ be the unique [fundamental system of a root system](../../../semisimple-lie-algebra.md#fundamental-system-of-a-root-system) defining that chamber. Taking closures gives $C(\Delta)\subseteq C(\Delta_0)$. Uniqueness follows because the interiors of two distinct chambers are disjoint. Thus **there is a unique such $\Delta_0$**.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Write the simple roots of the [G2 root system](../../../semisimple-lie-algebra.md#g2-root-system) as $\alpha$ short and $\beta$ long. The [Long-root A2 subsystem of G2](../../../semisimple-lie-algebra.md#long-root-a2-subsystem-of-g2) has simple roots

$$
\delta_1=\beta,\qquad\delta_2=3\alpha+\beta.
$$

If $\omega_1,\omega_2$ are its [fundamental weights](../../../semisimple-lie-algebra.md#fundamental-weight), then the $A_2$ root-weight relations give

$$
\alpha=\omega_2-\omega_1,\qquad
\alpha^\vee=\delta_2^\vee-\delta_1^\vee,\qquad
\beta^\vee=\delta_1^\vee.
$$

For the $A_2$-dominant weight $\lambda=a\omega_1+b\omega_2$, therefore,

$$
\langle\lambda,\beta^\vee\rangle=a,
\qquad
\langle\lambda,\alpha^\vee\rangle=b-a.
$$

The [dominant weight](../../../semisimple-lie-algebra.md#dominant-weight) inequalities for $G_2$ are thus equivalent to

$$
\boxed{b\geq a}
$$

because $A_2$-dominance already gives $a,b\geq0$.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The weights of the seven-dimensional irreducible $G_2$ representation are zero and the six short roots. In the $A_2$ [weight lattice](../../../semisimple-lie-algebra.md#weight-lattice), the three positive short roots are

$$
\alpha=\omega_2-\omega_1,\qquad
\alpha+\beta=\omega_1,\qquad
2\alpha+\beta=\omega_2.
$$

Together with their negatives, they split into the weight sets of the two dual three-dimensional [Fundamental representations of sl3](../../../semisimple-lie-algebra.md#fundamental-representations-of-sl3); the zero weight supplies a trivial representation. By the [Restriction of the seven-dimensional G2 representation to long-root A2](../../../semisimple-lie-algebra.md#restriction-of-the-seven-dimensional-g2-representation-to-long-root-a2),

$$
\boxed{V_7\!\downarrow_{\mathfrak{sl}_3}
\cong V(\omega_1)\oplus V(\omega_2)\oplus V(0).}
$$

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

The short-root [Weyl reflection](../../../semisimple-lie-algebra.md#weyl-reflection) $s_\alpha$ interchanges $\omega_1$ and $\omega_2$, because $\alpha=\omega_2-\omega_1$ and $\alpha^\vee=\delta_2^\vee-\delta_1^\vee$. Hence

$$
s_\alpha\lambda=b\omega_1+a\omega_2.
$$

The [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) orbit of the highest weight occurs in $U$ with a one-dimensional [extremal weight space](../../../semisimple-lie-algebra.md#extremal-weight-space). Let $v$ be a nonzero vector of weight $s_\alpha\lambda$. The same reflection exchanges the long simple roots: $s_\alpha\delta_1=\delta_2$ and $s_\alpha\delta_2=\delta_1$. If an $A_2$ raising operator did not annihilate $v$, then $s_\alpha\lambda+\delta_i$ would be a weight of $U$; applying $s_\alpha$ would make $\lambda+\delta_j$ a weight, contradicting the fact that $\lambda$ is the [highest weight](../../../semisimple-lie-algebra.md#highest-weight-of-a-representation).

Thus $v$ is an $A_2$ [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector) of weight $b\omega_1+a\omega_2$. The [complete reducibility of semisimple Lie algebra representations](../../../semisimple-lie-algebra.md#weyl-s-theorem-on-complete-reducibility) then supplies the corresponding irreducible summand, so

$$
\boxed{V(b\omega_1+a\omega_2)\subseteq U\!\downarrow_{\mathfrak{sl}_3}.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
