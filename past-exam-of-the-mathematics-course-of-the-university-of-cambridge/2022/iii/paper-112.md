# Paper 112

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/Paper_112.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/Paper_112.pdf)

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
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)

## 1

↑ **Parent:** [Paper 112](paper-112.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Let $K_1$ be the [connected sum](../../../knot-theory.md#connected-sum-of-knots) of $2022$ [trefoils](../../../knot-theory.md#trefoil-knot). The trefoil has [Seifert genus](../../../knot-theory.md#seifert-genus) one, and [additivity of Seifert genus](../../../knot-theory.md#additivity-of-seifert-genus) gives

$$
\boxed{g_s(K_1)=2022.}
$$

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Take the [twist knot](../../../knot-theory.md#twist-knot) whose standard diagram has $2020$ half-twists in its twist region and two crossings in its clasp. Every nontrivial twist knot has [Seifert genus](../../../knot-theory.md#seifert-genus) one. This diagram is a [reduced](../../../knot-theory.md#reduced-knot-diagram) [alternating knot diagram](../../../knot-theory.md#alternating-knot-diagram), so the [Tait crossing-number theorem](../../../knot-theory.md#tait-crossing-number-theorem) says that its $2020+2=2022$ crossings realize the [crossing number of a knot](../../../knot-theory.md#crossing-number-of-a-knot). Thus this knot has $g_s(K_2)=1$ and $c(K_2)=2022$.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Consider the symmetric [Laurent polynomial](../../../polynomial.md#laurent-polynomial)

$$
f(t)=t^2-1+t^{-2}.
$$

It satisfies $f(1)=1$, so the [Alexander polynomial realization theorem](../../../knot-theory.md#alexander-polynomial-realization-theorem) gives a [knot](../../../knot-theory.md#knot) $K_3$ with $\Delta_{K_3}(t)\doteq f(t)$. The polynomial is not a [unit](../../../algebra.md#unit-in-a-ring) of $\mathbb Z[t^{\pm1}]$, whereas

$$
\boxed{\det K_3=|\Delta_{K_3}(-1)|=|1-1+1|=1.}
$$

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

Take the untwisted [Whitehead double](../../../knot-theory.md#whitehead-double) of a [trefoil knot](../../../knot-theory.md#trefoil-knot). The Whitehead pattern has [winding number of a satellite pattern](../../../knot-theory.md#winding-number-of-a-satellite-pattern) zero and becomes the [unknot](../../../knot-theory.md#unknot) when its companion is the unknot. The [Satellite formula for the Alexander polynomial](../../../knot-theory.md#satellite-formula-for-the-alexander-polynomial) therefore gives

$$
\Delta_{K_4}(t)\doteq\Delta_{P(U)}(t)\Delta_{T_{2,3}}(1)=1.
$$

The Whitehead pattern is geometrically essential in its solid torus, so the [satellite knot](../../../knot-theory.md#satellite-knot) with nontrivial companion $T_{2,3}$ is nontrivial. Hence $K_4$ is not isotopic to the unknot despite having trivial [Alexander polynomial of a knot](../../../knot-theory.md#alexander-polynomial).

## 2

↑ **Parent:** [Paper 112](paper-112.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Apply the [Kauffman bracket](../../../knot-theory.md#kauffman-bracket) skein relation to every crossing in the two-string [tangle](../../../knot-theory.md#tangle) $D_1$. Each complete smoothing is a collection of closed circles together with one of the two crossingless pairings of the four boundary points. Rotation through $180^\circ$ about the indicated vertical axis preserves both crossingless pairings and the number of closed circles. Gluing the unchanged tangle $D_2$ to corresponding smoothings therefore gives equal terms, including equal loop factors, so $\langle D\rangle=\langle D'\rangle$.

Choose an orientation of $L$, and transport the induced orientations of the four ends of $D_1$ through the rotation to orient $L'$. Crossing signs inside the rotated tangle and outside it then have the same total, so the [writhe of a link diagram](../../../knot-theory.md#writhe-of-a-link-diagram) satisfies $w(D)=w(D')$. Applying the writhe normalization of the [Jones polynomial](../../../knot-theory.md#jones-polynomial) gives

$$
\boxed{V_L(t)=V_{L'}(t).}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The component knot types can change under this [Conway mutation](../../../knot-theory.md#mutation-knot-theory). To construct an example, place a knotted arc carrying a [trefoil knot](../../../knot-theory.md#trefoil-knot) summand in one strand of $D_1$ and a knotted arc carrying a [figure-eight knot](../../../knot-theory.md#figure-eight-knot) summand in one strand of $D_2$, leaving the other two strand portions trivial. Choose the outside pairing so that before rotation the two knotted portions lie on different components, while after rotation they lie on the same component. Then the component multisets are

$$
\{T_{2,3},4_1\}
\quad\hbox{and}\quad
\{T_{2,3}\mathbin{\#}4_1,U\},
$$

respectively. A [link isotopy](../../../knot-theory.md#link-isotopy) preserves the unordered multiset of component knot types, so these links are not isotopic, although part (a) shows that suitable orientations give them the same [Jones polynomial](../../../knot-theory.md#jones-polynomial).

## 3

↑ **Parent:** [Paper 112](paper-112.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Give each bounded region $R_i$ a generator $a_i$ and give the unbounded region $R_0$ the identity generator. At every crossing, read the four incident regions cyclically as $a,b,c,d$ and impose

$$
ab^{-1}cd^{-1}=1.
$$

Using the opposite cyclic convention inverts all such relators and gives the same group. One crossing relation is redundant, leaving $n$ generators and $n-1$ relators; this is the [Dehn presentation of a knot group](../../../knot-theory.md#dehn-presentation-of-a-knot-group).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Orient the diagram and assign its regions an [Alexander numbering](../../../knot-theory.md#alexander-numbering) with $R_0$ numbered zero. The [abelianization](../../../group-theory.md#abelianization) $\phi:\pi_1(E_K)\to\langle t\rangle$ sends $a_i$ to $t^{m_i}$, where $m_i$ is the number of $R_i$. Since $R_1$ is adjacent to $R_0$, $m_1=\pm1$.

Form the square matrix

$$
A_1=\left(\phi\!\left(\frac{\partial w_j}{\partial a_i}\right)\right)_{
1\leq j\leq n-1,\ 2\leq i\leq n}
$$

from the [Fox derivatives](../../../geometric-group-theory.md#fox-calculus) with respect to $a_i$ for $i>1$. This is the [Alexander matrix](../../../knot-theory.md#alexander-matrix) with the $a_1$ column deleted. The Fox identity implies that its maximal minors differ by the factors $\phi(a_i)-1$, and the standard presentation of the [Alexander module](../../../knot-theory.md#alexander-module-of-a-knot) therefore gives

$$
\det A_1\doteq\frac{t^{m_1}-1}{t-1}\Delta_K(t)\doteq\Delta_K(t),
$$

because $m_1=\pm1$. Thus $\Delta_K(t)$ is $\det A_1$ up to a unit $\pm t^r$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Expand the [determinant](../../../linear-algebra.md#determinant) of the matrix $A_1$ from part (b) by the [Leibniz formula for determinants](../../../linear-algebra.md#leibniz-formula-for-determinants). A matrix entry is a signed sum of [monomials](../../../polynomial.md#monomial) arising from the possible corners at its crossing. Choosing one summand in every row chooses one corner at every crossing, while choosing distinct columns puts exactly one chosen corner in every region $R_i$ with $i>1$ and none in the two deleted regions $R_0,R_1$. The surviving determinant terms are therefore in bijection with the [Kauffman states](../../../knot-theory.md#kauffman-state-of-a-knot-diagram) $s\in\mathcal S(D)$.

The [sign of a permutation](../../../finite-group-theory.md#sign-of-a-permutation) in the determinant together with the corner signs gives $(-1)^{\epsilon(s)}$, and multiplying the corner monomials gives $t^{\delta(s)}$. Since part (b) identifies this determinant with the [Alexander polynomial of a knot](../../../knot-theory.md#alexander-polynomial) up to a unit,

$$
\boxed{\Delta_K(t)\doteq\sum_{s\in\mathcal S(D)}(-1)^{\epsilon(s)}t^{\delta(s)}.}
$$

## 4

↑ **Parent:** [Paper 112](paper-112.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [Wirtinger presentation](../../../knot-theory.md#wirtinger-presentation) from a connected [knot diagram](../../../knot-theory.md#knot-diagram) has one generator per arc and one relator per crossing, with one relator redundant. Its presentation complex is a finite two-dimensional [CW complex](../../../algebraic-topology.md#cw-complex) $X$ with one zero-cell, $n$ one-cells, and $n-1$ two-cells, and the usual diagrammatic construction gives a [homotopy equivalence](../../../algebraic-topology.md#homotopy-equivalence) $X\simeq E_K$.

The [abelianization](../../../group-theory.md#abelianization) of the [knot group](../../../knot-theory.md#knot-group) is $H_1(E_K;\mathbb Z)\cong\mathbb Z$, generated by a [meridian of a knot](../../../knot-theory.md#meridian-of-a-knot). Every homomorphism to the [cyclic group](../../../group.md#cyclic-group) $\mathbb Z/2$ factors through this abelianization, and reduction modulo two is its unique surjection. Thus the requested map $\alpha$ is unique.

Its kernel determines a two-sheeted [covering space](../../../algebraic-topology.md#covering-space) $\widehat X$. The nontrivial [deck transformation](../../../algebraic-topology.md#deck-transformation) acts on cellular chains and homology, giving them module structures over the [group ring](../../../commutative-algebra.md#group-ring)

$$
\widehat R=\mathbb Z[\mathbb Z/2]\cong\mathbb Z[t]/(t^2-1).
$$

Lift one copy of every cell of $X$; its two deck translates form a free $\widehat R$-basis. Hence $C_0\cong\widehat R$, $C_1\cong\widehat R^n$, and $C_2\cong\widehat R^{n-1}$. If $\widetilde X$ is the [infinite cyclic cover](../../../knot-theory.md#infinite-cyclic-cover-of-a-knot-exterior), its cellular chains are free over $R=\mathbb Z[t^{\pm1}]$, and imposing $t^2=1$ gives

$$
C_*^{\mathrm{cell}}(\widehat X)\cong C_*^{\mathrm{cell}}(\widetilde X)\otimes_R\widehat R.
$$

For an odd prime $p$, the two [idempotents](../../../commutative-algebra.md#idempotent) $e_+=(1+t)/2$ and $e_-=(1-t)/2$ split the [group algebra](../../../associative-algebra.md#group-algebra)

$$
\mathbb F_p[\mathbb Z/2]\cong R_+\oplus R_-,
\qquad R_+=\mathbb F_p[t^{\pm1}]/(t-1),\quad R_-=\mathbb F_p[t^{\pm1}]/(t+1).
$$

The plus summand is the cellular chain complex of $X$ with $\mathbb F_p$ coefficients, while the minus summand is $C_-=C_*^{\mathrm{cell}}(\widetilde X)\otimes_RR_-$. Therefore

$$
H_*(\widehat X;\mathbb F_p)\cong H_*(E_K;\mathbb F_p)\oplus H_*(C_-).
$$

On the minus summand, the boundary $t-1:C_1\to C_0$ becomes multiplication by $-2$, which is invertible in $\mathbb F_p$, so $H_0(C_-)=0$. After the corresponding cancellation, the remaining square boundary matrix is an [Alexander matrix](../../../knot-theory.md#alexander-matrix) specialized at $t=-1$. It is singular over $\mathbb F_p$ exactly when

$$
\Delta_K(-1)\equiv0\pmod p,
$$

or equivalently when $p$ divides the [knot determinant](../../../knot-theory.md#knot-determinant) $\det K$. Thus $H_*(C_-)$ is nonzero exactly in that case.

Finally, $\det K=|\Delta_K(-1)|$ is a nonzero odd integer, so the minus complex is acyclic over $\mathbb Q$. Since a knot exterior has the rational homology of a circle,

$$
\boxed{H_i(\widehat X;\mathbb Q)\cong
\begin{cases}
\mathbb Q,&i=0,1,\\
0,&i\geq2.
\end{cases}}
$$

## 5

↑ **Parent:** [Paper 112](paper-112.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

A [framing of an embedded sphere](../../../algebraic-geometry.md#framing-of-an-embedded-sphere) $C:S^{k-1}\hookrightarrow N^{n-1}$ is a trivialization of its rank-$(n-k)$ [normal bundle](../../../algebraic-geometry.md#normal-bundle). The standard complex line $\mathbb{CP}^1\subset\mathbb{CP}^2$ has normal bundle of [Euler number](../../../fiber-bundle.md#euler-number-of-a-vector-bundle) $+1$, so this embedded $S^2$ has no framing.

If one framing $f_0$ exists, every other orientation-compatible framing is obtained from it by a map $S^{k-1}\to SO(n-k)$. Consequently the set of homotopy classes is a torsor for

$$
[S^{k-1},SO(n-k)]=\pi_{k-1}(SO(n-k)).
$$

For $k=2$ and $n=4$, this is $\pi_1(SO(2))\cong\mathbb Z$; the integer is the winding number of one framing relative to $f_0$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Distinct components of the positively oriented [torus link](../../../knot-theory.md#torus-link) $T_{n,n}$ have [linking number](../../../knot-theory.md#linking-number) one. Since every component also has framing $+1$ relative to the [Seifert framing](../../../knot-theory.md#seifert-framing), the [surgery linking matrix](../../../knot-theory.md#surgery-linking-matrix) and hence the [intersection form](../../../homology.md#intersection-form) of the [surgery trace](../../../knot-theory.md#surgery-trace) $W(\widehat L_1)$ are

$$
Q_1=J_n=
\begin{pmatrix}
1&\cdots&1\\
\vdots&\ddots&\vdots\\
1&\cdots&1
\end{pmatrix}.
$$

Its [Smith normal form](../../../algebra.md#smith-normal-form) is $\operatorname{diag}(1,0,\ldots,0)$. The surgery exact sequence, equivalently the kernel and cokernel of $Q_1$, gives

$$
H_i(S^3_{\widehat L_1};\mathbb Z)\cong
\begin{cases}
\mathbb Z,&i=0,3,\\
\mathbb Z^{n-1},&i=1,2,\\
0,&\text{otherwise}.
\end{cases}
$$

In [Kirby calculus](../../../knot-theory.md#kirby-calculus), sliding the components over one chosen component diagonalizes the framed link to a split $+1$-framed unknot and $n-1$ zero-framed unknots. Hence

$$
W(\widehat L_1)\cong(\mathbb{CP}^2\setminus\operatorname{int}B^4)\,\natural\,\mathop{\natural}_{n-1}(S^2\times D^2),
\qquad
\boxed{S^3_{\widehat L_1}\cong\mathop{\#}_{n-1}(S^1\times S^2),}
$$

where $\natural$ denotes [boundary connected sum](../../../differential-geometry.md#boundary-connected-sum).

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

With zero framings, the [surgery linking matrix](../../../knot-theory.md#surgery-linking-matrix) is

$$
Q_2=J_n-I_n.
$$

Its eigenvalues are $n-1$ on the span of $(1,\ldots,1)$ and $-1$ on the complementary subspace, so $\det Q_2=(-1)^{n-1}(n-1)$. For $n>1$, its [Smith normal form](../../../algebra.md#smith-normal-form) is $\operatorname{diag}(1,\ldots,1,n-1)$, and therefore

$$
H_i(S^3_{\widehat L_2};\mathbb Z)\cong
\begin{cases}
\mathbb Z,&i=0,3,\\
\mathbb Z/(n-1),&i=1,\\
0,&\text{otherwise}.
\end{cases}
$$

Handle slides reduce this surgery diagram to the standard surgery diagram of the [lens space](../../../knot-theory.md#lens-space) $L(n-1,1)$; equivalently, the generator of the cokernel has linking pairing $1/(n-1)$. Thus

$$
\boxed{S^3_{\widehat L_2}\cong L(n-1,1)}
$$

up to the orientation convention for surgery. When $n=1$, the matrix is $(0)$ and the exceptional answer is $S^1\times S^2$, with $H_1\cong H_2\cong\mathbb Z$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
