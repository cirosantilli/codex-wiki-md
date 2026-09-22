# Paper 139

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20139.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20139.pdf)

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
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 139](paper-139.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A ring is [left Noetherian](../../../noncommutative-algebra.md#left-noetherian-ring) when its left ideals satisfy the ascending-chain condition, equivalently when every left ideal is finitely generated; right Noetherian is defined analogously.

Filter $S$ by word degree in $x$. The equality $R+Rx=R+xR$ lets every coefficient move past one $x$ at the cost of lower-degree terms, so

$$
F_nS=R+Rx+\cdots+Rx^n.
$$

For a left ideal $I$, the leading coefficients in degree at most $n$ form an ascending chain of left ideals of $R$. Since $R$ is left Noetherian, this chain stabilizes and each term is finitely generated. Lift finitely many generators through the finitely many degrees before stabilization. Division by their leading terms reduces every element of $I$ to lower degree, and induction shows that these lifts generate $I$. Thus $S$ is left Noetherian.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Put $R=k[x]$. The relation $yr=ry+r'$ gives $R+Ry=R+yR$, so part (a) makes the [Weyl algebra](../../../noncommutative-algebra.md#weyl-algebra) $A_1(k)$ left Noetherian. Applying the same argument to its opposite ring makes it right Noetherian.

Assume $\operatorname{char}k=0$ and let $0\ne I\triangleleft A_1(k)$. Using the PBW basis $x^iy^j$, choose an element of $I$ of least positive $y$-degree. Commutation with $x$ differentiates in $y$, so minimality leaves a nonzero polynomial in $x$. Repeated commutation with $y$ differentiates that polynomial and eventually gives a nonzero scalar. Hence $1\in I$, proving simplicity. In characteristic $p>0$, both $x^p$ and $y^p$ are central, and the proper ideal $(x^p)$ proves that $A_1(k)$ is not simple.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $e=1-XY$, the projection onto constants. Then

$$
e_{ij}=X^ieY^j
$$

are matrix units: $e_{ij}e_{rs}=\delta_{jr}e_{is}$. Consequently

$$
Te_{00}\subsetneq Te_{00}+Te_{01}\subsetneq
Te_{00}+Te_{01}+Te_{02}\subsetneq\cdots
$$

is a strictly ascending chain of left ideals; each new column is independent. Thus $T$ is not left Noetherian. The corresponding row chain

$$
e_{00}T\subsetneq e_{00}T+e_{10}T\subsetneq\cdots
$$

shows that it is not right Noetherian.

## 2

↑ **Parent:** [Paper 139](paper-139.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

[Schur lemma](../../../representation-theory.md#schur-s-lemma) says that a homomorphism between simple modules is either zero or an isomorphism; consequently the endomorphism ring of a simple module is a division ring. Indeed, the kernel and image of a module homomorphism are submodules. Simplicity makes each either zero or the whole module, proving both assertions.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

After replacing $X$ by a maximal $D$-linearly independent subset with the same span, write $X=\{x_1,\ldots,x_n\}$. The standard independence lemma, proved by induction using Schur's lemma, says

$$
\bigcap_{i<n}\operatorname{ann}_R(x_i)\,x_n\ne0.
$$

Otherwise $rx_n$ would depend only on $(rx_1,\ldots,rx_{n-1})$, defining an $R$-map whose coordinate maps lie in $\operatorname{End}_R(V)$ and forcing $x_n\in\sum_{i<n}x_iD$. Applying the same argument with $y$ shows that $\bigcap_i\operatorname{ann}_R(x_i)y=0$ implies $y\in XD$, proving the requested claim.

The [Jacobson density theorem](../../../noncommutative-algebra.md#jacobson-density-theorem) states that if $x_1,\ldots,x_n$ are $D$-independent and $y_1,\ldots,y_n\in V$, there is $r\in R$ with $rx_i=y_i$ for every $i$. Induct on $n$. First match the first $n-1$ values. The independence lemma makes $I x_n$, for $I=\bigcap_{i<n}\operatorname{ann}_R(x_i)$, a nonzero submodule and hence all of $V$; an element of $I$ supplies the final correction.

If $R$ is primitive, choose a faithful simple module $V$. When $\dim_DV=n<\infty$, density makes $R\to\operatorname{End}_D(V)\cong\operatorname{Mat}_n(D)$ surjective and faithfulness makes it injective. If $\dim_DV$ is infinite, choose an $n$-dimensional $D$-subspace $W$ and let $R_n=\{r:rW\subseteq W\}$. Density makes restriction $R_n\to\operatorname{End}_D(W)\cong\operatorname{Mat}_n(D)$ surjective.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For a simple $R$-module $S$, matrix units show that every nonzero vector of $S^n$ generates all coordinates, so $S^n$ is a simple $\operatorname{Mat}_n(R)$-module. Conversely, if $V$ is simple over the matrix ring, $e_{11}V$ is a simple $R$-module and

$$
V\cong(e_{11}V)^n
$$

through the maps induced by $e_{i1}$ and $e_{1i}$. These constructions are inverse on isomorphism classes; this is the basic [Morita equivalence](../../../noncommutative-algebra.md#morita-equivalence) for a matrix ring.

The [Jacobson radical](../../../noncommutative-algebra.md#jacobson-radical) is the intersection of annihilators of all simple left modules. On $S^n$, a matrix annihilates every vector exactly when each entry annihilates $S$. Intersecting over all simple $S$ gives

$$
\boxed{J(\operatorname{Mat}_n(R))=\operatorname{Mat}_n(J(R)).}
$$

## 3

↑ **Parent:** [Paper 139](paper-139.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A module $E$ is [injective](../../../noncommutative-algebra.md#injective-module) if every map $A\to E$ extends across every inclusion $A\hookrightarrow B$. [Baer criterion](../../../noncommutative-algebra.md#baer-criterion) says it suffices to test inclusions of left ideals $I\hookrightarrow R$.

Necessity is immediate. Conversely, order all extensions of a given map $A\to E$ to intermediate submodules of $B$. A maximal one exists by Zorn's lemma. If its domain $C$ is not $B$, choose $b\notin C$ and let $I=\{r:rb\in C\}$. The map $I\to E$, $r\mapsto f(rb)$, extends to $R$ by the hypothesis; its value at $1$ extends $f$ to $C+Rb$, contradicting maximality. Thus $C=B$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

If $R$ is left Noetherian and $I\to\bigoplus_\alpha E_\alpha$ is a map from a left ideal, finitely many generators of $I$ have support in one finite set of summands. The map therefore lands in a finite direct sum of injectives and extends to $R$. Baer's criterion proves that the full direct sum is injective.

Conversely, let $I_1\subseteq I_2\subseteq\cdots$ and put $I=\bigcup I_n$. Embed each $R/I_n$ in an injective module $E_n$. The map

$$
I\longrightarrow\bigoplus_{n\geq1}E_n,\qquad
a\longmapsto(a+I_n)_n
$$

has finite support. If the direct sum is injective, it extends to $R$; the extension's value at $1$ has finite support, forcing $a\in I_n$ for every sufficiently large $n$ and every $a\in I$. Hence the chain stabilizes. This is the [Bass-Papp theorem](../../../noncommutative-algebra.md#bass-papp-theorem).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Over a commutative PID, Baer's criterion reduces to maps $(r)\to E$. Such a map extends to $R$ exactly when every equation $re=x$ with $r\ne0$ is solvable. Thus injective modules are exactly the [divisible modules](../../../noncommutative-algebra.md#divisible-module).

Let $Q$ be the fraction field. The indecomposable injectives are

$$
Q
\quad\text{and}\quad
R[p^{-1}]/R
$$

for one representative $p$ of each associate class of irreducibles. The latter is the $p$-primary Prüfer module, the union of the cyclic modules generated by $p^{-n}+R$. The structure theorem for divisible modules decomposes every divisible module into copies of $Q$ and these Prüfer modules, proving that the list is complete.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Because $N$ is essential in $M$, every associated prime of $M$ occurs in $N$. Since $JN=0$, all these primes contain $J$. For a finitely generated module over a commutative Noetherian ring,

$$
\sqrt{\operatorname{ann}_R(M)}
=\bigcap_{\mathfrak p\in\operatorname{Ass}(M)}\mathfrak p.
$$

Hence $J\subseteq\sqrt{\operatorname{ann}M}$; finite generation of the ideal $J$ gives $J^nM=0$ for some $n$.

Now $R/J$ is essential in its [injective hull](../../../noncommutative-algebra.md#injective-hull). For $x\in E(R/J)$, the finitely generated module $Rx+R/J$ has essential submodule $R/J$, so the result just proved gives $J^nx=0$ for some $n$. The reverse inclusion is tautological, and therefore

$$
\boxed{E(R/J)=\bigcup_{n\geq1}\{x:J^nx=0\}.}
$$

## 4

↑ **Parent:** [Paper 139](paper-139.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A multiplicatively closed set $S$ is a [left Ore set](../../../noncommutative-algebra.md#left-ore-set) if for every $s\in S$ and $r\in R$ there are $s'\in S,r'\in R$ with $s'r=r's$. This condition gives common left annihilators, so $t_S(M)$ is closed under addition and scalar multiplication in every module.

Conversely apply the assumed submodule property to $M=R/Rs$. The element $1+Rs$ is $S$-torsion, hence so is $r+Rs$. Thus some $s'\in S$ satisfies $s'r\in Rs$, say $s'r=r's$, which is precisely the Ore condition.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

A proper two-sided ideal $P$ is [prime](../../../noncommutative-algebra.md#prime-ideal-of-a-noncommutative-ring) when $AB\subseteq P$ for two-sided ideals implies $A\subseteq P$ or $B\subseteq P$. The nilpotent ideal $ke_{21}$ lies in every prime of $T_2(k)$, and the quotient is $k\times k$. Hence the two primes are

$$
P_a=\{(a,c,d):a=0\},\qquad
P_d=\{(a,c,d):d=0\}.
$$

Here $\mathcal C(P_a)=\{a\ne0\}$ and $\mathcal C(P_d)=\{d\ne0\}$.

Direct multiplication of triples

$$
(a,c,d)(a',c',d')=(aa',ca'+dc',dd')
$$

shows that all of $\mathcal C(P_a)$ satisfies the left Ore equations. For $P_d$, the largest left Ore subset is

$$
\{(a,c,d):a\ne0,\ d\ne0\}=T_2(k)^*.
$$

Indeed units always form an Ore set. If $d\ne0$ but $a=0$, applying the Ore equation successively to $e_{21}$ and $e_{22}$ gives incompatible equations, so no left Ore subset can contain that element.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let $D=\partial_t$. Since

$$
[tD+\lambda,D]=-D,
$$

the assignments $\theta_\lambda(y)=tD+\lambda$ and $\theta_\lambda(x)=D$ respect $[y,x]=-x$ and extend through the [universal enveloping algebra](../../../lie-algebra.md#universal-enveloping-algebra).

The operator $y$ has distinct eigenvectors $t^n$ with eigenvalues $\lambda+n$, while $x(t^n)=nt^{n-1}$. Therefore the submodules are exactly

$$
0,\quad k\oplus kt\oplus\cdots\oplus kt^m\ (m\geq0),\quad k[t].
$$

The character $x\mapsto0$, $y\mapsto\lambda$ has kernel $I_\lambda$, so $U(\mathfrak g)/I_\lambda\cong k$ and $I_\lambda$ is maximal.

By part (a), the $S$-torsion in every module is a submodule. On $V=k\oplus kt$, $x(t)=1$ and $y$ has eigenvalues $\lambda,\lambda+1$. If some $s\in S$ vanished on the $(\lambda+1)$-character, then $s(t)\in k$. Since $s(1)$ is the nonzero scalar given by its image modulo $I_\lambda$, subtracting a suitable constant from $t$ would produce an $S$-torsion vector $v$ with $xv=1$. Submodule closure would make $1$ torsion, contradicting $S\subseteq\mathcal C(I_\lambda)$. Thus

$$
S\subseteq\mathcal C(I_\lambda)\cap\mathcal C(I_{\lambda+1}).
$$

Apply the same argument to each adjacent two-dimensional quotient

$$
(k\oplus\cdots\oplus kt^{n+1})/(k\oplus\cdots\oplus kt^{n-1})
$$

where $x(t^{n+1})=(n+1)t^n\ne0$ because $\operatorname{char}k=0$. Induction gives

$$
\boxed{S\subseteq\bigcap_{n\in\mathbb N_0}\mathcal C(I_{\lambda+n}).}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
