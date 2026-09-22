# Paper 302

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_302.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_302.pdf)

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

For a [Matrix Lie group](../../../lie-theory.md#matrix-lie-group), the [exponential map of a matrix Lie group](../../../lie-theory.md#exponential-map-of-a-matrix-lie-group) is the convergent [matrix exponential](../../../linear-operator-theory.md#matrix-exponential)

$$
\boxed{\operatorname{Exp}(X)=e^X=\sum_{n=0}^{\infty}\frac{X^n}{n!}.}
$$

Its domain is the [Lie algebra](../../../lie-algebra.md) $\mathfrak g=T_I G$, and $e^{tX}\in G$ for every real $t$ when $X\in\mathfrak g$. Because multiples of the same matrix commute, $e^{sX}e^{tX}=e^{(s+t)X}$ and $(e^{tX})^{-1}=e^{-tX}$. Thus take $I=\mathbb R$ to obtain the image of a [one-parameter subgroup](../../../lie-theory.md#one-parameter-subgroup).

Here is the precise [classification of nontrivial one-parameter subgroups](../../../lie-theory.md#classification-of-nontrivial-one-parameter-subgroups). For $X\ne0$, the smooth [group homomorphism](../../../group-theory.md#group-homomorphism) $\gamma_X:t\mapsto e^{tX}$ has a closed kernel $K\subset\mathbb R$. A closed subgroup of $\mathbb R$ is zero, $\tau\mathbb Z$ for some $\tau>0$, or all of $\mathbb R$. Indeed, if positive elements have infimum zero, their integer multiples approximate every real number, so closedness makes the subgroup all of $\mathbb R$; otherwise the infimum is attained and is its least positive generator. The last possibility is excluded by $\gamma_X'(0)=X\ne0$. Give the image the quotient topology and smooth structure from $\mathbb R/K$. Its inclusion in $G$ is an injective [immersion](../../../differential-geometry.md#immersion), since $\gamma_X'(t)=e^{tX}X$ never vanishes. Consequently it is a [Lie subgroup](../../../lie-theory.md#lie-subgroup), with

$$
\boxed{G_X\cong(\mathbb R,+)\quad\text{or}\quad\mathbb R/(\tau\mathbb Z)\cong S^1.}
$$

In the periodic case $[0,\tau)$ is also a parameter interval covering the image, with endpoints understood modulo $\tau$.

Two qualifications matter. If $X=0$, the image is the trivial group, a third possibility omitted by the wording “two”. Also, a general [one-parameter subgroup](../../../lie-theory.md#one-parameter-subgroup) need not be closed or embedded: an irrational winding $t\mapsto\operatorname{diag}(R(t),R(\sqrt2t))$ in a two-torus is an example, where $R(t)$ is a planar rotation. The classification uses the intrinsic immersed [Lie subgroup](../../../lie-theory.md#lie-subgroup) structure, rather than assuming that the matrix subspace topology is the topology of $\mathbb R$.

For the real [special linear group](../../../group-theory.md#special-linear-group), differentiating $\det(I+tX)=1+t\operatorname{tr}X+O(t^2)$ at the identity shows that its Lie algebra consists of traceless matrices. Conversely $\det e^{tX}=e^{t\operatorname{tr}X}=1$ for a traceless matrix. Hence

$$
\boxed{\mathfrak{sl}_2(\mathbb R)=\left\{\begin{pmatrix}a&b\\c&-a\end{pmatrix}:a,b,c\in\mathbb R\right\}.}
$$

Choose the standard basis of the real [sl2 Lie algebra](../../../semisimple-lie-algebra.md#sl2-lie-algebra),

$$
L_0=\begin{pmatrix}1&0\\0&-1\end{pmatrix},\qquad
L_+=\begin{pmatrix}0&1\\0&0\end{pmatrix},\qquad
L_-=\begin{pmatrix}0&0\\1&0\end{pmatrix}.
$$

Their squares have the required values. Direct matrix multiplication gives the [Lie brackets](../../../lie-algebra.md#lie-bracket)

$$
\boxed{[L_0,L_+]=2L_+,\qquad[L_0,L_-]=-2L_-,\qquad[L_+,L_-]=L_0.}
$$

Writing $[L_a,L_b]=f_{ab}{}^cL_c$, these specify all the nonzero [Lie algebra structure constants](../../../lie-algebra.md#structure-constant-of-a-lie-algebra): $f_{0+}{}^+=2$, $f_{0-}{}^-=-2$, $f_{+-}{}^0=1$, together with their negatives on reversing the lower indices.

The three requested exponentials are

$$
\begin{aligned}
e^{tL_0}&=\begin{pmatrix}e^t&0\\0&e^{-t}\end{pmatrix},&&t\in\mathbb R,\\
e^{tL_+}&=I_2+tL_+=\begin{pmatrix}1&t\\0&1\end{pmatrix},&&t\in\mathbb R,\\
e^{t(L_+-L_-)}&=\begin{pmatrix}\cos t&\sin t\\-\sin t&\cos t\end{pmatrix},&&t\in[0,2\pi).
\end{aligned}
$$

Thus the first two images are isomorphic to the additive real group, while the last is $SO(2)$, the [circle group](../../../lie-theory.md#circle-group). The PDF gives $L_+-L_-$ here; the local TeX's $L_--L_-$ is a transcription error.

For a general generator, put $\Delta=\alpha_0^2+\alpha_+\alpha_-$. Direct multiplication gives $X^2=\Delta I_2$. If $\Delta>0$, the eigenvalues $\pm\sqrt\Delta$ give an unbounded exponential image. If $\Delta=0$ but $X\ne0$, it is a [nilpotent linear map](../../../linear-operator-theory.md#nilpotent-linear-map) with exponential $I_2+tX$, again unbounded. If $\Delta=-\omega^2<0$, the power series instead gives

$$
e^{tX}=\cos(\omega t)I_2+\frac{\sin(\omega t)}\omega X,
$$

with least positive period $2\pi/\omega$. Its image is a continuous image of a circle and is compact. Equivalently, $X/\omega$ is a real complex structure and is similar over $\mathbb R$ to the rotation generator. Therefore the exact criterion for [compact one-parameter subgroups of SL2R](../../../lie-theory.md#compact-one-parameter-subgroups-of-sl2r) is

$$
\boxed{G_X\text{ is compact}\quad\Longleftrightarrow\quad\alpha_0^2+\alpha_+\alpha_-<0\ \text{or}\ (\alpha_0,\alpha_+,\alpha_-)=(0,0,0).}
$$

For a nonzero generator only the strict inequality remains.

## 2

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Work over $\mathbb R$ or $\mathbb C$, in finite dimension and characteristic zero. The [Killing form](../../../lie-algebra.md#killing-form) of a [Lie algebra](../../../lie-algebra.md) is the trace form of its [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra):

$$
\boxed{\kappa(x,y)=\operatorname{tr}(\operatorname{ad}_x\operatorname{ad}_y),\qquad\operatorname{ad}_x(z)=[x,z].}
$$

It is bilinear and symmetric by the [cyclic property of the trace](../../../linear-algebra.md#cyclic-property-of-the-trace). It is an [invariant bilinear form on a Lie algebra](../../../lie-algebra.md#invariant-bilinear-form-on-a-lie-algebra), since the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) gives $\operatorname{ad}_{[x,y]}=[\operatorname{ad}_x,\operatorname{ad}_y]$ and hence

$$
\begin{aligned}
\kappa([x,y],z)
&=\operatorname{tr}([\operatorname{ad}_x,\operatorname{ad}_y]\operatorname{ad}_z)\\
&=\operatorname{tr}(\operatorname{ad}_x[\operatorname{ad}_y,\operatorname{ad}_z])
=\kappa(x,[y,z]).
\end{aligned}
$$

Equivalently, $\kappa([z,x],y)+\kappa(x,[z,y])=0$. A Lie algebra automorphism preserves the form, because it conjugates the adjoint matrices. Its [radical of a bilinear form](../../../linear-algebra.md#radical-of-a-bilinear-form) $\mathfrak r_\kappa=\{x:\kappa(x,\mathfrak g)=0\}$ is an [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra) by invariance. The [center of a Lie algebra](../../../lie-algebra.md#center-of-a-lie-algebra) lies in this radical, so the form vanishes for an abelian algebra. On a direct sum of ideals the summands are orthogonal and the form restricts to their own Killing forms.

A short argument proves the requested implication without assuming the [Cartan criterion for semisimplicity](../../../lie-algebra.md#cartan-criterion-for-semisimplicity). Let $\mathfrak a$ be an abelian [ideal of a Lie algebra](../../../lie-algebra.md#ideal-of-a-lie-algebra), $x\in\mathfrak a$, and $y\in\mathfrak g$. The map $\operatorname{ad}_x$ takes $\mathfrak g$ into $\mathfrak a$ and vanishes on $\mathfrak a$, while $\operatorname{ad}_y$ preserves $\mathfrak a$. Therefore $\operatorname{ad}_x\operatorname{ad}_y$ has image in $\mathfrak a$ and is zero on $\mathfrak a$. In a basis extending a basis of $\mathfrak a$, both diagonal blocks are zero, so its trace vanishes. This proves that [abelian ideals lie in the radical of the Killing form](../../../lie-algebra.md#abelian-ideals-lie-in-the-radical-of-the-killing-form).

If the [solvable radical](../../../lie-algebra.md#radical-of-a-lie-algebra) $\mathfrak r$ were nonzero, its [derived series of a Lie algebra](../../../lie-algebra.md#derived-series-of-a-lie-algebra) would have a last nonzero term $\mathfrak a$. The [Jacobi identity](../../../lie-algebra.md#jacobi-identity) makes every derived term an ideal of $\mathfrak g$, and the last one is abelian. Thus $0\ne\mathfrak a\subseteq\mathfrak r_\kappa$, contradicting nondegeneracy. We obtain

$$
\boxed{\kappa\text{ nondegenerate}\ \Longrightarrow\ \mathfrak r=0\ \Longrightarrow\ \mathfrak g\text{ is a semisimple Lie algebra}.}
$$

The converse holds as well in characteristic zero; together these implications are the [Cartan criterion for semisimplicity](../../../lie-algebra.md#cartan-criterion-for-semisimplicity).

For a complex [simple Lie algebra](../../../semisimple-lie-algebra.md#simple-lie-algebra), that criterion gives nondegeneracy on $\mathfrak g$. Let $\mathfrak h$ be a [Cartan subalgebra](../../../semisimple-lie-algebra.md#cartan-subalgebra). Use the standard [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition)

$$
\mathfrak g=\mathfrak h\oplus\bigoplus_{\alpha\in\Phi}\mathfrak g_\alpha,
\qquad[h,e_\alpha]=\alpha(h)e_\alpha.
$$

For $h,h'\in\mathfrak h$ and a [root vector](../../../semisimple-lie-algebra.md#root-vector) $e_\alpha$, choose $t\in\mathfrak h$ with $\alpha(t)\ne0$. Invariance gives

$$
\alpha(t)\kappa(h,e_\alpha)=\kappa(h,[t,e_\alpha])=\kappa([h,t],e_\alpha)=0.
$$

Thus $\mathfrak h$ is orthogonal to every nonzero [root space](../../../semisimple-lie-algebra.md#root-space). If $h\in\mathfrak h$ is also orthogonal to $\mathfrak h$, it is orthogonal to all of $\mathfrak g$ and hence is zero. This establishes [nondegeneracy of the Killing form on a Cartan subalgebra](../../../semisimple-lie-algebra.md#nondegeneracy-of-the-killing-form-on-a-cartan-subalgebra):

$$
\boxed{\kappa|_{\mathfrak h\times\mathfrak h}\text{ is nondegenerate}.}
$$

The same invariance calculation shows that $\kappa(\mathfrak g_\alpha,\mathfrak g_\beta)=0$ unless $\alpha+\beta=0$. Opposite root spaces are therefore paired nondegenerately. Tracing the adjoint action on the root-space decomposition yields

$$
\kappa(h,h')=\sum_{\alpha\in\Phi}\alpha(h)\alpha(h'),
$$

since the root spaces of a complex semisimple algebra are one-dimensional and its adjoint action on $\mathfrak h$ is zero.

The relevant [Euclidean subspace of a Cartan subalgebra](../../../semisimple-lie-algebra.md#euclidean-subspace-of-a-cartan-subalgebra) is

$$
\mathfrak h_{\mathbb R}=\operatorname{span}_{\mathbb R}\{h_{\alpha_1},\ldots,h_{\alpha_\ell}\}
=\{h\in\mathfrak h:\alpha(h)\in\mathbb R\text{ for all }\alpha\in\Phi\},
$$

where the $h_{\alpha_i}$ are the simple [coroots](../../../semisimple-lie-algebra.md#coroot), normalized by $\alpha_i(h_{\alpha_i})=2$. The standard Euclidean property is that $\kappa$ is real and positive definite on this space. The displayed trace formula explains it: $\kappa(h,h)$ is a sum of real squares, and the roots span $\mathfrak h^*$, so all squares vanish only for $h=0$. Via the nondegenerate form, the roots can consequently be regarded as vectors in a real [Euclidean normed vector space](../../../functional-analysis.md#euclidean-norm). The induced dual [inner product](../../../linear-algebra.md#inner-product) makes [root reflections](../../../semisimple-lie-algebra.md#root-reflection) orthogonal and allows root lengths and angles to be encoded by [Cartan integers](../../../semisimple-lie-algebra.md#cartan-integer) and the [Dynkin diagram](../../../semisimple-lie-algebra.md#dynkin-diagram).

This positivity is on a specified real subspace; the complex Killing form is a bilinear form, not a positive [Hermitian inner product](../../../linear-algebra.md#hermitian-form). On a [compact real form](../../../semisimple-lie-algebra.md#compact-real-form-of-a-complex-semisimple-lie-algebra) the Killing form is instead negative definite. For example the [Killing form of the special linear Lie algebra](../../../lie-algebra.md#killing-form-of-the-special-linear-lie-algebra) gives $\kappa(X,Y)=4\operatorname{tr}(XY)$ for $\mathfrak{sl}_2$, so $\kappa(L_0,L_0)=8$ but $\kappa(iL_0,iL_0)=-8$.

## 3

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use the wiki's [Cartan matrix](../../../semisimple-lie-algebra.md#cartan-matrix) convention

$$
A_{ij}=\langle\alpha_i,\alpha_j^\vee\rangle=\frac{2(\alpha_i,\alpha_j)}{(\alpha_j,\alpha_j)}.
$$

Label the long [simple root](../../../semisimple-lie-algebra.md#simple-root) first when the lengths differ. The matrix of an irreducible rank-two [root system](../../../semisimple-lie-algebra.md#root-system) has the form $A=\begin{pmatrix}2&-a\\-b&2\end{pmatrix}$, where $a,b$ are positive integers. Integrality and the signs follow from the [Cartan integers](../../../semisimple-lie-algebra.md#cartan-integer) for distinct simple roots, and irreducibility rules out a zero off-diagonal pair. Its positive-definite symmetrization gives $ab<4$, equivalently $ab=4\cos^2\theta<4$. Moreover $a/b=\|\alpha_1\|^2/\|\alpha_2\|^2\geq1$. Thus $(a,b)=(1,1),(2,1),(3,1)$, giving the entire [classification of rank-two root systems](../../../semisimple-lie-algebra.md#classification-of-rank-two-root-systems) relevant to a simple algebra:

$$
\boxed{\begin{array}{c|c|c|c}
\text{type}&A&\|\alpha_1\|/\|\alpha_2\|&\theta\\\hline
A_2&\begin{pmatrix}2&-1\\-1&2\end{pmatrix}&1&2\pi/3\\
B_2=C_2&\begin{pmatrix}2&-2\\-1&2\end{pmatrix}&\sqrt2&3\pi/4\\
G_2&\begin{pmatrix}2&-3\\-1&2\end{pmatrix}&\sqrt3&5\pi/6
\end{array}}
$$

These correspond to $\mathfrak{sl}_3(\mathbb C)$, $\mathfrak{so}_5(\mathbb C)\cong\mathfrak{sp}_4(\mathbb C)$, and the exceptional algebra $\mathfrak g_2$. Here $B_2=C_2$ denotes the [Isomorphism between so5 and sp4](../../../semisimple-lie-algebra.md#isomorphism-between-so5-and-sp4), not an additional case. The disconnected $A_1\times A_1$ system corresponds to a semisimple but nonsimple algebra and is excluded.

The [Dynkin diagrams](../../../semisimple-lie-algebra.md#dynkin-diagram), with nodes in the same order as the matrices, are

$$
\begin{array}{ccl}
A_2&:&\overset{\alpha_1}{\circ}\! -\!\overset{\alpha_2}{\circ},\\[0.5em]
B_2&:&\overset{\alpha_1}{\circ}\!\Rightarrow\!\overset{\alpha_2}{\circ},\\[0.5em]
G_2&:&\overset{\alpha_1}{\circ}\!\equiv\!>\!\overset{\alpha_2}{\circ}.
\end{array}
$$

The second and third diagrams have two and three bonds respectively, with the arrowhead pointing to the [short root](../../../semisimple-lie-algebra.md#short-root) $\alpha_2$. In the last diagram $\equiv$ draws the three bonds and $>$ their arrowhead.

To enumerate roots, use the standard [root string](../../../semisimple-lie-algebra.md#root-string) theorem: for $\beta\ne\pm\alpha$, the roots $\beta+n\alpha$ are consecutive from $\beta-p\alpha$ through $\beta+q\alpha$, with $p-q=\langle\beta,\alpha^\vee\rangle$. Also use the standard results that the [root system](../../../semisimple-lie-algebra.md#root-system) is reduced, every root is conjugate under the [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) to a simple root, and each [root space](../../../semisimple-lie-algebra.md#root-space) has dimension one.

Write $m=a\in\{1,2,3\}$. Since a difference of simple roots is not a root, the $\alpha_2$-string starting at $\alpha_1$ has $p=0$ and $q=m$. It produces $\alpha_1,\alpha_1+\alpha_2,\ldots,\alpha_1+m\alpha_2$. The $\alpha_1$-string starting at $\alpha_2$ has $q=1$. In type $G_2$, the further string through $\beta=\alpha_1+3\alpha_2$ has

$$
\langle\beta,\alpha_1^\vee\rangle=2-3=-1,
$$

and $\beta-\alpha_1=3\alpha_2$ is not a root, so it also produces $2\alpha_1+3\alpha_2$. The resulting positive roots are

$$
\boxed{\begin{aligned}
\Phi^+(A_2)&=\{\alpha_1,\alpha_2,\alpha_1+\alpha_2\},\\
\Phi^+(B_2)&=\{\alpha_1,\alpha_2,\alpha_1+\alpha_2,\alpha_1+2\alpha_2\},\\
\Phi^+(G_2)&=\{\alpha_1,\alpha_2,\alpha_1+\alpha_2,\alpha_1+2\alpha_2,\alpha_1+3\alpha_2,2\alpha_1+3\alpha_2\}.
\end{aligned}}
$$

All roots are these and their negatives. To check completeness, the simple [root reflections](../../../semisimple-lie-algebra.md#root-reflection) act on coordinates by

$$
s_1(r\alpha_1+s\alpha_2)=(-r+s)\alpha_1+s\alpha_2,\qquad
s_2(r\alpha_1+s\alpha_2)=r\alpha_1+(mr-s)\alpha_2.
$$

Each listed set together with its negatives is stable under both reflections. It contains the simple roots and consists of roots already forced by strings. Since every root lies in a Weyl orbit of a simple root, no other roots can occur. This proves the lists for the [A2 root system](../../../semisimple-lie-algebra.md#a2-root-system), [B2 root system](../../../semisimple-lie-algebra.md#b2-root-system), and [G2 root system](../../../semisimple-lie-algebra.md#g2-root-system). The [root-space decomposition](../../../semisimple-lie-algebra.md#root-space-decomposition) then gives

$$
\boxed{\dim\mathfrak{sl}_3=2+6=8,\qquad\dim\mathfrak{so}_5=2+8=10,\qquad\dim\mathfrak g_2=2+12=14.}
$$

For the restriction to a [sl2 subalgebra associated with a root](../../../semisimple-lie-algebra.md#sl2-subalgebra-associated-with-a-root), normalize its Cartan element to be $h_\alpha=\alpha^\vee$. On a root vector of root $\beta$, its eigenvalue is $\langle\beta,\alpha^\vee\rangle$. The [classification of finite-dimensional sl2 representations](../../../semisimple-lie-algebra.md#classification-of-finite-dimensional-sl2-representations) says that $R(\Lambda)$ has weights $\Lambda,\Lambda-2,\ldots,-\Lambda$ and dimension $\Lambda+1$. A root string of $\Lambda+1$ nonparallel roots therefore supplies one such irreducible module: the raising and lowering brackets connect its consecutive root spaces.

For clarity, the positive-side strings for each simple-root direction are listed below. Brackets denote the whole consecutive string; a single listed root is a string of length one. In every row also include each negative string in reverse order, and separately the triple formed by the root $\alpha_i$, its negative, and $h_{\alpha_i}$.

$$
\begin{array}{c|c|l}
\text{type}&\text{direction}&\text{nonparallel positive-side strings}\\\hline
A_2&\alpha_1&[\alpha_2,\alpha_1+\alpha_2]\\
A_2&\alpha_2&[\alpha_1,\alpha_1+\alpha_2]\\
B_2&\alpha_1&[\alpha_2,\alpha_1+\alpha_2],\quad[\alpha_1+2\alpha_2]\\
B_2&\alpha_2&[\alpha_1,\alpha_1+\alpha_2,\alpha_1+2\alpha_2]\\
G_2&\alpha_1&[\alpha_2,\alpha_1+\alpha_2],\quad[\alpha_1+3\alpha_2,2\alpha_1+3\alpha_2],\quad[\alpha_1+2\alpha_2]\\
G_2&\alpha_2&[\alpha_1,\alpha_1+\alpha_2,\alpha_1+2\alpha_2,\alpha_1+3\alpha_2],\quad[2\alpha_1+3\alpha_2]
\end{array}
$$

The root's own triple is always $R(2)$. The one-dimensional subspace of $\mathfrak h$ annihilated by $\alpha_i$ commutes with this subalgebra and gives $R(0)$. Each singleton root in the table, and its negative, contributes another $R(0)$. Reading the other string lengths now gives the [adjoint branching to root sl2 subalgebras in rank two](../../../lie-algebra.md#adjoint-branching-to-root-sl2-subalgebras-in-rank-two):

$$
\boxed{\begin{array}{c|c|l}
\text{type}&\text{simple root}&\mathfrak g\downarrow_{\mathfrak{sl}_2(\alpha_i)}\\\hline
A_2&\alpha_1\text{ or }\alpha_2&R(2)\oplus2R(1)\oplus R(0)\\
B_2&\alpha_1\text{ (long)}&R(2)\oplus2R(1)\oplus3R(0)\\
B_2&\alpha_2\text{ (short)}&3R(2)\oplus R(0)\\
G_2&\alpha_1\text{ (long)}&R(2)\oplus4R(1)\oplus3R(0)\\
G_2&\alpha_2\text{ (short)}&R(2)\oplus2R(3)\oplus3R(0)
\end{array}}
$$

Their dimensions are respectively $8,10,10,14,14$. The last row agrees with [G2 adjoint branching to a short-root sl2 subalgebra](../../../semisimple-lie-algebra.md#g2-adjoint-branching-to-a-short-root-sl2-subalgebra). All labels in the table are highest weights, rather than dimensions.

## 4

↑ **Parent:** [Paper 302](paper-302.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Use anti-Hermitian representation matrices for the [unitary representation](../../../representation-theory.md#unitary-representation), so $R(X)^\dagger=-R(X)$. Absorb the [gauge coupling](../../../relativistic-quantum-field.md#gauge-coupling) into the connection, consistently with the transformation law in the PDF. The appropriate [gauge covariant derivative](../../../relativistic-quantum-field.md#gauge-covariant-derivative) is

$$
\boxed{D_\mu\phi=\partial_\mu\phi+R(A_\mu)\phi.}
$$

This has a plus sign because the inhomogeneous part of the connection transformation is $-\epsilon\partial_\mu X$. Its variation is

$$
\begin{aligned}
\frac1\epsilon\delta_X(D_\mu\phi)
&=R(\partial_\mu X)\phi+R(X)\partial_\mu\phi
-R(\partial_\mu X)\phi+R([X,A_\mu])\phi+R(A_\mu)R(X)\phi\\
&=R(X)\partial_\mu\phi+[R(X),R(A_\mu)]\phi+R(A_\mu)R(X)\phi\\
&=R(X)D_\mu\phi.
\end{aligned}
$$

Thus [gauge covariance of a scalar covariant derivative](../../../relativistic-quantum-field.md#gauge-covariance-of-a-scalar-covariant-derivative) gives

$$
\boxed{\delta_X(D_\mu\phi)=\epsilon R(X)D_\mu\phi.}
$$

The cancellation uses that $R$ is a [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation), including its commutator identity.

The [gauge field strength](../../../relativistic-quantum-field.md#gauge-field-strength) is

$$
\boxed{F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu+[A_\mu,A_\nu],\qquad\delta_XF_{\mu\nu}=\epsilon[X,F_{\mu\nu}].}
$$

It is the curvature appearing in $[D_\mu,D_\nu]\phi=R(F_{\mu\nu})\phi$. The index positions in the PDF are related by the constant [Minkowski metric](../../../special-relativity.md#minkowski-metric); lowering the index in its transformation law gives the convention used here.

Take signature $(+,-,-,-)$, let $B$ be a real symmetric gauge-invariant internal form, and let $\langle\cdot,\cdot\rangle_V$ be the positive [Hermitian form](../../../linear-algebra.md#hermitian-form) preserved by the unitary matter representation. One consistent [Lorentz transformation](../../../special-relativity.md#lorentz-transformation) scalar [Lagrangian density](../../../quantum-field-theory.md#lagrangian-density) is

$$
\boxed{\mathcal L=-\frac1{4g_{\mathrm{YM}}^2}B(F_{\mu\nu},F^{\mu\nu})+\langle D_\mu\phi,D^\mu\phi\rangle_V-m^2\langle\phi,\phi\rangle_V-\lambda\langle\phi,\phi\rangle_V^2.}
$$

Here $g_{\mathrm{YM}}>0$, $m^2\geq0$, and $\lambda\geq0$ give a simple stable potential. The coupling is in the kinetic normalization because it was absorbed into $A_\mu$; it is not inserted again into $D_\mu$. Taking a zero or another gauge-invariant potential is also possible. A positive nondegenerate $B$ gives the usual physical gauge kinetic energy, as for a compact gauge algebra. More generally the invariance calculation below applies to any symmetric [invariant bilinear form on a Lie algebra](../../../lie-algebra.md#invariant-bilinear-form-on-a-lie-algebra), including the [Killing form](../../../lie-algebra.md#killing-form).

Under the infinitesimal [gauge-field transformation law](../../../relativistic-quantum-field.md#gauge-field-transformation-law),

$$
\delta_X B(F_{\mu\nu},F^{\mu\nu})=\epsilon\{B([X,F_{\mu\nu}],F^{\mu\nu})+B(F_{\mu\nu},[X,F^{\mu\nu}])\}=0.
$$

Invariance and symmetry of $B$ give the cancellation. For matter, both $\phi$ and $D_\mu\phi$ transform by $R(X)$, so anti-Hermiticity gives

$$
\delta_X\langle v,w\rangle_V=\epsilon\langle R(X)v,w\rangle_V+\epsilon\langle v,R(X)w\rangle_V=0
$$

for either pairing used in the Lagrangian. Its potential is a function of the invariant scalar norm. Therefore $\boxed{\delta_X\mathcal L=0}$, establishing [gauge invariance](../../../relativistic-quantum-field.md#gauge-invariance) of this [Yang-Mills theory](../../../relativistic-quantum-field.md#yang-mills-theory) coupled to a scalar. Contraction of spacetime indices with the Minkowski metric gives Lorentz invariance.

For the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra), define the [Lie algebra structure constants](../../../lie-algebra.md#structure-constant-of-a-lie-algebra) by

$$
[T^a,T^b]=f^{ab}{}_{c}T^c,\qquad\kappa^{ab}=\kappa(T^a,T^b).
$$

Internal superscripts here are basis labels, as in the paper; spacetime indices alone are raised with the Minkowski metric. The [adjoint covariant derivative](../../../relativistic-quantum-field.md#adjoint-covariant-derivative) and curvature have components

$$
(D_\mu\phi)^a=\partial_\mu\phi^a+f^{bc}{}_{a}A_\mu^b\phi^c,\qquad
F_{\mu\nu}^a=\partial_\mu A_\nu^a-\partial_\nu A_\mu^a+f^{bc}{}_{a}A_\mu^b A_\nu^c.
$$

These formulas involve no extra factor of $i$, because the generators use the Lie-algebra convention rather than Hermitian physics generators.

To make the Killing-form sign explicit, write $B=s\kappa$ and $\langle\phi,\psi\rangle_V=s\kappa^{ab}(\phi^a)^*\psi^b$. The literal contraction requested in the paper corresponds to $s=1$. For a [compact real form](../../../semisimple-lie-algebra.md#compact-real-form-of-a-complex-semisimple-lie-algebra) of a complex semisimple gauge algebra, its actual positive [inner product](../../../linear-algebra.md#inner-product) has $s=-1$, since the Killing form is negative definite. With a complex adjoint scalar, the fully expanded [Killing-form Lagrangian for an adjoint scalar](../../../relativistic-quantum-field.md#killing-form-lagrangian-for-an-adjoint-scalar) is

$$
\boxed{\begin{aligned}
\mathcal L_s={}&-\frac{s}{4g_{\mathrm{YM}}^2}\kappa^{ab}
(\partial_\mu A_\nu^a-\partial_\nu A_\mu^a+f^{cd}{}_{a}A_\mu^cA_\nu^d)
(\partial^\mu A^{b\nu}-\partial^\nu A^{b\mu}+f^{ef}{}_{b}A^{e\mu}A^{f\nu})\\
&+s\kappa^{ab}(\partial_\mu\phi^a+f^{cd}{}_{a}A_\mu^c\phi^d)^*
(\partial^\mu\phi^b+f^{ef}{}_{b}A^{e\mu}\phi^f)\\
&-s m^2\kappa^{ab}(\phi^a)^*\phi^b
-\lambda\bigl(\kappa^{ab}(\phi^a)^*\phi^b\bigr)^2.
\end{aligned}}
$$

All repeated internal labels are summed; $s^2=1$ explains the absence of $s$ from the quartic term. Invariance is equivalently the component identity $f^{ca}{}_{d}\kappa^{db}+f^{cb}{}_{d}\kappa^{ad}=0$. For a real adjoint scalar, omit complex conjugation and insert $1/2$ in the scalar kinetic and quadratic mass terms; the same invariance proof applies.

The PDF's identification of the Killing form with an inner product thus requires a sign convention. It also requires nondegeneracy if it is to give ordinary kinetic terms: on an Abelian gauge factor the Killing form vanishes, so an additional invariant metric is needed there. These qualifications do not alter the covariance identities or the formal gauge invariance of the displayed Killing-form contractions.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
