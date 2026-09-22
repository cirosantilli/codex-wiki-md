# Paper 138

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_138.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_138.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
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
    - [Solution](#4/a/solution)
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
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [i](#5/c/i)
      - [Solution](#5/c/i/solution)
    - [ii](#5/c/ii)
      - [Solution](#5/c/ii/solution)
    - [iii](#5/c/iii)
      - [Solution](#5/c/iii/solution)
    - [iv](#5/c/iv)
      - [Solution](#5/c/iv/solution)
- [6](#6)
  - [a](#6/a)
    - [i](#6/a/i)
      - [Solution](#6/a/i/solution)
    - [ii](#6/a/ii)
      - [Solution](#6/a/ii/solution)
    - [iii](#6/a/iii)
      - [Solution](#6/a/iii/solution)
    - [iv](#6/a/iv)
      - [Solution](#6/a/iv/solution)
    - [v](#6/a/v)
      - [Solution](#6/a/v/solution)
  - [b](#6/b)
    - [i](#6/b/i)
      - [Solution](#6/b/i/solution)
    - [ii](#6/b/ii)
      - [Solution](#6/b/ii/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)

## 1

↑ **Parent:** [Paper 138](paper-138.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

An $A$-module is a [semisimple module](../../../module-theory.md#semisimple-module) when it is a direct sum of [simple modules](../../../module-theory.md#irreducible-module), equivalently when every submodule has a complementary submodule. The finite-dimensional algebra $A$ is a [semisimple algebra](../../../associative-algebra.md#semisimple-algebra) when its left regular module ${}_AA$ is semisimple.

Let $C_{p^n}=\langle g\rangle$, put $N=p^n$, and suppose $\operatorname{char}k=p$. The [freshman's dream](../../../combinatorics.md#freshman-s-dream) gives

$$
g^N-1=(g-1)^N,
$$

so, with $u=g-1$,

$$
kC_{p^n}\cong k[u]/(u^N).
$$

The [indecomposable modules of a cyclic p-group in characteristic p](../../../representation-theory.md#indecomposable-modules-of-a-cyclic-p-group-in-characteristic-p) are precisely

$$
\boxed{M_r=k[u]/(u^r),\qquad1\leq r\leq N.}
$$

Indeed, a module is a vector space with a nilpotent operator $u$, and its decomposition into [Nilpotent Jordan blocks](../../../linear-operator-theory.md#nilpotent-jordan-block) gives these modules. Each $M_r$ is a [uniserial module](../../../module-theory.md#uniserial-module), with unique chain

$$
M_r\supset uM_r\supset\cdots\supset u^{r-1}M_r\supset0.
$$

Therefore

$$
\boxed{J(M_r)=uM_r,\qquad\operatorname{Soc}(M_r)=u^{r-1}M_r.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For a finite-dimensional module over $A$, the [radical of a module](../../../module-theory.md#radical-of-a-module) satisfies $J(M)=J(A)M$. Hence

$$
J(U\oplus V)=J(A)(U\oplus V)=J(U)\oplus J(V),
$$

and induction gives $J^r(U\oplus V)=J^r(U)\oplus J^r(V)$ for every $r$. A simple submodule of a direct sum projects into semisimple submodules of each summand, and equivalently

$$
\operatorname{Soc}(M)=\{m:J(A)m=0\}.
$$

Thus the same argument, or induction through the defining quotients, gives

$$
\boxed{\operatorname{Soc}^r(U\oplus V)
=\operatorname{Soc}^r(U)\oplus\operatorname{Soc}^r(V).}
$$

This is [radical and socle series of a direct sum](../../../module-theory.md#radical-and-socle-series-of-a-direct-sum).

Now let $G$ be a finite $p$-group and let $k$ have characteristic $p$. The [group algebra of a p-group in characteristic p is local](../../../representation-theory.md#group-algebra-of-a-p-group-in-characteristic-p-is-local), with unique simple module $k$. The socle of its regular module is

$$
\operatorname{Soc}(kG)=(kG)^G
=k\sum_{g\in G}g,
$$

which is one-dimensional. If $kG=U\oplus V$ with both summands nonzero, finite length gives nonzero socles for $U$ and $V$, and the direct-sum identity would make $\operatorname{Soc}(kG)$ at least two-dimensional. Therefore

$$
\boxed{{}_{kG}kG\text{ is indecomposable}.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [radical of a module](../../../module-theory.md#radical-of-a-module) is the smallest submodule $N\subseteq M$ for which $M/N$ is a [semisimple module](../../../module-theory.md#semisimple-module). Consequently, if

$$
M=M_0\supseteq M_1\supseteq M_2\supseteq\cdots
$$

has semisimple successive quotients, then $J(M_i)\subseteq M_{i+1}$. Induction gives

$$
J^i(M)\subseteq M_i,
$$

so the [radical series of a module](../../../module-theory.md#radical-series-of-a-module) descends at least as fast as every such series.

Dually, the [socle](../../../module-theory.md#socle-mathematics) is the largest semisimple submodule. If

$$
0=N_0\subseteq N_1\subseteq N_2\subseteq\cdots
$$

has semisimple successive quotients, induction in $M/N_i$ gives

$$
N_i\subseteq\operatorname{Soc}^i(M),
$$

so the [socle series of a module](../../../module-theory.md#socle-series-of-a-module) ascends at least as fast as every such series.

Both series terminate because $M$ has finite [composition length](../../../finite-group-theory.md#composition-length). More precisely,

$$
J^i(M)=J(A)^iM,
\qquad
\operatorname{Soc}^i(M)=\{x\in M:J(A)^ix=0\}.
$$

Thus $J^r(M)=0$ exactly when $J(A)^r$ annihilates all of $M$, which is exactly when $\operatorname{Soc}^r(M)=M$. The two least terminating indices therefore coincide:

$$
\boxed{m=n=\text{the Loewy length of }M.}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/i">i</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/i/solution">Solution</h5>

↑ **Parent:** [I](#1/d/i)

For $1\leq r\leq n$, let $S_r=k$ with a lower triangular matrix $a=(a_{ij})$ acting by the scalar $a_{rr}$. These are pairwise nonisomorphic [simple modules](../../../module-theory.md#irreducible-module), since the diagonal [matrix units](../../../vector-space.md#matrix-unit) $e_{ii}$ distinguish them.

Let $N$ be the ideal of strictly lower triangular matrices. It is nilpotent, and

$$
A/N\cong k^n
$$

is a [semisimple algebra](../../../associative-algebra.md#semisimple-algebra). Hence $N$ is the [Jacobson radical](../../../noncommutative-algebra.md#jacobson-radical); explicitly,

$$
\boxed{J(A)=N=\operatorname{span}_k\{e_{rs}:r>s\}.}
$$

<h4 id="1/d/ii">ii</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/d/ii)

For the left regular module, the [radical series of a module](../../../module-theory.md#radical-series-of-a-module) is obtained by multiplying by powers of the [Jacobson radical](../../../noncommutative-algebra.md#jacobson-radical):

$$
J^i({}_AA)=J(A)^i=N^i.
$$

Products of [matrix units](../../../vector-space.md#matrix-unit) show that

$$
\boxed{N^i=\operatorname{span}_k\{e_{rs}:r-s\geq i\},
\qquad0\leq i\leq n,}
$$

with $N^0=A$ and $N^n=0$. Thus each step removes one subdiagonal, and the [Loewy length](../../../module-theory.md#loewy-length) of ${}_AA$ is $n$.

<h4 id="1/d/iii">iii</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/d/iii)

Order the simple modules as in part (i), so that $S_r$ records the $r$th diagonal character. The quotient $N^i/N^{i+1}$ has basis

$$
e_{i+1,1},e_{i+2,2},\ldots,e_{n,n-i}.
$$

For $a\in A$, multiplication gives

$$
ae_{r,r-i}\equiv a_{rr}e_{r,r-i}\pmod{N^{i+1}},
$$

because every term below row $r$ lies on a lower subdiagonal. Hence the line generated by $e_{r,r-i}$ is $S_r$, and the lines are independent. Therefore the radical layers of the [lower triangular matrix algebra](../../../linear-algebra.md#lower-triangular-matrix-algebra) are

$$
\boxed{J^i(A)/J^{i+1}(A)
\cong S_{i+1}\oplus S_{i+2}\oplus\cdots\oplus S_n.}
$$

## 2

↑ **Parent:** [Paper 138](paper-138.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $g$ be a [p-regular element](../../../representation-theory.md#p-regular-element). Its eigenvalues on $M$ are roots of unity of order prime to $p$. If $\widehat\lambda_1,\ldots,\widehat\lambda_d$ are their [Teichmuller lifts](../../../arithmetic.md#teichmuller-representative) to characteristic-zero roots of unity, the [Brauer character](../../../representation-theory.md#brauer-character) is

$$
\boxed{\chi_M(g)=\sum_{r=1}^d\widehat\lambda_r.}
$$

It depends only on the conjugacy class of $g$, is additive in short exact sequences, and equals the restriction of an ordinary character whenever the representation lifts.

For linear independence, choose a splitting [p-modular system](../../../representation-theory.md#p-modular-system) and let $P_i$ be the [projective cover](../../../module-theory.md#projective-cover) of the simple module $S_i$. A projective lattice lifting $P_i$ has an ordinary character $\Phi_i$ that vanishes on p-singular elements. Reduction and ordinary character orthogonality give

$$
\frac1{|G|}\sum_{g\ p\text{-regular}}
\Phi_i(g^{-1})\chi_{S_j}(g)
=\dim\operatorname{Hom}_{kG}(P_i,S_j)
=\delta_{ij},
$$

because $S_i$ is the head of $P_i$. Pairing a relation $\sum_jc_j\chi_{S_j}=0$ with every $\Phi_i$ yields $c_i=0$ for every $i$. Hence

$$
\boxed{\{\chi_{S_i}\}\text{ is linearly independent over }\mathbb C.}
$$

This is the linear-independence part of the [Brauer–Nesbitt theorem](../../../representation-theory.md#brauer-nesbitt-theorem).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

There is a natural isomorphism

$$
\operatorname{Hom}_{kG}(P,U)
\cong\operatorname{Hom}_{kG}(P\otimes_kU^*,k),
$$

obtained by evaluating a homomorphism against a covector. Since $P$ is a direct summand of a free module and tensoring a free $kG$-module with $U^*$ using the diagonal action again gives a free module, $P\otimes U^*$ is a [projective module](../../../module-theory.md#projective-module).

Lift this projective module to an $\mathcal O G$-lattice. Projectivity makes the dimension of the homomorphism space equal to the multiplicity of the trivial representation after extending scalars to $K$. The lifted ordinary character vanishes on p-singular elements, while on p-regular elements it is the product

$$
\chi_P(g)\chi_{U^*}(g)=\chi_P(g)\chi_U(g^{-1}).
$$

Ordinary character orthogonality and the substitution $g\mapsto g^{-1}$ therefore give

$$
\boxed{
\dim\operatorname{Hom}_{kG}(P,U)
=\frac1{|G|}\sum_{g\ p\text{-regular}}
\chi_P(g^{-1})\chi_U(g).}
$$

Equivalently, this is the [Brauer character inner product](../../../representation-theory.md#brauer-character-inner-product) between the [projective character](../../../representation-theory.md#projective-character) of $P$ and the Brauer character of $U$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Apply part (b) with $P=P_i$ and $U=S_j$. A homomorphism $P_i\to S_j$ kills $J(P_i)$ and therefore factors through the head $P_i/J(P_i)\cong S_i$. By [Schur lemma](../../../representation-theory.md#schur-s-lemma) over the splitting field,

$$
\dim\operatorname{Hom}_{kG}(P_i,S_j)=\delta_{ij}.
$$

Consequently the two stated bases satisfy the [Duality of simple and projective Brauer characters](../../../representation-theory.md#duality-of-simple-and-projective-brauer-characters):

$$
\boxed{\langle\chi_{P_i},\chi_{S_j}\rangle=\delta_{ij}.}
$$

The form is nondegenerate directly: if $\phi\ne0$, then

$$
\langle\phi,\phi\rangle
=\frac1{|G|}\sum_{g\ p\text{-regular}}|\phi(g)|^2>0.
$$

Equivalently, in coordinates indexed by the p-regular conjugacy classes it is a positive diagonal [Hermitian form](../../../linear-algebra.md#hermitian-form) with weights $1/|C_G(x)|$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Writing the [Brauer character inner product](../../../representation-theory.md#brauer-character-inner-product) as a sum over conjugacy-class representatives gives

$$
\langle\chi_{P_i},\chi_{S_j}\rangle
=\sum_r\frac{
\overline{\chi_{P_i}(x_r)}\chi_{S_j}(x_r)}
{|C_G(x_r)|}.
$$

Thus the duality from part (c) is exactly

$$
\boxed{\overline\Pi D X^T=I.}
$$

All three matrices are square. Reversing the two inverse factors gives $DX^T\overline\Pi=I$, hence

$$
X^T\overline\Pi=D^{-1}.
$$

Taking complex conjugates yields

$$
\boxed{\overline X^{,T}\Pi=D^{-1}
=\operatorname{diag}(|C_G(x_1)|,\ldots,|C_G(x_n)|).}
$$

The $(g,h)$ entry is $\sum_S\overline{\chi_S(g)}\chi_{P_S}(h)$, and $\overline{\chi_S(g)}=\chi_S(g^{-1})$. Therefore [Column orthogonality for Brauer characters](../../../representation-theory.md#column-orthogonality-for-brauer-characters) gives

$$
\boxed{
\sum_S\chi_S(g^{-1})\chi_{P_S}(h)
=\begin{cases}
|C_G(g)|,&g\text{ and }h\text{ are conjugate},\\
0,&\text{otherwise}.
\end{cases}}
$$

## 3

↑ **Parent:** [Paper 138](paper-138.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Give the dual $M^*=\operatorname{Hom}_k(M,k)$ the contragredient action $(g\lambda)(m)=\lambda(g^{-1}m)$. If $\delta_h$ is the functional dual to the basis element $h\in G$, then

$$
g\delta_h=\delta_{gh}.
$$

Thus the map $h\mapsto\delta_h$ extends to a $kG$-isomorphism

$$
\boxed{kG\cong(kG)^*.}
$$

This is also the left-module form of the fact that a [group algebra is a symmetric algebra](../../../representation-theory.md#group-algebra-is-a-symmetric-algebra).

If $P$ is finitely generated and projective, it is a direct summand of $(kG)^r$. Dualizing makes $P^*$ a direct summand of $((kG)^*)^r\cong(kG)^r$, so $P^*$ is projective. The converse follows by dualizing again and using $P\cong P^{**}$.

For any finite-dimensional algebra $A$, the module $A^*$ is injective because

$$
\operatorname{Hom}_A(-,A^*)\cong\operatorname{Hom}_k(-,k)
$$

is exact. Since $kG\cong(kG)^*$, free $kG$-modules are injective, and so are their projective direct summands. Conversely, duality sends injectives to projectives, so every finite-dimensional injective is projective. Hence [projective modules over a finite group algebra are injective](../../../representation-theory.md#projective-modules-over-a-finite-group-algebra-are-injective).

Finally, let $P$ be indecomposable projective. It is also an indecomposable injective. Its nonzero [socle](../../../module-theory.md#socle-mathematics) contains a simple module $S$, and the [injective hull](../../../noncommutative-algebra.md#injective-hull) $E(S)$ is a direct summand of $P$. Indecomposability forces $P=E(S)$. Since $S$ is essential in its injective hull, every simple submodule of $P$ equals $S$. Therefore

$$
\boxed{\operatorname{Soc}(P)\text{ is simple}.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Write $P\cong kGe$ for a [primitive idempotent](../../../commutative-algebra.md#primitive-idempotent) $e$. The coefficient-of-identity form makes $kG$ a [symmetric algebra](../../../representation-theory.md#symmetric-algebra-frobenius-algebra). Associativity of this nondegenerate form identifies the orthogonal complement of $J(kG)e$ in $kGe$ with the elements annihilated by $J(kG)$, namely $\operatorname{Soc}(P)$. It therefore induces a nondegenerate $kG$-invariant pairing between

$$
P/J(P)=kGe/J(kG)e
$$

and $\operatorname{Soc}(P)$. Both are simple by projectivity and part (a), and the symmetric form has identity Nakayama permutation. Consequently the [head and socle of an indecomposable projective group-algebra module](../../../representation-theory.md#head-and-socle-of-an-indecomposable-projective-group-algebra-module) satisfy

$$
\boxed{P/J(P)\cong\operatorname{Soc}(P).}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Decompose the projective module as

$$
P\cong\bigoplus_T P_T^{,m_T},
$$

where $T$ ranges over the simple modules. Since $P_T/J(P_T)\cong T$, the multiplicity of $S$ in the [head of a module](../../../module-theory.md#head-of-a-module) $P/J(P)$ is $m_S$. Part (b) gives $\operatorname{Soc}(P_T)\cong T$, so the multiplicity in $\operatorname{Soc}(P)$ is the same $m_S$.

The [invariant submodule](../../../module-theory.md#invariant-submodule) and [coinvariant module](../../../module-theory.md#coinvariant-module) satisfy

$$
P^G\cong\operatorname{Hom}_{kG}(k,P),
\qquad
(P_G)^*\cong(P^*)^G.
$$

Thus $\dim P^G$ is the multiplicity of the trivial module in $\operatorname{Soc}(P)$, while $\dim P_G=\dim\operatorname{Hom}_{kG}(P,k)$ is its multiplicity in the head. Applying the same argument to the projective module $P^*$ yields

$$
\boxed{\dim P^G=\dim P_G=\dim(P^*)^G=\dim(P^*)_G.}
$$

The dual $P_S^*$ is indecomposable projective. Its head is dual to $\operatorname{Soc}(P_S)\cong S$, hence is $S^*$. Uniqueness of [projective covers](../../../module-theory.md#projective-cover) proves the [dual of a projective cover over a group algebra](../../../representation-theory.md#dual-of-a-projective-cover-over-a-group-algebra):

$$
\boxed{(P_S)^*\cong P_{S^*}.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Put $N_G=\sum_{g\in G}g$. Its image on every module lies in the [invariant submodule](../../../module-theory.md#invariant-submodule), since $hN_G=N_G$. In the regular module,

$$
(kG)^G=kN_G,
$$

and this line is the socle of the projective cover $P_k$ of the trivial module.

Suppose $N_GM\ne0$. Choose $m\in M$ with $N_Gm\ne0$ and consider the homomorphism

$$
f:kG\longrightarrow M,
\qquad x\longmapsto xm.
$$

Its restriction $f|_{P_k}$ is nonzero on $\operatorname{Soc}(P_k)=kN_G$. Because $P_k$ is the [injective hull](../../../noncommutative-algebra.md#injective-hull) of its simple socle, that socle is essential: every nonzero submodule meets it. Hence $\ker(f|_{P_k})=0$. The resulting embedding $P_k\hookrightarrow M$ splits because $P_k$ is injective. Since $M$ is indecomposable, $M\cong P_k$.

Conversely, on $P_k$ the image of $N_G$ is its one-dimensional socle. Thus the [group norm element detects the trivial projective cover](../../../representation-theory.md#group-norm-element-detects-the-trivial-projective-cover):

$$
\boxed{
\dim_k(N_GM)=
\begin{cases}
1,&M\cong P_k,\\
0,&M\not\cong P_k.
\end{cases}}
$$

## 4

↑ **Parent:** [Paper 138](paper-138.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

An $RG$-module $M$ is [relative projective module](../../../representation-theory.md#relative-projective-module) for $H$ when it has the lifting property for every $H$-split epimorphism: whenever the solid arrows form a commutative diagram

$$
\begin{array}{ccc}
&M&\\
{}_{\widetilde f}\swarrow&&\searrow^{f}\\
X&\xrightarrow{\pi}&Y
\end{array}
$$

with $\pi:X\twoheadrightarrow Y$ an $RG$-map possessing an $RH$-linear section, there is an $RG$-map $\widetilde f:M\to X$ such that $\pi\widetilde f=f$. Equivalently, every $H$-split epimorphism onto $M$ has a $G$-linear section, or

$$
M\mid\operatorname{Ind}_H^G\operatorname{Res}_H^G M.
$$

For $\alpha\in\operatorname{End}_{RH}(M)$ define the [relative trace](../../../representation-theory.md#relative-trace)

$$
\operatorname{Tr}_H^G(\alpha)
=\sum_{x\in[G/H]}x\alpha x^{-1}.
$$

The [D. Higman criterion](../../../representation-theory.md#d-higman-criterion) is

$$
\boxed{M\text{ is relatively }H\text{-projective}
\quad\Longleftrightarrow\quad
\operatorname{id}_M\in
\operatorname{Tr}_H^G\operatorname{End}_{RH}(M).}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

Set

$$
\alpha=[G:H]^{-1}\operatorname{id}_M\in\operatorname{End}_{RH}(M).
$$

Every conjugate of $\alpha$ equals $\alpha$, so

$$
\operatorname{Tr}_H^G(\alpha)
=[G:H]\alpha=\operatorname{id}_M.
$$

The [D. Higman criterion](../../../representation-theory.md#d-higman-criterion) therefore gives

$$
\boxed{\text{every }RG\text{-module is relatively }H\text{-projective}.}
$$

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

If $M$ is projective over $RG$, then its restriction is projective over $RH$ because $RG$ is a free right $RH$-module and a free $RG$-module restricts to a free $RH$-module.

Conversely, suppose $\operatorname{Res}_H^GM$ is projective. Then

$$
\operatorname{Ind}_H^G\operatorname{Res}_H^GM
$$

is projective over $RG$. Part (i) says that $M$ is a direct summand of this induced module, so $M$ is projective. Hence [projectivity detected on a subgroup of invertible index](../../../representation-theory.md#projectivity-detected-on-a-subgroup-of-invertible-index) gives

$$
\boxed{M\text{ is }RG\text{-projective}
\quad\Longleftrightarrow\quad
\operatorname{Res}_H^GM\text{ is }RH\text{-projective}.}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let $U\leq\operatorname{SL}_2(p)$ be the Sylow p-subgroup of upper unitriangular matrices. It is cyclic of order $p$, generated by

$$
u=\begin{pmatrix}1&1\\0&1\end{pmatrix}.
$$

Realize $S^r(V_2)$ as the homogeneous polynomials of degree $r$ in $X,Y$, with $u$ acting by $X\mapsto X$ and $Y\mapsto X+Y$. For $0\leq r<p$, the only vectors fixed by $u$ are the multiples of $X^r$: successive comparison of the coefficients of $Y^r,Y^{r-1},\ldots$ proves this. Thus the nilpotent operator $u-1$ has one-dimensional kernel. Its [Jordan normal form](../../../linear-operator-theory.md#jordan-normal-form) therefore has a single block, so

$$
\boxed{\operatorname{Res}_U^G S^r(V_2)\text{ is indecomposable of dimension }r+1.}
$$

This also follows from the [indecomposable modules of a cyclic p-group in characteristic p](../../../representation-theory.md#indecomposable-modules-of-a-cyclic-p-group-in-characteristic-p).

For $r=p-1$, the restriction has dimension $p$ and is the regular $kU$-module, hence is projective. Since $[G:U]$ is prime to $p$, part (b)(ii) makes $S^{p-1}(V_2)$ a simple projective $kG$-module. It is therefore a [defect-zero representation](../../../representation-theory.md#defect-zero-representation) and lifts to an ordinary irreducible representation of the same dimension. Consequently

$$
\boxed{\operatorname{SL}_2(p)\text{ has an ordinary irreducible character of degree }p.}
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Let $P$ be a Sylow p-subgroup. Since $[G:P]$ is invertible in $k$, every $kG$-module is relatively $P$-projective.

Suppose first that $kP$ has only finitely many indecomposable modules $U_1,\ldots,U_t$. For every indecomposable $kG$-module $M$, decompose $\operatorname{Res}_P^GM$ into the $U_i$. Relative projectivity makes $M$ a summand of the corresponding finite direct sum of the $\operatorname{Ind}_P^GU_i$. The [Krull–Schmidt theorem](../../../module-theory.md#krull-schmidt-theorem) leaves only finitely many possible indecomposable summands, so $kG$ has finite representation type.

Conversely, suppose $kG$ has finitely many indecomposables. For an indecomposable $kP$-module $U$, the identity double coset in the [Mackey restriction formula](../../../representation-theory.md#mackey-restriction-formula) shows that $U$ is a direct summand of

$$
\operatorname{Res}_P^G\operatorname{Ind}_P^GU.
$$

Decomposing the induced module into the finitely many $kG$-indecomposables and restricting them shows, again by Krull–Schmidt, that only finitely many $U$ can occur. Thus

$$
\boxed{kG\text{ has finite representation type}
\Longleftrightarrow kP\text{ has finite representation type}.}
$$

If $P$ is cyclic, the [indecomposable modules of a cyclic p-group in characteristic p](../../../representation-theory.md#indecomposable-modules-of-a-cyclic-p-group-in-characteristic-p) form a finite list. If $P$ is noncyclic, its [Frattini quotient](../../../finite-group-theory.md#frattini-quotient) has rank at least two and therefore has a quotient $C_p\times C_p$. Inflation preserves indecomposability and nonisomorphism, while $k(C_p\times C_p)$ has infinitely many indecomposable modules. The [Higman criterion for finite representation type of a group algebra](../../../representation-theory.md#higman-criterion-for-finite-representation-type-of-a-group-algebra) now gives

$$
\boxed{kG\text{ has finite representation type}
\Longleftrightarrow P\text{ is cyclic}.}
$$

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Existence of a minimal subgroup follows because $G$ has only finitely many subgroups and every module is relatively $G$-projective. Suppose an indecomposable module $M$ is relatively projective for both $H$ and $K$. Then $M$ is a summand of $\operatorname{Ind}_H^G U$ and of $\operatorname{Ind}_K^G V$ for suitable modules $U,V$. Applying the [Mackey restriction formula](../../../representation-theory.md#mackey-restriction-formula) and the [Krull–Schmidt theorem](../../../module-theory.md#krull-schmidt-theorem) shows that $M$ is relatively projective for some subgroup

$$
H\cap{}^gK.
$$

If $H$ and $K$ are minimal, this forces $H\subseteq{}^gK$. Reversing their roles gives the reverse containment after conjugacy; since the groups are finite, $H$ and $K$ are conjugate. Thus vertices form a unique conjugacy class.

Let $Q$ be a vertex and let $P$ be a Sylow p-subgroup of $Q$. Since $[Q:P]$ is invertible in $k$, every $kQ$-module is relatively $P$-projective. Transitivity of relative projectivity makes $M$ relatively $P$-projective, so minimality forces $Q=P$. Hence every vertex is a p-group.

For the trivial module $k$, every $kH$-endomorphism is scalar, and its relative trace to $G$ is multiplication by $[G:H]$. The [D. Higman criterion](../../../representation-theory.md#d-higman-criterion) says that $k$ is relatively $H$-projective exactly when $p\nmid[G:H]$. The minimal such subgroups are precisely the Sylow p-subgroups. Therefore the [vertex of an indecomposable module](../../../representation-theory.md#vertex-of-an-indecomposable-module) gives

$$
\boxed{\text{the vertex of }k_G\text{ is a Sylow p-subgroup of }G.}
$$

## 5

↑ **Parent:** [Paper 138](paper-138.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

A block idempotent is a primitive central [idempotent](../../../commutative-algebra.md#idempotent) $e\in R$. The module $M$ lies in the corresponding [block of a group algebra](../../../representation-theory.md#block-of-a-group-algebra) when

$$
eM=M,
$$

equivalently when every other block idempotent annihilates $M$.

If $V$ lies in $e$, then the centrality of $e$ makes both its submodule $U$ and quotient $W$ lie in $e$. Conversely, suppose $eU=U$ and $eW=W$. Then $(1-e)V$ maps to zero in $W$, so $(1-e)V\subseteq U$. But $(1-e)U=0$, and applying the idempotent $1-e$ once more gives

$$
(1-e)V=(1-e)^2V=0.
$$

Thus $eV=V$, proving

$$
\boxed{V\text{ lies in }e\quad\Longleftrightarrow\quad U\text{ and }W\text{ lie in }e.}
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Regard the block algebra $RG e$ as an $R[G\times G]$-module through left and right multiplication,

$$
(g,h)x=gxh^{-1}.
$$

A [defect group of a block](../../../representation-theory.md#defect-group-of-a-block) is a p-subgroup $D\leq G$ for which $\Delta D=\{(d,d):d\in D\}$ is a vertex of an indecomposable summand determining the block; equivalently, $D$ is maximal with

$$
\operatorname{Br}_D(e)\ne0
$$

under the [Brauer morphism](../../../representation-theory.md#brauer-morphism). The uniqueness of vertices up to conjugacy in $G\times G$, together with the diagonal form of these vertices, shows that any two such $D$ are conjugate in $G$. Hence

$$
\boxed{\text{all defect groups of a block form one }G\text{-conjugacy class}.}
$$

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/i">i</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/i/solution">Solution</h5>

↑ **Parent:** [I](#5/c/i)

Only the classes $1,3,7A,7B$ are 2-regular. The trivial module and the natural three-dimensional module are simple; the dual natural module gives the conjugate three-dimensional character. Restricting the ordinary characters to the odd-order classes and using $\alpha+\overline\alpha=-1$ produces the fourth simple character of degree eight. The [Brauer character](../../../representation-theory.md#brauer-character) table is

$$
\boxed{
\begin{array}{c|rrrr}
&1&3&7A&7B\\\hline
\phi_1&1&1&1&1\\
\phi_3&3&0&\alpha&\overline\alpha\\
\phi_{\overline3}&3&0&\overline\alpha&\alpha\\
\phi_8&8&-1&1&1
\end{array}}
$$

The ordinary degree-eight character restricts exactly to $\phi_8$. Since its degree contains the full 2-part $8$ of $|G|$, this simple module is projective and its singleton block has defect zero. Thus

$$
\boxed{\phi_8\text{ lies in the unique defect-zero block};
\quad\phi_1,\phi_3,\phi_{\overline3}\text{ lie in the principal block}.}
$$

<h4 id="5/c/ii">ii</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/c/ii)

On the 2-regular classes the six ordinary characters decompose as

$$
\chi_1=\phi_1,
\quad \chi_{3A}=\phi_3,
\quad \chi_{3B}=\phi_{\overline3},
\quad \chi_6=\phi_3+\phi_{\overline3},
\quad \chi_7=\phi_1+\phi_3+\phi_{\overline3},
\quad \chi_8=\phi_8.
$$

Therefore the [decomposition matrix](../../../representation-theory.md#decomposition-matrix-modular-representation-theory), with columns ordered $1,3,\overline3,8$, is

$$
\boxed{
D=\begin{pmatrix}
1&0&0&0\\
0&1&0&0\\
0&0&1&0\\
0&1&1&0\\
1&1&1&0\\
0&0&0&1
\end{pmatrix}.}
$$

The [Cartan matrix of a group algebra](../../../representation-theory.md#cartan-matrix-of-a-group-algebra) is

$$
\boxed{
C=D^TD=
\begin{pmatrix}
2&1&1&0\\
1&3&2&0\\
1&2&3&0\\
0&0&0&1
\end{pmatrix}.}
$$

<h4 id="5/c/iii">iii</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/c/iii)

The rows of the [Cartan matrix of a group algebra](../../../representation-theory.md#cartan-matrix-of-a-group-algebra) express the [projective characters](../../../representation-theory.md#projective-character) in the simple Brauer-character basis. Thus

$$
\begin{aligned}
\Phi_1&=2\phi_1+\phi_3+\phi_{\overline3},\\
\Phi_3&=\phi_1+3\phi_3+2\phi_{\overline3},\\
\Phi_{\overline3}&=\phi_1+2\phi_3+3\phi_{\overline3},\\
\Phi_8&=\phi_8.
\end{aligned}
$$

Evaluating gives

$$
\boxed{
\begin{array}{c|rrrr}
&1&3&7A&7B\\\hline
\Phi_1&8&2&1&1\\
\Phi_3&16&1&\alpha-1&\overline\alpha-1\\
\Phi_{\overline3}&16&1&\overline\alpha-1&\alpha-1\\
\Phi_8&8&-1&1&1
\end{array}.}
$$

<h4 id="5/c/iv">iv</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#5/c/iv)

The eight-dimensional simple module is projective, so its [tensor product of group representations](../../../representation-theory.md#tensor-product-of-group-representations) with the natural three-dimensional module is projective. Its Brauer character is

$$
\phi_8\phi_3=(24,0,\alpha,\overline\alpha).
$$

From part (iii),

$$
\Phi_3+\Phi_8
=(24,0,\alpha,\overline\alpha).
$$

The duality of simple and projective Brauer characters makes the decomposition multiplicities unique. Hence, writing $P_3$ and $P_8$ for the corresponding projective covers,

$$
\boxed{8\otimes3\cong P_3\oplus P_8.}
$$

This completes the explicit [2-modular representation theory of GL3 of F2](../../../representation-theory.md#2-modular-representation-theory-of-gl3-of-f2) calculation.

## 6

↑ **Parent:** [Paper 138](paper-138.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/i">i</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/i/solution">Solution</h5>

↑ **Parent:** [I](#6/a/i)

The divisibility in (i) is the standard dimension test for a projective modular representation. If $P$ is a projective $kG$-module and $S$ is a Sylow p-subgroup of order $p^d$, then $\operatorname{Res}_S^GP$ is projective over $kS$. The [group algebra of a p-group in characteristic p is local](../../../representation-theory.md#group-algebra-of-a-p-group-in-characteristic-p-is-local), so every finitely generated projective $kS$-module is free. Consequently

$$
\boxed{p^d\mid\dim_kP.}
$$

This will apply to $P=\overline W$ in the implication (v)$\Rightarrow$(i).

<h4 id="6/a/ii">ii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/a/ii)

Assume (ii), and write the ring decomposition as

$$
\mathcal OG\cong\operatorname{End}_{\mathcal O}(W)\times B
\cong M_n(\mathcal O)\times B.
$$

The natural column module $W\cong\mathcal O^n$ is projective over $M_n(\mathcal O)$ by [Morita equivalence](../../../noncommutative-algebra.md#morita-equivalence); extending it by zero across $B$ makes it projective over $\mathcal OG$. After extending scalars to $K$, the action factors through $M_n(K)$ on its natural module $K^n$, which is simple. Therefore

$$
\boxed{\text{(ii)}\Longrightarrow\text{(iii)}.}
$$

<h4 id="6/a/iii">iii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6/a/iii)

Assume (iii). Reduction of the projective lattice $W$ is projective, because a direct-summand decomposition of a free $\mathcal OG$-module remains one after tensoring with $k$. Completeness of $\mathcal O$ and [idempotent lifting](../../../commutative-algebra.md#idempotent-lifting) show that $\overline W$ is indecomposable: otherwise a nontrivial idempotent of $\operatorname{End}_{kG}(\overline W)$ would lift and split $W$, hence split the simple $KG$-module $M$.

Let $\chi$ be the ordinary irreducible character of $M$. Since $W$ is projective, $\chi$ vanishes on p-singular elements and restricts to the [projective character](../../../representation-theory.md#projective-character) $\Phi$ of $\overline W$. Thus

$$
\dim_k\operatorname{End}_{kG}(\overline W)
=\langle\Phi,\Phi\rangle_{p'}
=\langle\chi,\chi\rangle=1.
$$

An indecomposable projective module that is not simple has, besides its identity, a nonzero noninvertible endomorphism obtained by projecting onto its simple head and embedding the isomorphic simple socle. Hence its endomorphism algebra has dimension at least two. Therefore $\overline W$ is simple as well as projective, proving

$$
\boxed{\text{(iii)}\Longrightarrow\text{(v)}.}
$$

<h4 id="6/a/iv">iv</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#6/a/iv)

Under (ii), tensor the direct-product decomposition with the residue field $k$. Since $W$ is free over $\mathcal O$,

$$
k\otimes_{\mathcal O}\operatorname{End}_{\mathcal O}(W)
\cong\operatorname{End}_k(\overline W)\cong M_n(k).
$$

Hence

$$
kG\cong\operatorname{End}_k(\overline W)\times(k\otimes_{\mathcal O}B),
$$

and the reduced action map is the projection onto the first factor. This proves

$$
\boxed{\text{(ii)}\Longrightarrow\text{(iv)}.}
$$

<h4 id="6/a/v">v</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/v/solution">Solution</h5>

↑ **Parent:** [V](#6/a/v)

Assume (v). If the generic fibre $M=K\otimes_{\mathcal O}W$ had a nonzero proper $KG$-submodule, intersecting it with $W$ and rescaling to obtain a saturated lattice would give a nonzero proper $kG$-submodule of $\overline W$. Thus $M$ is simple.

Because $\overline W$ is projective, its restriction to a Sylow p-subgroup $S$ is projective. The local algebra $kS$ has only free finitely generated projectives, so $|S|=p^d$ divides

$$
\dim_k\overline W=\operatorname{rank}_{\mathcal O}W=\dim_KM=n.
$$

Consequently

$$
\boxed{\text{(v)}\Longrightarrow\text{(i)}.}
$$

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/i">i</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/i/solution">Solution</h5>

↑ **Parent:** [I](#6/b/i)

Let $D$ act on the [group algebra](../../../associative-algebra.md#group-algebra) $kG$ by conjugation. Its fixed-point algebra is

$$
(kG)^D=\{a\in kG:dad^{-1}=a\text{ for every }d\in D\},
$$

and the [centralizer](../../../group-theory.md#centralizer) $C_G(D)$ consists of the elements of $G$ commuting with every element of $D$. The [Brauer morphism](../../../representation-theory.md#brauer-morphism) is

$$
\beta=\operatorname{Br}_D:(kG)^D\longrightarrow kC_G(D),
\qquad
\sum_{g\in G}a_gg\longmapsto\sum_{g\in C_G(D)}a_gg.
$$

Thus $\beta$ deletes the coefficients of basis elements outside $C_G(D)$. The nonfixed $D$-orbits have cardinality divisible by $p$, so the usual orbit argument shows that this projection is a unital [ring homomorphism](../../../commutative-algebra.md#ring-homomorphism). Hence

$$
\boxed{\beta=\operatorname{Br}_D:(kG)^D\to kC_G(D).}
$$

<h4 id="6/b/ii">ii</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/b/ii)

Put $N=N_G(D)$. For an algebra on which a group acts by conjugation, write

$$
A_D^H=\operatorname{Tr}_D^H(A^D),
\qquad
\operatorname{Tr}_D^H(a)=\sum_{h\in H/D}hah^{-1},
$$

for its [transfer ideal of conjugation-fixed elements](../../../representation-theory.md#transfer-ideal-of-conjugation-fixed-elements). In the diagram, $\tau=\operatorname{Tr}_D^G$, $\tau'=\operatorname{Tr}_D^N$, the upper map is $\beta=\operatorname{Br}_D$, and $\beta'$ is the restriction of $\operatorname{Br}_D$ from $(kG)^G$ to $(kG)_D^G$. Since $N$ normalizes both $D$ and $C_G(D)$, the lower map lands in $(kC_G(D))_D^N$.

For $a\in(kG)^D$, let $D$ act on the left cosets $G/D$. A coset $gD$ is fixed precisely when $g^{-1}Dg\leq D$, hence, because the two groups have the same order, precisely when $g\in N$. Every nonfixed orbit has size divisible by $p$. Moreover, after applying $\operatorname{Br}_D$, all summands indexed by one $D$-orbit are equal: conjugation by an element of $D$ acts trivially on $kC_G(D)$. Those orbits therefore contribute zero in characteristic $p$, while the fixed cosets contribute the trace over $N/D$. Consequently

$$
\beta'\tau(a)
=\operatorname{Br}_D\!\left(\operatorname{Tr}_D^G(a)\right)
=\operatorname{Tr}_D^N\!\left(\operatorname{Br}_D(a)\right)
=\tau'\beta(a).
$$

This is the [Brauer morphism and relative trace](../../../representation-theory.md#brauer-morphism-and-relative-trace) identity, so **the diagram commutes**.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

The [decomposition matrix](../../../representation-theory.md#decomposition-matrix-modular-representation-theory) separates into two connected components. The first contains $\phi_1,\phi_2$ and $\chi_1,\chi_{3A},\chi_{3B},\chi_4$; it is the principal block $B_0$. The second contains only $\phi_3$ and $\chi_5$; since $\phi_3(1)=5$ contains the full 5-part of $|A_5|=60$, this is a [defect-zero representation](../../../representation-theory.md#defect-zero-representation) and its block $B_1$ has defect group $1$.

For $D=1$, the [normalizer](../../../group-theory.md#normalizer) is $N_G(1)=G$, so the [Brauer correspondence](../../../representation-theory.md#brauer-correspondence) is the identity and $B_1$ corresponds to itself.

The defect group of the principal block is a Sylow 5-subgroup $P\cong C_5$. There are six Sylow 5-subgroups in $A_5$, so the [orbit-stabilizer theorem](../../../group-theory.md#orbit-stabilizer-theorem) gives

$$
|N_{A_5}(P)|=\frac{60}{6}=10.
$$

The [centralizer](../../../group-theory.md#centralizer) of a 5-cycle in $A_5$ is $P$, and an involution in the normalizer acts on $P$ by inversion. Hence

$$
N=N_{A_5}(P)\cong C_5\rtimes C_2\cong D_{10}.
$$

In characteristic five the simple $kN$-modules are inflated from $N/P\cong C_2$: their [Brauer characters](../../../representation-theory.md#brauer-character) are $\psi_+=(1,1)$ and $\psi_-=(1,-1)$ on the identity and involution classes. If $1,\varepsilon,\rho_1,\rho_2$ are the two one-dimensional and two two-dimensional ordinary characters of $D_{10}$, their reductions are

$$
1\mapsto\psi_+,
\qquad
\varepsilon\mapsto\psi_-,
\qquad
\rho_1,\rho_2\mapsto\psi_++\psi_-.
$$

The resulting [decomposition matrix](../../../representation-theory.md#decomposition-matrix-modular-representation-theory) is connected, so these characters form the unique 5-block $b_0$ of $N$, with defect group $P$. By the [Brauer first main theorem](../../../representation-theory.md#brauer-first-main-theorem),

$$
\boxed{B_0\longleftrightarrow b_0\text{ for }D=C_5,
\qquad B_1\longleftrightarrow B_1\text{ for }D=1.}
$$

This is the complete [5-modular blocks of A5](../../../representation-theory.md#5-modular-blocks-of-a5) correspondence.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
