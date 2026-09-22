# Paper 112

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20112.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20112.pdf)

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
  - [e](#1/e)
    - [Solution](#1/e/solution)
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

## 1

↑ **Parent:** [Paper 112](paper-112.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [Seifert surface](../../../knot-theory.md#seifert-surface) for an [oriented knot](../../../knot-theory.md#oriented-knot) $K$ is a compact connected oriented surface $F\subset S^3$ whose oriented boundary is $K$. For homology classes represented by oriented curves $x,y\subset F$, the [Seifert form](../../../knot-theory.md#seifert-form) is

$$
\theta_F([x],[y])=\operatorname{lk}(x^+,y),
$$

where $x^+$ is the positive normal push-off. Choosing a basis of $H_1(F;\mathbb Z)$ gives a [Seifert matrix](../../../knot-theory.md#seifert-matrix) $A$.

For $\omega\in S^1\setminus\{1\}$, the [Levine-Tristram signature](../../../knot-theory.md#levine-tristram-signature) is

$$
\sigma_\omega(K)=\operatorname{sign}\bigl((1-\omega)A+(1-\overline\omega)A^T\bigr).
$$

The determinant of this Hermitian matrix vanishes away from $\omega=1$ exactly at the unit roots of the [Alexander polynomial of a knot](../../../knot-theory.md#alexander-polynomial) $\Delta_K$. Consequently the signature is locally constant on their complement.

For $\omega=e^{i\theta}$ near $1$,

$$
(1-\omega)A+(1-\overline\omega)A^T
=i\theta(A^T-A)+O(\theta^2).
$$

The real skew-symmetric unimodular matrix $A^T-A$ has standard symplectic blocks, so the Hermitian matrix $i(A^T-A)$ has its positive and negative [eigenvalues](../../../linear-operator-theory.md#eigenvalue) in opposite pairs and has signature zero. Thus $\sigma_\omega(K)=0$ near $1$. If $\Delta_K$ has no unit roots, then $S^1\setminus\{1\}$ contains no singular point of the signature form and is connected, so local constancy gives $\sigma_\omega(K)=0$ everywhere. With the usual convention $\sigma_1(K)=0$, the signature vanishes identically.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $V=S^1\times D^2$ contain the [pattern of a satellite knot](../../../knot-theory.md#pattern-of-a-satellite-knot) $P$. Its class in $H_1(V;\mathbb Z)\cong\mathbb Z$ is the [winding number of a satellite pattern](../../../knot-theory.md#winding-number-of-a-satellite-pattern). Winding number zero therefore makes $P$ null-homologous in $V$, so $P$ bounds an oriented embedded surface $F_P\subset V$. Let

$$
g_P=g(F_P).
$$

For any companion [knot](../../../knot-theory.md#knot) $K$, an embedding $V\hookrightarrow S^3$ as a tubular neighborhood of $K$ carries $F_P$ to a [Seifert surface](../../../knot-theory.md#seifert-surface) for the [satellite knot](../../../knot-theory.md#satellite-knot) $P(K)$. Hence

$$
g_s(P(K))\leq g(F_P)=g_P,
$$

and the bound depends only on the pattern.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Boundary-connected-summing minimal [Seifert surfaces](../../../knot-theory.md#seifert-surface) for $K$ and $K'$ gives

$$
g_s(K\mathbin{\#}K')\leq g_s(K)+g_s(K').
$$

For the reverse inequality, let $F$ be a minimal-genus Seifert surface for the [connected sum of knots](../../../knot-theory.md#connected-sum-of-knots) and let $S$ be its standard splitting sphere. A minimal-genus Seifert surface is incompressible in the knot exterior: a compression either lowers its genus or separates off a closed component that can be discarded. Put $F$ and $S$ in transverse position and minimize the number of intersection circles. An innermost circle on $S$ either gives a compression of $F$ or bounds a disk on $F$ across which it can be removed. Both alternatives contradict minimality, so $F\cap S$ consists only of the single arc joining the two points of $S\cap\partial F$.

Cutting $F$ along this arc gives Seifert surfaces $F_1,F_2$ for $K,K'$. Their Euler characteristics satisfy

$$
\chi(F)=\chi(F_1)+\chi(F_2)-1,
$$

which, since all three surfaces have one boundary component, is equivalent to

$$
g(F)=g(F_1)+g(F_2)\geq g_s(K)+g_s(K').
$$

This proves additivity.

The [torus knot](../../../knot-theory.md#torus-knot) $T_{2,3}$ bounds a once-punctured torus, and its degree-two [Alexander polynomial of a knot](../../../knot-theory.md#alexander-polynomial) forces every Seifert surface to have genus at least one. Thus $g_s(T_{2,3})=1$. If it were a [composite knot](../../../knot-theory.md#composite-knot), both nontrivial summands would have positive Seifert genus, and additivity would give genus at least two. Hence $T_{2,3}$ is a [prime knot](../../../knot-theory.md#prime-knot).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Induct on the [Seifert genus](../../../knot-theory.md#seifert-genus) $g_s(K)$. A genus-zero knot is the [unknot](../../../knot-theory.md#unknot). If $K$ is prime there is nothing to prove. Otherwise write $K=K_1\mathbin{\#}K_2$ with both summands nontrivial. Part c gives

$$
g_s(K)=g_s(K_1)+g_s(K_2),
$$

so each summand has strictly smaller genus than $K$. Apply the induction hypothesis to both. Since the genus drops at every nontrivial split, the process terminates after finitely many steps and expresses $K$ as a finite [connected sum](../../../knot-theory.md#connected-sum-of-knots) of [prime knots](../../../knot-theory.md#prime-knot).

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

If $K=K_1\mathbin{\#}K_2$ with both summands nontrivial, the sphere separating the two punctured three-balls in the connected-sum construction is a [splitting sphere of a knot](../../../knot-theory.md#splitting-sphere-of-a-knot). If it were trivial, the corresponding one-string tangle would be boundary-parallel and one of $K_1,K_2$ would be the [unknot](../../../knot-theory.md#unknot). The sphere is therefore nontrivial.

Conversely, a splitting sphere $S$ divides $S^3$ into three-balls $B_1,B_2$, and $K\cap B_i$ is a properly embedded arc. Join its endpoints by a fixed arc on $S$ and push that joining arc slightly into $B_i$; this closes the two tangles to knots $K_1,K_2$. Reversing the construction shows

$$
K=K_1\mathbin{\#}K_2.
$$

If either $K_i$ were unknotted, an innermost-disk argument for a spanning disk of $K_i$ would make the corresponding tangle boundary-parallel, which is exactly the stated triviality condition for $S$. A nontrivial splitting sphere therefore makes both summands nontrivial, so $K$ is composite.

## 2

↑ **Parent:** [Paper 112](paper-112.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

After replacing a class by a nonsingular representative, let $A$ represent a [Seifert form](../../../knot-theory.md#seifert-form) over a field $F$ of characteristic different from two. Set

$$
Q=A+A^T,
\qquad
T=A^{-1}A^T.
$$

A direct calculation gives $T^TQT=Q$, so $(F^{2g},Q,T)$ is an [isometric structure](../../../knot-theory.md#isometric-structure). A metabolizer for $A$ corresponds to a $T$-invariant metabolizer for $Q$, and stabilization gives the canonical homomorphism

$$
\mathcal{AC}_F\longrightarrow\mathcal W_F.
$$

Conversely, for an isometric structure with $I+T$ invertible, define

$$
A=Q(I+T)^{-1}.
$$

Then $A+A^T=Q$ and $A^{-1}A^T=T$. These constructions respect orthogonal sums and metabolic structures and are inverse on Witt classes, proving $\mathcal{AC}_F\cong\mathcal W_F$.

For an irreducible symmetric Laurent polynomial $\delta$, the [primary component of an isometric structure](../../../knot-theory.md#primary-component-of-an-isometric-structure) is

$$
V_\delta=\ker\delta(T)^N
$$

for large $N$. The primary decomposition is orthogonal, so restriction of $Q$ and $T$ to $V_\delta$ defines the projection

$$
\mathcal W_F\longrightarrow\mathcal W_F^\delta.
$$

Now take $F=\mathbb R$ and let $\delta$ have roots $\omega,\overline\omega$ on the unit circle, with $\omega=e^{i\theta}$ in the upper half-plane. The isomorphism $\mathcal W_{\mathbb R}^\delta\cong2\mathbb Z$ sends a class to the even signature jump

$$
J_\omega=lim_{\varepsilon\downarrow0}
\left(\sigma_{e^{i(\theta+\varepsilon)}}-
\sigma_{e^{i(\theta-\varepsilon)}}\right).
$$

For the class of a knot, this is precisely the jump of its [Levine-Tristram signature](../../../knot-theory.md#levine-tristram-signature) at the root $\omega$; reversing the choice of side changes the overall sign convention.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Over $\mathbb R$, the relevant part of the [Alexander polynomial of a knot](../../../knot-theory.md#alexander-polynomial) of $T_{2,5}$ has the two irreducible symmetric factors

$$
\delta_1(t)=t+t^{-1}-2\cos(\pi/5),
\qquad
\delta_3(t)=t+t^{-1}-2\cos(3\pi/5).
$$

Their upper-half-plane roots are $\alpha=e^{\pi i/5}$ and $\alpha^3=e^{3\pi i/5}$. The supplied determinant shows that the [Levine-Tristram signature](../../../knot-theory.md#levine-tristram-signature) can jump only at these roots and their conjugates.

For the supplied [Seifert matrix](../../../knot-theory.md#seifert-matrix), direct inertia calculations on successive arcs of the upper semicircle give

$$
\sigma_\omega(T_{2,5})=
\begin{cases}
0,&0<\arg\omega<\pi/5,\\
-2,&\pi/5<\arg\omega<3\pi/5,\\
-4,&3\pi/5<\arg\omega\leq\pi.
\end{cases}
$$

Changing the orientation convention reverses all signs but changes no conclusion. Thus the jumps at both $\alpha$ and $\alpha^3$ are $-2$. It follows from part a that

$$
[T_{2,5}]_\delta\ne0
\quad\Longleftrightarrow\quad
\delta\doteq\delta_1\text{ or }\delta_3,
$$

and in both nonzero cases the image is a generator of $\mathcal W_{\mathbb R}^\delta\cong2\mathbb Z$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

In fact the conclusion holds for every [amphichiral knot](../../../knot-theory.md#amphichiral-knot); the hypothesis on the [Arf invariant of a knot](../../../knot-theory.md#arf-invariant-of-a-knot) is unnecessary. Let $Y=\Sigma_2(K)$ be the [two-fold branched cover of a knot](../../../knot-theory.md#two-fold-branched-cover-of-a-knot). Amphichirality gives an orientation-reversing self-homeomorphism of $Y$, so its [linking form of a branched cover](../../../knot-theory.md#linking-form-of-a-branched-cover) satisfies

$$
(H_1(Y),\lambda_Y)\cong(H_1(Y),-\lambda_Y).
$$

Fix an odd prime $p$ and pass to the $p$-primary subgroup. The standard filtration by powers of $p$ decomposes its linking form into nonsingular symmetric forms over $\mathbb F_p$. On a graded piece of dimension $d$, an anti-isometry has a matrix $P$ satisfying

$$
P^TAP=-A.
$$

Taking determinants gives

$$
(\det P)^2=(-1)^d.
$$

If $p\equiv3\pmod4$, then $-1$ is not a square in $\mathbb F_p$, so every such $d$ is even. The sum of these graded dimensions is the exponent

$$
\nu_p|H_1(Y)|=\nu_p|\Delta_K(-1)|.
$$

It is therefore even, as required.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

For the supplied [Seifert matrix](../../../knot-theory.md#seifert-matrix) $A$,

$$
\Delta_K(t)=\det(tA-A^T)
=-t^4+3t^3-3t^2+3t-1,
$$

and the symmetric form $Q=A+A^T$ has signature $-2$. Thus

$$
\sigma_{-1}(K)=-2\ne0.
$$

Since the [Levine-Tristram signature](../../../knot-theory.md#levine-tristram-signature) is an additive homomorphism on the [algebraic concordance group](../../../knot-theory.md#algebraic-concordance-of-knots), $K$ has infinite algebraic-concordance order.

Over $\mathbb Q_3$, reduction of the Alexander polynomial gives

$$
-\Delta_K(t)\equiv(t^2+t-1)(t^2-t-1)\pmod3.
$$

The factors are coprime, nonsymmetric, and exchanged by reciprocity. Hensel lifting therefore decomposes the local isometric structure into a reciprocal pair, which is metabolic. Its class in $\mathcal W_{\mathbb Q_3}$ is zero and in particular does not have order four.

For $p=11$, diagonalization gives

$$
Q\sim\left\langle-2,-\frac32,2,-\frac{11}{6}\right\rangle.
$$

The second residue at $11$ is the one-dimensional form

$$
\left\langle-\frac16\right\rangle
=\langle9\rangle=\langle1\rangle
\quad\text{in }W(\mathbb F_{11}).
$$

Because $11\equiv3\pmod4$, $W(\mathbb F_{11})\cong\mathbb Z/4$ and this one-dimensional form is a generator. The [P-adic algebraic-concordance obstruction](../../../knot-theory.md#p-adic-algebraic-concordance-obstruction) therefore has exact order four, so the image of $K$ in $\mathcal W_{\mathbb Q_{11}}$ has order four.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

The [Satellite formula for the Levine-Tristram signature](../../../knot-theory.md#satellite-formula-for-the-levine-tristram-signature) applied to the $(2,5)$ [cable knot](../../../knot-theory.md#cable-knot) gives

$$
\sigma_\omega(K_{2,5})
=\sigma_\omega(T_{2,5})+\sigma_{\omega^2}(K).
$$

At $\omega=-1$, the second term is $\sigma_1(K)=0$, whereas part b gives

$$
|\sigma_{-1}(T_{2,5})|=4.
$$

The [Levine-Tristram signature bound on the slice genus](../../../knot-theory.md#levine-tristram-signature-bound-on-the-slice-genus) now yields

$$
2g_4(K_{2,5})\geq|\sigma_{-1}(K_{2,5})|=4.
$$

**Hence $g_4(K_{2,5})\geq2$, so the cable cannot bound a punctured torus in $B^4$.**

## 3

↑ **Parent:** [Paper 112](paper-112.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [slice knot](../../../knot-theory.md#slice-knot) is a knot $K\subset S^3=\partial B^4$ that bounds a smooth properly embedded [slice disk](../../../knot-theory.md#slice-disk) in $B^4$. A [doubly slice knot](../../../knot-theory.md#doubly-slice-knot) is a transverse equatorial cross-section of an unknotted smooth two-sphere in $S^4$.

The [slice genus](../../../knot-theory.md#slice-genus) $g_4(K)$ is the minimum genus of a smooth compact connected oriented surface properly embedded in $B^4$ with boundary $K$. The [double slice genus](../../../knot-theory.md#double-slice-genus) $g_{ds}(K)$ is the minimum genus of an unknotted closed connected oriented surface in $S^4$ whose transverse intersection with an equatorial $S^3$ is $K$. Thus slice and doubly slice mean respectively $g_4(K)=0$ and $g_{ds}(K)=0$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Remove a small ball meeting $K$ in an unknotted arc. The remaining knotted arc lies in a three-ball. Rotate that ball once around its boundary two-sphere in $S^4$ and rotate the arc through $m$ additional full twists during the revolution. The trace, capped along the fixed endpoints, is the [twist-spun knot](../../../knot-theory.md#twist-spun-knot) $\operatorname{Tw}_m(K)$.

The [Zeeman theorem on twist-spun knots](../../../knot-theory.md#zeeman-theorem-on-twist-spun-knots) says that the complement fibers over $S^1$ with fiber the punctured $m$-fold cyclic branched cover of $S^3$ over $K$. For $m=1$ or $-1$ this cover is $S^3$, so $\operatorname{Tw}_{\pm1}(K)$ is unknotted.

A projection-independent specification of the requested [banded-unlink diagram](../../../knot-theory.md#banded-unlink-diagram) for $\operatorname{Tw}_0(T_{2,3})$ is as follows. Draw a reflection-symmetric diagram of $T_{2,3}\mathbin{\#}(-T_{2,3})$ with the connected-sum neck on the symmetry axis. Cut at the neck, perform the oriented smoothing in each reflected crossing pair to obtain the lower unlink, and retain the two dual rectangular bands in each pair, one above and one below the projection plane. Simultaneous surgery on all these paired bands gives the reflected upper unlink. Capping the two unlinks produces exactly the spinning movie: the lower half rotates the cut trefoil through one semicircle and the upper half supplies its mirror semicircle. The paired placement of the bands records zero twisting; adding one full relative twist to every band pair gives the corresponding $m$-twist-spun diagram.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

A genus-one [Seifert matrix](../../../knot-theory.md#seifert-matrix) for the [Stevedore knot](../../../knot-theory.md#stevedore-knot) is

$$
A=\begin{pmatrix}1&1\\0&-2\end{pmatrix}.
$$

Its Alexander polynomial is

$$
\Delta(t)=\det(tA-A^T)=-2t^2+5t-2,
$$

whose roots are $2$ and $1/2$. There are no unit roots, so Question 1(a) proves that every [Levine-Tristram signature](../../../knot-theory.md#levine-tristram-signature) of the Stevedore knot vanishes.

On the other hand,

$$
A+A^T=\begin{pmatrix}2&1\\1&-4\end{pmatrix}
$$

has Smith normal form $\operatorname{diag}(1,9)$. Therefore

$$
H_1(\Sigma_2(6_1))\cong\mathbb Z/9.
$$

If a knot is doubly slice, the linking form on the first homology of its [two-fold branched cover of a knot](../../../knot-theory.md#two-fold-branched-cover-of-a-knot) is hyperbolic: it has two complementary metabolizers, arising from the two sides of the unknotted sphere. A cyclic group of order nine has a unique subgroup of order three, so its [linking form of a branched cover](../../../knot-theory.md#linking-form-of-a-branched-cover) cannot have two complementary metabolizers. The Stevedore knot is consequently not [doubly slice](../../../knot-theory.md#doubly-slice-knot), despite its identically vanishing signature function.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

In either diagram of the [Stevedore knot](../../../knot-theory.md#stevedore-knot), the evident ribbon band can be cut to leave a two-component [unlink](../../../knot-theory.md#unlink). Cap those components by disjoint disks in $B^4$ and restore the band. This constructs a [ribbon disk](../../../knot-theory.md#ribbon-disk), hence proves that the Stevedore knot is [slice](../../../knot-theory.md#slice-knot).

The two displayed Stevedore diagrams give two distinct ribbon-band presentations. Use one below the equator and the reverse of the other above it. In [banded-unlink diagram](../../../knot-theory.md#banded-unlink-diagram) language, draw their common unlink and include the two ribbon bands, one from each presentation. Reading the movie from bottom to top gives the indicated birth level, the two saddle bands, and the death level. The resulting surface is knotted: the two-band movie is the standard presentation obtained by gluing the two Stevedore ribbon disks, and a van Kampen calculation retains a noncyclic quotient coming from the trefoil group, whereas the complement of the unknotted model has cyclic fundamental group.

There is a terminology issue in the question. If “2-knot” means an embedded $S^2$, as it normally does, one minimum, two index-one saddles, and one maximum have Euler characteristic

$$
1-2+1=0,
$$

so the resulting orientable [surface knot](../../../knot-theory.md#surface-knot) is a torus, not a two-sphere. The construction above answers the question under the broader usage in which “2-knot” means a connected knotted surface. Under the standard narrow definition, the requested critical-point data are impossible.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Let $D\subset B^4$ be a [slice disk](../../../knot-theory.md#slice-disk) for $K$. Its normal bundle is trivial. A small normal push-off $D'$ is disjoint from $D$, and its boundary is the zero-framed [Seifert longitude](../../../knot-theory.md#seifert-longitude) $\nu_K$. Hence the two-component link $K_{2,0}=K\cup\nu_K$ bounds the pair of disjoint disks $D\cup D'$.

Orient $D'$ oppositely to $D$. In the other hemisphere of $S^4$, join their boundary circles by the product annulus supplied by the zero framing. The union

$$
D\cup (K\times[0,1])\cup D'
$$

is a two-sphere. More concretely, it is the rounded boundary of the three-ball $D\times[-\varepsilon,\varepsilon]$, so it is unknotted. Its equatorial intersection is $K\cup\nu_K$, and both link components lie on the same sphere. Thus $K_{2,0}$ is doubly slice as a [colored link](../../../knot-theory.md#colored-link) with the trivial coloring.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
