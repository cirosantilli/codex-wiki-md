# Paper 1

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper1.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper1.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
    - [iv](#2/b/iv)
      - [Solution](#2/b/iv/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Identify the [Lie algebra](../../../lie-algebra.md) $\mathfrak g$ with the tangent space $T_eG$. For $X\in\mathfrak g$, its [left-invariant vector field](../../../lie-theory.md#left-invariant-vector-field) is $X^L(g)=(dL_g)_eX$. Let $\gamma_X$ be its integral curve with $\gamma_X(0)=e$. Uniqueness of integral curves and left invariance give $\gamma_X(s+t)=\gamma_X(s)\gamma_X(t)$ wherever initially defined. Repetition of a local curve extends it to all real times. Thus $\gamma_X$ is the unique [one-parameter subgroup](../../../lie-theory.md#one-parameter-subgroup) with derivative $X$ at zero, and the [Exponential map of a Lie group](../../../lie-theory.md#exponential-map-of-a-lie-group) is defined by

$$
\boxed{\exp X=\gamma_X(1),\qquad \exp(tX)=\gamma_X(t).}
$$

Smooth dependence of solutions of differential equations on their initial data and parameters makes this map smooth.

The derivative at zero is particularly simple:

$$
(d\exp)_0(X)=\left.\frac d{dt}\right|_{t=0}\exp(tX)=X.
$$

It is the identity linear map from $\mathfrak g$ to $T_eG$. The [inverse function theorem](../../../calculus.md#inverse-function-theorem) therefore proves that the [Exponential map of a Lie group](../../../lie-theory.md#exponential-map-of-a-lie-group) is a [local diffeomorphism](../../../calculus.md#local-diffeomorphism) at zero, producing a [local exponential chart](../../../lie-theory.md#local-exponential-chart). This proves the requested local assertion.

There is a necessary qualification to the other assertion: the image of every [one-parameter subgroup](../../../lie-theory.md#one-parameter-subgroup) lies in the [identity component of a Lie group](../../../lie-theory.md#identity-component-of-a-lie-group) $G^\circ$. The correct statement without a connectedness hypothesis is

$$
\boxed{\exp:(\mathfrak g,+)\to G\text{ is a homomorphism}
\quad\Longleftrightarrow\quad G^\circ\text{ is abelian}.}
$$

Indeed, if $\exp$ is a [group homomorphism](../../../group-theory.md#group-homomorphism), its image is an abelian subgroup. It contains an identity neighborhood by the local result. An open subgroup of a connected [group](../../../group.md) is the entire [group](../../../group.md): every coset is open, so its complement is also open. Thus $\exp(\mathfrak g)=G^\circ$, proving that this component is abelian.

Conversely, if $G^\circ$ is abelian, then $\exp(tX)\exp(tY)$ is a [one-parameter subgroup](../../../lie-theory.md#one-parameter-subgroup): its [group](../../../group.md) law follows by commuting the factors. Its derivative at zero is $X+Y$. Uniqueness gives $\exp(t(X+Y))=\exp(tX)\exp(tY)$ and, at $t=1$, additivity. This proves the [additivity of the Lie exponential map](../../../lie-theory.md#additivity-of-the-lie-exponential-map) criterion. For connected $G$ it is exactly the stated equivalence with an abelian [group](../../../group.md). For disconnected $G$ the unrestricted claim is false: $S_3\times\mathbb R$ is a nonabelian [Lie group](../../../lie-theory.md#lie-group), but its exponential is the homomorphism $x\mapsto(e,x)$. The original PDF does not impose connectedness in that sentence, so that qualification cannot be omitted.

Now suppose $G$ is connected and abelian, of dimension $n$. The exponential is a surjective [group homomorphism](../../../group-theory.md#group-homomorphism), and its kernel $\Lambda$ is discrete by local injectivity at zero. The induced map

$$
\mathbb R^n/\Lambda\longrightarrow G
$$

is a bijective [Lie group homomorphism](../../../lie-theory.md#lie-group-homomorphism) and a local diffeomorphism, hence a [Lie group isomorphism](../../../lie-theory.md#lie-group-isomorphism). To identify the quotient, take linearly independent elements $\lambda_1,\ldots,\lambda_b\in\Lambda$ spanning the real linear span of $\Lambda$, and let $\Lambda_0=\sum_i\mathbb Z\lambda_i$. Every coset of $\Lambda_0$ in $\Lambda$ has a representative in the bounded fundamental parallelepiped of these vectors. A discrete additive subgroup has finite intersection with a compact set: otherwise differences of arbitrarily close elements would approach zero, contradicting discreteness at zero. Thus $\Lambda/\Lambda_0$ is finite.

It follows that $\Lambda$ is a finitely generated torsion-free abelian [group](../../../group.md) of rank $b$, hence has a $\mathbb Z$-basis of $b$ elements. These basis elements also span its $b$-dimensional real span and are linearly independent over $\mathbb R$. Extending them to a real basis identifies $\Lambda$ with $\mathbb Z^b\times\{0\}^{n-b}$. Consequently the [classification of connected abelian Lie groups](../../../lie-theory.md#classification-of-connected-abelian-lie-groups) is

$$
\boxed{G\cong\mathbb R^{n-b}\times(\mathbb R/\mathbb Z)^b
=\mathbb R^a\times T^b,\qquad a+b=n.}
$$

The compact circle factors record the periods of the [one-parameter subgroups](../../../lie-theory.md#one-parameter-subgroup).

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [Lie algebra](../../../lie-algebra.md) of [SL2R](../../../group-theory.md#real-special-linear-group-of-degree-two) is the space of traceless real two-by-two [matrices](../../../vector-space.md#matrix). For $A$ in this space, the [Cayley-Hamilton theorem](../../../mathematics.md#cayley-hamilton-theorem) gives $A^2=cI$, where $c=-\det A$. Expanding the [matrix exponential](../../../linear-operator-theory.md#matrix-exponential), if $c=s^2>0$ then

$$
\exp A=(\cosh s)I+\frac{\sinh s}{s}A,
\qquad \operatorname{tr}(\exp A)=2\cosh s\geq2.
$$

If $c=0$, then $\exp A=I+A$ and its [trace](../../../linear-algebra.md#matrix-trace) is $2$. If $c=-s^2<0$, then

$$
\exp A=(\cos s)I+\frac{\sin s}{s}A,
\qquad \operatorname{tr}(\exp A)=2\cos s\in[-2,2].
$$

In every case $\operatorname{tr}(\exp A)\geq-2$. But

$$
g=\begin{pmatrix}-2&0\\0&-1/2\end{pmatrix}
$$

has determinant one and [trace](../../../linear-algebra.md#matrix-trace) $-5/2$. Thus $g\in SL_2(\mathbb R)$ is not an exponential, and **the exponential map is not surjective**.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Let $E_{12}=\begin{pmatrix}0&1\\0&0\end{pmatrix}$, so $A(t)=I+tE_{12}$ and $E_{12}^2=0$. Multiplication gives

$$
\begin{pmatrix}m&0\\0&m^{-1}\end{pmatrix}
A(t)
\begin{pmatrix}m^{-1}&0\\0&m\end{pmatrix}
=\begin{pmatrix}1&m^2t\\0&1\end{pmatrix}.
$$

The nilpotence also gives $(I+tE_{12})^k=I+ktE_{12}$ for every nonnegative integer $k$, since all higher binomial terms vanish. Hence, for each positive integer $m$,

$$
\boxed{\operatorname{diag}(m,m^{-1})A(t)\operatorname{diag}(m,m^{-1})^{-1}
=A(m^2t)=A(t)^{m^2}.}
$$

These are [unipotent matrices](../../../lie-theory.md#unipotent-matrix) in [SL2R](../../../group-theory.md#real-special-linear-group-of-degree-two). The integer is positive, since the displayed diagonal [matrix](../../../vector-space.md#matrix) is undefined at $m=0$.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Put $U=\phi(A(t))$. Applying the [group homomorphism](../../../group-theory.md#group-homomorphism) $\phi$ to the identity just proved shows that $U$ is conjugate to $U^{m^2}$ for every positive integer $m$. Thus the multiset of its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) is unchanged by taking their $m^2$th powers.

Take $m=2$. The fourth-power operation permutes this finite multiset. For each [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $z$, iterating its permutation cycle gives $z^{4^r}=z$ for some positive integer $r$. Since $U$ is unitary, $z\ne0$, so $z^{4^r-1}=1$: every [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is a [root of unity](../../../algebra.md#root-of-unity). Choose a positive integer $d$ divisible by all their orders. Every [eigenvalue](../../../linear-operator-theory.md#eigenvalue) of $U^{d^2}$ is then one. Because its [eigenvalue](../../../linear-operator-theory.md#eigenvalue) multiset is also the original one, we obtain

$$
\boxed{\text{every eigenvalue of }\phi(A(t))\text{ equals }1.}
$$

This is [square-power rigidity of a finite nonzero spectrum](../../../algebra.md#square-power-rigidity-of-a-finite-nonzero-spectrum). Finiteness of the dimension is essential to the permutation-cycle argument.

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

Let $N$ be the [normal closure](../../../group-theory.md#normal-closure) of the upper unipotents $U(t)=A(t)$. Conjugation by $J=\begin{pmatrix}0&-1\\1&0\end{pmatrix}$ gives

$$
JU(t)J^{-1}=\begin{pmatrix}1&0\\-t&1\end{pmatrix}.
$$

Thus $N$ also contains every lower unipotent $L(s)=\begin{pmatrix}1&0\\s&1\end{pmatrix}$. We prove explicitly that these [elementary unipotent generators of SL2R](../../../group-theory.md#elementary-unipotent-generators-of-sl2r) generate the full [group](../../../group.md).

For $a\ne0$, multiplication gives

$$
w(a)=U(a)L(-a^{-1})U(a)
=\begin{pmatrix}0&a\\-a^{-1}&0\end{pmatrix},
\qquad
w(a)w(-1)=\begin{pmatrix}a&0\\0&a^{-1}\end{pmatrix}.
$$

So all determinant-one diagonal [matrices](../../../vector-space.md#matrix) lie in $N$. If $g=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ has $a\ne0$ and $ad-bc=1$, then

$$
g=L(c/a)\begin{pmatrix}a&0\\0&a^{-1}\end{pmatrix}U(b/a),
$$

because its lower-right entry is $(1+bc)/a=d$. If $a=0$, then $c\ne0$ and left multiplication by $U(1)$ makes the upper-left entry equal to $c$. The resulting [matrix](../../../vector-space.md#matrix) lies in $N$ by the preceding factorization, and $U(1)^{-1}\in N$ restores $g$. Therefore

$$
\boxed{N=SL_2(\mathbb R).}
$$

<h4 id="2/b/iv">iv</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/b/iv)

Every [unitary matrix](../../../linear-operator-theory.md#unitary-matrix) is unitarily diagonalizable. Part (ii) therefore proves the stronger [matrix](../../../vector-space.md#matrix) statement $\phi(A(t))=I$, not merely a statement about its [eigenvalues](../../../linear-operator-theory.md#eigenvalue). The [kernel of a group homomorphism](../../../group-theory.md#kernel-of-a-group-homomorphism) is a [normal subgroup](../../../group-theory.md#normal-subgroup), and it contains every upper unipotent. By part (iii) their [normal closure](../../../group-theory.md#normal-closure) is the entire [group](../../../group.md). Thus

$$
\boxed{\phi(g)=I\quad\text{for every }g\in SL_2(\mathbb R).}
$$

This proves the [triviality of finite-dimensional unitary representations of SL2R](../../../representation-theory.md#triviality-of-finite-dimensional-unitary-representations-of-sl2r). In fact the argument used only the algebraic homomorphism property and finite-dimensional unitarity; it did not need continuity.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For a [compact Lie group](../../../lie-theory.md#compact-lie-group) $G$, the complex [representation ring of a compact group](../../../representation-theory.md#representation-ring-of-a-compact-group) $R(G)$ is the [Grothendieck group](../../../algebraic-topology.md#grothendieck-group) of finite-dimensional [continuous](../../../calculus.md#continuous-function) complex [group representations](../../../representation-theory.md#group-representation), with the relations $[M\oplus N]=[M]+[N]$. Multiplication is $[M][N]=[M\otimes N]$, and the unit is the trivial one-dimensional [representation](../../../representation-theory.md#group-representation). The ring of [class functions](../../../representation-theory.md#class-function) is

$$
c\ell(G)=\{f\in C(G,\mathbb C):f(hgh^{-1})=f(g)
\text{ for all }g,h\in G\},
$$

with pointwise addition and multiplication. The [character](../../../representation-theory.md#character-of-a-representation) of $M$ is $\chi_M(g)=\operatorname{tr}\rho_M(g)$. The [trace](../../../linear-algebra.md#matrix-trace) identities for direct sums and tensor products make

$$
[M]-[N]\longmapsto\chi_M-\chi_N
$$

a well-defined [ring homomorphism](../../../commutative-algebra.md#ring-homomorphism) $\chi:R(G)\to c\ell(G)$.

Normalize [Haar measure](../../../measure-theory.md#haar-measure) by $\int_Gdg=1$. Averaging a positive definite [Hermitian inner product](../../../linear-algebra.md#hermitian-form) gives

$$
(v,w)_G=\int_G(\rho(g)v,\rho(g)w)_0\,dg,
$$

which is positive definite and $G$-invariant. This proves [unitarization of a compact-group representation](../../../representation-theory.md#unitarization-of-a-compact-group-representation). In a [unitary representation](../../../representation-theory.md#unitary-representation) the [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) of an [invariant subspace](../../../representation-theory.md#invariant-subspace) is invariant. Induction on dimension therefore gives [complete reducibility of compact-group representations](../../../representation-theory.md#complete-reducibility-of-compact-group-representations). Hence every element of $R(G)$ is a finite integral linear combination of irreducible classes.

We establish the needed [character orthogonality for compact groups](../../../representation-theory.md#character-orthogonality-for-compact-groups) carefully. For irreducible unitary [representations](../../../representation-theory.md#group-representation) $V,W$, let $G$ act on $\operatorname{Hom}_{\mathbb C}(W,V)$ by

$$
g\cdot A=\rho_V(g)A\rho_W(g)^{-1}.
$$

Its average $P=\int_G(g\cdot)\,dg$ is a projection onto $\operatorname{Hom}_G(W,V)$: averaging makes every image invariant, and it fixes every intertwiner. The [trace](../../../linear-algebra.md#matrix-trace) of this action is $\chi_V(g)\overline{\chi_W(g)}$, since the inverse of a unitary [matrix](../../../vector-space.md#matrix) has conjugate [trace](../../../linear-algebra.md#matrix-trace). Taking the [trace](../../../linear-algebra.md#matrix-trace) of the projection gives

$$
\int_G\chi_V(g)\overline{\chi_W(g)}\,dg
=\dim\operatorname{Hom}_G(W,V).
$$

For completeness, [Schur's lemma](../../../representation-theory.md#schur-s-lemma) follows here from invariance of the kernel and image of an intertwiner. A nonzero intertwiner between irreducibles is an isomorphism. An endomorphism of an irreducible complex [representation](../../../representation-theory.md#group-representation) has an [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\lambda$; the noninvertible intertwiner $A-\lambda I$ must vanish. Thus the last dimension is one for isomorphic irreducibles and zero for inequivalent ones.

If a virtual [character](../../../representation-theory.md#character-of-a-representation) $\sum_Vn_V\chi_V$ vanishes, integrating it against $\overline{\chi_W}$ gives $n_W=0$ for every irreducible $W$. The irreducible multiplicities therefore distinguish the classes, and

$$
\boxed{\chi:R(G)\longrightarrow c\ell(G)\text{ is injective}.}
$$

This also proves that two finite-dimensional [representations](../../../representation-theory.md#group-representation) with the same [character](../../../representation-theory.md#character-of-a-representation) are isomorphic.

For [SU(2)](../../../topological-group.md#su-2-group), the irreducibles are $V_k=\operatorname{Sym}^k(\mathbb C^2)$, $k\geq0$, of dimension $k+1$. One can see this classification through the usual $\mathfrak{sl}_2$ operators $H,E,F$: a [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector) $v$ has $Hv=kv$, $Ev=0$, and the relations $[H,E]=2E$, $[H,F]=-2F$, $[E,F]=H$ give, by induction,

$$
EF^jv=j(k-j+1)F^{j-1}v.
$$

The torus weights are integers. If $F^rv\ne0$ but $F^{r+1}v=0$, the identity at $j=r+1$ forces $k=r\geq0$. The vectors $v,Fv,\ldots,F^kv$ span an invariant irreducible module, which in an irreducible [representation](../../../representation-theory.md#group-representation) is the whole space. This is the symmetric-power module. Conversely its successive monomial weight vectors are linked by $E,F$ with nonzero coefficients, proving its irreducibility. Thus the [classification of finite-dimensional representations of SU2](../../../representation-theory.md#classification-of-finite-dimensional-representations-of-su2) gives every irreducible, rather than just a list of examples.

On the [maximal torus](../../../lie-theory.md#maximal-torus) $T=\{\operatorname{diag}(z,z^{-1}):|z|=1\}$, their [characters](../../../representation-theory.md#character-of-a-representation) are

$$
\chi_k(z)=z^k+z^{k-2}+\cdots+z^{-k}.
$$

With $x=\chi_1=z+z^{-1}$, multiplication gives $\chi_{k+1}=x\chi_k-\chi_{k-1}$, starting with $\chi_0=1$. Hence each $\chi_k$ is a monic integral polynomial of degree $k$ in $x$. For example $\chi_2=x^2-1$ and $\chi_3=x^3-2x$. They form a basis over $\mathbb Z$, so

$$
\boxed{R(SU(2))\cong\mathbb Z[x],\qquad x=[\mathbb C^2].}
$$

The [character](../../../representation-theory.md#character-of-a-representation) map realizes this ring as the finite integral polynomials in $z+z^{-1}$, interpreted as [continuous](../../../calculus.md#continuous-function) [class functions](../../../representation-theory.md#class-function). Its image is not the whole infinite-dimensional ring of [continuous](../../../calculus.md#continuous-function) [class functions](../../../representation-theory.md#class-function); injectivity is the assertion being proved.

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

We prove uniform approximation, not just approximation in $L^2$. The analytic facts used are: a [continuous](../../../calculus.md#continuous-function) square-integrable kernel gives a compact integral operator on $L^2$; the [spectral theorem for compact self-adjoint operators](../../../compact-operator.md#spectral-theorem-for-compact-hermitian-operators) decomposes the closure of its range into its finite-dimensional nonzero [eigenspaces](../../../linear-operator-theory.md#eigenspace); and [continuous](../../../calculus.md#continuous-function) functions are dense in $L^2$ for normalized [Haar measure](../../../measure-theory.md#haar-measure) on a [compact Lie group](../../../lie-theory.md#compact-lie-group). Normalized [Haar measure](../../../measure-theory.md#haar-measure) on a compact [group](../../../group.md) is both left- and right-invariant and is preserved by inversion.

Choose a [continuous](../../../calculus.md#continuous-function) nonnegative function $k$ of integral one, supported in a sufficiently small symmetric neighborhood of the identity, with $k(g^{-1})=k(g)$. Such functions are obtained from a local bump and its inverted bump followed by normalization. Define the [convolution](../../../fourier-analysis.md#convolution) operator

$$
(Th)(x)=\int_Gh(y)k(y^{-1}x)\,dy.
$$

Its kernel is [continuous](../../../calculus.md#continuous-function) on $G\times G$, so $T$ is compact. The symmetry of $k$ makes it self-adjoint. It commutes with the [left translations](../../../lie-theory.md#left-and-right-translation-on-a-lie-group) $(L_gh)(x)=h(g^{-1}x)$ by a change of variable $y=gz$.

By [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and invariance of [Haar measure](../../../measure-theory.md#haar-measure),

$$
\|Th\|_\infty\leq\|k\|_2\|h\|_2.
$$

The same integral formula and continuity of the kernel show $Th$ is [continuous](../../../calculus.md#continuous-function) for every $h\in L^2(G)$. Moreover, rewriting $y=xz^{-1}$ gives $(Tf)(x)=\int f(xz^{-1})k(z)\,dz$. Uniform continuity on the compact [group](../../../group.md) therefore makes $\|Tf-f\|_\infty$ arbitrarily small when the support of $k$ is small. Also $\|T\|_{\infty\to\infty}\leq1$ because $k\geq0$ and has integral one.

Fix $\varepsilon>0$ and take $k$ so $\|Tf-f\|_\infty<\varepsilon/3$. Then

$$
\|T^2f-f\|_\infty
\leq\|T(Tf-f)\|_\infty+\|Tf-f\|_\infty
<2\varepsilon/3.
$$

Let $P_N$ be the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) onto increasing finite sums of the nonzero [eigenspaces](../../../linear-operator-theory.md#eigenspace) of $T$. Since $Tf$ lies in the closure of the range, the [spectral theorem](../../../hilbert-space.md#spectral-theorem) gives $P_NTf\to Tf$ in $L^2$. Applying the smoothing estimate gives

$$
\|TP_NTf-T^2f\|_\infty
\leq\|k\|_2\|P_NTf-Tf\|_2\longrightarrow0.
$$

Thus some $h=TP_NTf$ satisfies $\|h-f\|_\infty<\varepsilon$.

Each nonzero [eigenspace](../../../linear-operator-theory.md#eigenspace) is finite dimensional, invariant under $L_g$, and consists of [continuous](../../../calculus.md#continuous-function) functions: if $Tv=\lambda v$ with $\lambda\ne0$, then $v=Tv/\lambda$. The finite sum $M$ containing $h$ therefore carries the finite-dimensional [unitary representation](../../../representation-theory.md#unitary-representation) $\rho(g)=L_g|_M$. It is [continuous](../../../calculus.md#continuous-function), since translating each of its finitely many [continuous](../../../calculus.md#continuous-function) basis functions depends continuously on $g$ in the uniform and hence the $L^2$ norm.

Let $\ell$ be evaluation at the identity on $M$, and let the [dual representation](../../../representation-theory.md#dual-representation) on $M^*$ be $\theta(g)\ell=\ell\circ\rho(g^{-1})$. For the linear functional $L_h$ on $M^*$ defined by $L_h(u)=u(h)$,

$$
L_h(\theta(g)\ell)=\ell(\rho(g^{-1})h)=h(g).
$$

The rank-one endomorphism $\alpha=\ell\otimes L_h$ of $M^*$ satisfies $\operatorname{tr}(\alpha\theta(g))=L_h(\theta(g)\ell)$. Therefore

$$
\boxed{\|f-\operatorname{tr}(\alpha\theta(\,\cdot\,))\|_\infty<\varepsilon.}
$$

This is the requested [Peter-Weyl theorem](../../../representation-theory.md#peter-weyl-theorem), proved via the [convolution proof of uniform Peter-Weyl approximation](../../../representation-theory.md#convolution-proof-of-uniform-peter-weyl-approximation). The extra convolution after the spectral truncation is what upgrades the $L^2$ estimate to a uniform one.

To deduce a faithful finite-dimensional [representation](../../../representation-theory.md#group-representation), first note that these [representations](../../../representation-theory.md#group-representation) separate points. For $g\ne e$, choose a [continuous](../../../calculus.md#continuous-function) function taking different values at $g$ and $e$, and approximate it closely enough by a [trace](../../../linear-algebra.md#matrix-trace) coefficient to retain that difference. The [representation](../../../representation-theory.md#group-representation) appearing in that [trace](../../../linear-algebra.md#matrix-trace) must satisfy $\theta(g)\ne I$.

There is an identity neighborhood $U$ containing no nontrivial subgroup. Here is the [Lie groups have no small subgroups](../../../lie-theory.md#lie-groups-have-no-small-subgroups) argument: choose an injective exponential chart on a Lie-algebra ball of radius $r$, and take $U=\exp(B_\delta)$ with $0<\delta<r/2$. If a subgroup contained a nonidentity $\exp X$ in $U$, choose the first integer $m$ with $m\|X\|\geq\delta$. Then $\delta\leq m\|X\|<2\delta<r$, so its power $\exp(mX)$ lies outside $U$, a contradiction. For a zero-dimensional [group](../../../group.md), take $U=\{e\}$.

For every $g\notin U$, choose a [representation](../../../representation-theory.md#group-representation) nontrivial at $g$. The sets on which these [representations](../../../representation-theory.md#group-representation) are not the identity are open and cover the compact set $G\setminus U$. A finite subcover gives finitely many [representations](../../../representation-theory.md#group-representation), whose [direct sum](../../../vector-space.md#direct-sum) has kernel contained in $U$. A subgroup contained in $U$ is trivial, so this [direct sum](../../../vector-space.md#direct-sum) is faithful. Averaging its Hermitian form makes it unitary. Thus the [finite faithful representation from point-separating representations](../../../representation-theory.md#finite-faithful-representation-from-point-separating-representations) yields

$$
\boxed{G\hookrightarrow U_n\text{ for some finite }n.}
$$

Using the no-small-subgroups neighborhood is essential; $G\setminus\{e\}$ alone need not be compact, so a finite-subcover argument on that punctured set would not be valid.

## 5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

A [maximal torus](../../../lie-theory.md#maximal-torus) in a compact connected [Lie group](../../../lie-theory.md#lie-group) is a compact connected abelian Lie subgroup maximal among such subgroups. By the connected abelian classification it is isomorphic to a product of circles. Such subgroups exist: choose one of largest dimension among compact connected abelian subgroups; a proper inclusion of connected Lie subgroups would increase dimension. Write $\mathfrak t$ for its [Lie algebra](../../../lie-algebra.md).

Here are the main steps of the conjugacy assertion, with the critical arguments supplied. Average an inner product on $\mathfrak g$ over the adjoint action to obtain an $\operatorname{Ad}(G)$-invariant positive definite inner product. It defines a [bi-invariant Riemannian metric](../../../lie-theory.md#bi-invariant-riemannian-metric). Compactness makes this metric complete, and the [Hopf-Rinow theorem](../../../riemannian-geometry.md#hopf-rinow-theorem) joins the identity to any $g$ by a geodesic. For a bi-invariant metric the Levi-Civita connection on left-invariant fields is $\nabla_XY=[X,Y]/2$, so the geodesic starting with $X$ is $\exp(tX)$. Consequently every $g$ has the form $\exp X$.

The Lie-algebra centralizer of $\mathfrak t$ is exactly $\mathfrak t$. If $X$ commutes with $\mathfrak t$, its [one-parameter subgroup](../../../lie-theory.md#one-parameter-subgroup) commutes with $T$. The closure of the subgroup generated by $T$ and $\exp(\mathbb RX)$ is compact, connected and abelian, so it is a torus; maximality forces it to equal $T$, giving $X\in\mathfrak t$. The torus action on $\mathfrak g_\mathbb C$ decomposes into finitely many [character](../../../representation-theory.md#character-of-a-representation) [weight spaces](../../../semisimple-lie-algebra.md#weight-space). The zero-[weight space](../../../semisimple-lie-algebra.md#weight-space) is $\mathfrak t_\mathbb C$. Choose $H\in\mathfrak t$ outside the finitely many kernels of the nonzero weight differentials. Then the centralizer of $H$ is exactly $\mathfrak t$.

For an arbitrary $X\in\mathfrak g$, the [continuous](../../../calculus.md#continuous-function) function $g\mapsto\langle\operatorname{Ad}_gX,H\rangle$ attains a maximum. Put $Y=\operatorname{Ad}_{g_0}X$ at a maximizer. Differentiating along $\exp(sZ)g_0$ gives

$$
0=\langle[Z,Y],H\rangle=\langle Z,[Y,H]\rangle
\quad\text{for every }Z\in\mathfrak g.
$$

Hence $[Y,H]=0$, so $Y\in\mathfrak t$. Exponentiating gives $g_0(\exp X)g_0^{-1}=\exp Y\in T$. This [adjoint-orbit criterion for maximal-torus conjugacy](../../../lie-theory.md#adjoint-orbit-criterion-for-maximal-torus-conjugacy) proves

$$
\boxed{\text{every element of }G\text{ belongs to a subgroup conjugate to }T.}
$$

Restriction of [representations](../../../representation-theory.md#group-representation) is a [ring homomorphism](../../../commutative-algebra.md#ring-homomorphism) $\operatorname{Res}:R(G)\to R(T)$. If a virtual [representation](../../../representation-theory.md#group-representation) restricts to zero, its [character](../../../representation-theory.md#character-of-a-representation) vanishes on $T$. Since [characters](../../../representation-theory.md#character-of-a-representation) are [class functions](../../../representation-theory.md#class-function) and every element is conjugate into $T$, it vanishes on all of $G$. The injectivity of the [character](../../../representation-theory.md#character-of-a-representation) map proved in Question 3 then gives

$$
\boxed{\operatorname{Res}:R(G)\longrightarrow R(T)\text{ is injective}.}
$$

The [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) is $W=N_G(T)/T$. For $n\in N_G(T)$, the operator $\rho(n)$ intertwines the restriction of $\rho$ with its twist by $t\mapsto ntn^{-1}$. Therefore every restricted [representation](../../../representation-theory.md#group-representation), and every virtual difference of them, is fixed by $W$:

$$
\boxed{\operatorname{Res}(R(G))\subseteq R(T)^W.}
$$

For the [special orthogonal group](../../../linear-algebra.md#special-orthogonal-group) $G=SO(2m+1)$, take

$$
T=\{\operatorname{diag}(R_{\theta_1},\ldots,R_{\theta_m},1)\},
$$

where $R_\theta$ is a real planar rotation. It is a [maximal torus](../../../lie-theory.md#maximal-torus): its Lie-algebra centralizer consists of the independent infinitesimal rotations in those planes. Its [character](../../../representation-theory.md#character-of-a-representation) lattice is $\mathbb Z^m$, so, writing $z_i=e^{i\theta_i}$,

$$
R(T)=\mathbb Z[z_1^{\pm1},\ldots,z_m^{\pm1}].
$$

Indeed commuting unitary torus [matrices](../../../vector-space.md#matrix) diagonalize simultaneously into one-dimensional [characters](../../../representation-theory.md#character-of-a-representation), and the [characters](../../../representation-theory.md#character-of-a-representation) of the circle are exactly the integral powers.

The normalizer permutes the real rotation planes and can reverse each angle independently. Permutations of whole two-dimensional blocks have determinant one. A reflection in one rotation plane reverses its angle and has determinant minus one; combining it with reflection of the remaining fixed line gives an element of $SO(2m+1)$. Thus all independent inversions occur. Conversely a normalizer must permute the distinct nontrivial torus [character](../../../representation-theory.md#character-of-a-representation) pairs $\{\pm e_i\}$ and preserve the fixed line, so there are no additional actions. The kernel of this action is exactly $T$, giving

$$
\boxed{W\cong(\mathbb Z/2)^m\rtimes S_m,\qquad
z_i\mapsto z_{\sigma(i)}^{\pm1}.}
$$

It follows that the restriction identifies $R(SO(2m+1))$ with a subring of the signed-permutation-invariant [Laurent polynomials](../../../polynomial.md#laurent-polynomial). In this case we can prove equality. Invariance under individual inversions first gives

$$
\mathbb Z[z_1^{\pm1},\ldots,z_m^{\pm1}]^{(\mathbb Z/2)^m}
=\mathbb Z[x_1,\ldots,x_m],\qquad x_i=z_i+z_i^{-1}.
$$

For one variable, every invariant is an integral combination of $1$ and $z^k+z^{-k}$, and these satisfy the recurrence $s_{k+1}=x s_k-s_{k-1}$. Applying this one coordinate at a time proves the assertion over the other Laurent coefficient rings. Permutation invariance and the [Fundamental theorem of symmetric polynomials](../../../polynomial.md#fundamental-theorem-of-symmetric-polynomials) then give

$$
R(T)^W=\mathbb Z[e_1(x),\ldots,e_m(x)],
$$

where $e_k$ are the [elementary symmetric polynomials](../../../polynomial.md#elementary-symmetric-polynomial).

Let $V$ be the complexification of the defining $(2m+1)$-dimensional real [representation](../../../representation-theory.md#group-representation). Its torus weights are $1,z_i,z_i^{-1}$. The [characters](../../../representation-theory.md#character-of-a-representation) of its exterior powers obey

$$
\sum_{k=0}^{2m+1}\chi_{\Lambda^kV}t^k
=(1+t)\prod_{i=1}^m(1+z_it)(1+z_i^{-1}t)
=(1+t)\prod_{i=1}^m(1+x_it+t^2).
$$

For $k\leq m$, choosing $j$ linear terms and $r$ quadratic terms shows that the coefficient $c_k=\chi_{\Lambda^kV}$ is

$$
c_k=
\sum_{j+2r=k}\binom{m-j}{r}e_j+
\sum_{j+2r=k-1}\binom{m-j}{r}e_j,\qquad e_0=1.
$$

Its leading term is $e_k$ with coefficient one; all other terms use $e_j$ with $j<k$. By induction $e_k$ lies in the restriction image, because $c_k$ is the [character](../../../representation-theory.md#character-of-a-representation) of a genuine [representation](../../../representation-theory.md#group-representation) and all smaller $e_j$ already lie in the image. Hence every invariant polynomial lies there, proving the [representation ring of an odd-dimensional special orthogonal group](../../../representation-theory.md#representation-ring-of-an-odd-dimensional-special-orthogonal-group) description

$$
\boxed{R(SO(2m+1))\cong R(T)^W
=\mathbb Z[e_1,\ldots,e_m]
=\mathbb Z[c_1,\ldots,c_m].}
$$

The triangular change of generators is integral, so $[\Lambda^1V],\ldots,[\Lambda^mV]$ are algebraically independent polynomial generators. For $m=1$, $c_1=1+z+z^{-1}$ and this reduces to $R(SO(3))=\mathbb Z[V_3]$, with the three-dimensional defining [representation](../../../representation-theory.md#group-representation) as generator. These are genuine [representations](../../../representation-theory.md#group-representation) of the orthogonal [group](../../../group.md), not the half-integral spin weights of its simply connected double cover.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
