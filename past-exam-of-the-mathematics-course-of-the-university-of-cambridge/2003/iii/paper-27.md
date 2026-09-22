# Paper 27

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper27.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper27.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [cellular approximation theorem](../../../algebraic-topology.md#cellular-approximation-theorem) says that a [continuous map](../../../topology.md#continuous-map) between [CW complexes](../../../algebraic-topology.md#cw-complex) is [homotopic](../../../algebraic-topology.md#homotopy) to a [cellular map](../../../algebraic-topology.md#cellular-map), meaning that it sends each $q$-skeleton into the target's $q$-skeleton. Give $S^n$, for $n>0$, its [CW complex](../../../algebraic-topology.md#cw-complex) structure with one zero-cell and one $n$-cell. Its $n$-skeleton is the whole sphere, so the theorem applies and gives the requested result. For $n=0$ use the two zero-cells of $S^0$. In particular the conclusion is

$$
\boxed{f\simeq g,\qquad g(S^n)\subseteq X_n.}
$$

There is no local-finiteness assumption on $X$.

For completeness, here is a direct proof of the needed case of [cellular approximation](../../../algebraic-topology.md#cellular-approximation-theorem), including the point-avoidance step. We use three standard facts, stated explicitly. First, a [compact subset](../../../topology.md#compact-space) of a [CW complex](../../../algebraic-topology.md#cw-complex) lies in a finite subcomplex. Second, a [continuous map](../../../topology.md#continuous-map) from a [smooth manifold](../../../differential-geometry.md#smooth-manifold) into Euclidean space has arbitrarily close smooth approximations, and smooth cutoffs exist around compact subsets of open sets. Third, the [Sard theorem](../../../differential-geometry.md#sard-s-theorem) says the critical values of a smooth map have measure zero; when the domain dimension is smaller than the target dimension, its entire image has measure zero.

The first fact has a useful short proof. If a compact set met infinitely many open cells, choose one point in each of countably many distinct cells. Closure-finiteness makes every closed cell meet the chosen set, and every subset of it, in finitely many points. The weak topology of a [CW complex](../../../algebraic-topology.md#cw-complex) then makes all those subsets closed. The chosen set is an infinite closed discrete subset of a compact space, a contradiction. Taking the closures of the finitely many cells met proves the claim.

Now $f(S^n)$ lies in a finite subcomplex $Y$. Take a top-dimensional open cell $e^d$ of $Y$ with $d>n$, and identify its interior with the open unit ball in $\mathbb R^d$ using its characteristic map. On the open set $U=f^{-1}(e^d)$, write $F:U\to B^d$ for the coordinate expression. Choose $0<r'<r''<1$ and a smooth cutoff $\chi$ supported in $F^{-1}(B_{r''})$ and equal to one near the compact set $F^{-1}(\overline B_{r'})$. By [smooth approximation of maps into Euclidean space](../../../differential-geometry.md#smooth-approximation-of-maps-into-euclidean-space), choose a smooth $h:U\to\mathbb R^d$ with $|h-F|<\delta$, where $\delta<\min(r'/2,1-r'')$. Replace $F$ by

$$
G=F+\chi(h-F).
$$

The straight-line interpolation is a [homotopy](../../../algebraic-topology.md#homotopy) supported away from the boundary of the cell and stays inside that cell. Where $\chi\ne1$, we have $|F|>r'$ and hence $|G|>r'/2$. By the [Sard theorem](../../../differential-geometry.md#sard-s-theorem), choose $z\in B_{r'/4}$ outside $h(U)$. Where $\chi=1$ we have $G=h$, and elsewhere $|G|>r'/2$, so the modified map avoids $z$ everywhere.

Radial retraction of $D^d\setminus\{z\}$ onto its boundary fixes that boundary. It therefore descends through the characteristic map, including its possibly noninjective boundary identifications, and fixes all other cells of $Y$. Composing gives a [homotopy](../../../algebraic-topology.md#homotopy) whose endpoint misses all of $e^d$. Remove every cell of dimension greater than $n$ in descending order. There are finitely many such cells, so their homotopies concatenate to yield $g:S^n\to Y^n\subseteq X_n$. This proves [dimension reduction of sphere maps into CW skeleta](../../../algebraic-topology.md#dimension-reduction-of-sphere-maps-into-cw-skeleta). The approximation step is essential: an arbitrary continuous image of $S^n$ can fill a higher-dimensional region, so dimension alone would not supply an omitted point.

## 2

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [Morse lemma](../../../differential-geometry.md#morse-lemma) states that if $p$ is a [nondegenerate critical point](../../../calculus.md#nondegenerate-critical-point) of a smooth real function $f$ on an $m$-dimensional [smooth manifold](../../../differential-geometry.md#smooth-manifold), there are smooth coordinates $y_1,\ldots,y_m$, centered at $p$, such that

$$
\boxed{f(y)=f(p)-\sum_{i=1}^{\lambda}y_i^2+\sum_{i=\lambda+1}^m y_i^2.}
$$

Here $\lambda$ is the [Morse index](../../../differential-geometry.md#morse-index), the number of negative directions of the [Hessian matrix](../../../calculus.md#hessian-matrix) at $p$. The equality is exact on a neighborhood, not merely a second-order expansion.

To prove it, start with any coordinates putting $p=0$. Since $df(0)=0$, integral [Taylor theorem](../../../calculus.md#taylor-theorem) gives

$$
f(x)-f(0)=\sum_{i,j=1}^m a_{ij}(x)x_ix_j,\qquad a_{ij}(x)=\int_0^1(1-t)\,\partial_i\partial_jf(tx)\,dt.
$$

The [matrix](../../../vector-space.md#matrix) $A(x)=(a_{ij}(x))$ is smooth and symmetric, with $A(0)=\tfrac12\operatorname{Hess}f(0)$. By [Sylvester's law of inertia](../../../linear-algebra.md#sylvester-s-law-of-inertia), a constant invertible linear coordinate change makes $A(0)=\operatorname{diag}(-I_\lambda,I_{m-\lambda})$.

We perform completion of squares with coefficients depending smoothly on the original $x$. The first pivot $a_{11}(x)$ stays nonzero and keeps its sign on a sufficiently small neighborhood. Algebraically,

$$
x^TA(x)x=a_{11}(x)\left(x_1+\sum_{j>1}\frac{a_{1j}(x)}{a_{11}(x)}x_j\right)^2+\sum_{i,j>1}\left(a_{ij}(x)-\frac{a_{i1}(x)a_{1j}(x)}{a_{11}(x)}\right)x_ix_j.
$$

The remaining coefficient matrix is the [Schur complement](../../../linear-algebra.md#schur-complement). At zero it is the remaining signed diagonal matrix, so its first pivot is also nonzero nearby. Continue recursively, shrinking the neighborhood finitely many times. Every pivot $d_i(x)$ is smooth and nonzero, with sign $\epsilon_i=-1$ for $i\leq\lambda$ and $+1$ thereafter. Absorb $|d_i(x)|$ into the square by its smooth positive square root. This produces a smooth triangular matrix $B(x)$ with nonzero diagonal such that

$$
x^TA(x)x=\sum_i\epsilon_i\bigl(B(x)x\bigr)_i^2.
$$

All coefficients here are functions of the original $x$; no circular coordinate substitution is involved. Define $\Phi(x)=B(x)x$. Its derivative at zero is $D\Phi(0)=B(0)$, which is invertible. The [inverse function theorem](../../../calculus.md#inverse-function-theorem) makes $y=\Phi(x)$ a smooth coordinate system and gives the asserted exact quadratic form. The number of negative squares agrees with the [Hessian matrix](../../../calculus.md#hessian-matrix) signature and hence with the [Morse index](../../../differential-geometry.md#morse-index). This is the [smooth completing-square proof of the Morse lemma](../../../differential-geometry.md#smooth-completing-square-proof-of-the-morse-lemma).

## 3

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [Morse function](../../../differential-geometry.md#morse-function) is a smooth real-valued function all of whose [critical points](../../../analysis.md#critical-point) have nonsingular [Hessian matrices](../../../calculus.md#hessian-matrix). We use the descending convention for a [gradient-like vector field](../../../differential-geometry.md#gradient-like-vector-field) $V$: away from critical points, $df(V)<0$, and near a critical point of [Morse index](../../../differential-geometry.md#morse-index) $\lambda$, in [Morse lemma](../../../differential-geometry.md#morse-lemma) coordinates $f=f(p)-|u|^2+|v|^2$, the field can be chosen as $V=(2u,-2v)$.

For its flow $\phi_t$, define the [unstable manifold](../../../dynamical-systems.md#unstable-manifold) $W^u(p)=\{x:\lim_{t\to-\infty}\phi_t(x)=p\}$ and the [stable manifold](../../../dynamical-systems.md#stable-manifold) $W^s(q)=\{x:\lim_{t\to+\infty}\phi_t(x)=q\}$. Their dimensions are $\operatorname{ind}p$ and $m-\operatorname{ind}q$. The [Morse-Smale transversality condition](../../../analysis.md#morse-smale-gradient-flow) is

$$
T_xW^u(p)+T_xW^s(q)=T_xM\quad\text{for every }x\in W^u(p)\cap W^s(q).
$$

For a closed [manifold](../../../topology.md#topological-manifold), this lets us form the [Morse-Smale complex](../../../differential-geometry.md#morse-smale-complex) over $\mathbb Z$. Orient each unstable manifold and take

$$
C_j=\bigoplus_{\operatorname{ind}p=j}\mathbb Zp,\qquad \partial p=\sum_{\operatorname{ind}q=j-1}n(p,q)q.
$$

The transverse intersection for an index difference of one is one-dimensional; quotienting by flow time gives a finite set of trajectories, and $n(p,q)$ counts them with orientation signs. Compactifying the one-dimensional spaces of trajectories for an index difference of two adds broken trajectories. Their oriented boundary count is zero, giving $\partial^2=0$. The descending cells are the unstable manifolds, and these counts are the incidence numbers of the corresponding [cellular chain complex](../../../homology.md#cellular-chain-complex), so **the homology of this complex is $H_*(M;\mathbb Z)$**. Ambient orientability is unnecessary: orientations of the unstable cells provide the requisite coorientations and trajectory signs.

For the [Klein bottle](../../../topology.md#klein-bottle), use the quotient of $\mathbb R^2$ by $(s,t)\sim(s+2\pi,-t)$ and $(s,t)\sim(s,t+2\pi)$. A model of the standard four-critical-point height function is

$$
f(s,t)=\cos s+\varepsilon\cos t,\qquad0<\varepsilon<1.
$$

It is well defined under both identifications. Its [critical points](../../../analysis.md#critical-point), their [Morse indices](../../../differential-geometry.md#morse-index), and critical values are

$$
\begin{array}{c|c|c}
\text{point}&\text{index}&f\\\hline
m=(\pi,\pi)&0&-1-\varepsilon\\
b=(\pi,0)&1&-1+\varepsilon\\
a=(0,\pi)&1&1-\varepsilon\\
q=(0,0)&2&1+\varepsilon.
\end{array}
$$

The [Hessian matrix](../../../calculus.md#hessian-matrix) is diagonal with entries $-\cos s$ and $-\varepsilon\cos t$, so each point is nondegenerate. The flat quotient metric gives descending equations $\dot s=\sin s$, $\dot t=\varepsilon\sin t$. Their saddle separatrices are the coordinate lines; the two saddle-to-saddle intersections are empty, and all remaining stable and unstable intersections are transverse. This is a [Morse-Smale gradient flow](../../../analysis.md#morse-smale-gradient-flow). If one insists on the exact local-model version of a [gradient-like vector field](../../../differential-geometry.md#gradient-like-vector-field) above, change the two coordinate speeds near the critical points to the standard quadratic-model speeds. This preserves the separatrices, signs and transversality.

Both branches of either saddle flow to the minimum with opposite endpoint signs, so $\partial a=\partial b=0$. From the maximum to $a$, the two trajectories lie on $s=0$ and approach $t=\pi$ from opposite directions. The identification in $t$ is a translation, so their incidence signs are opposite and cancel. The two trajectories to $b$ lie on $t=0$ and approach $s=\pi$ from opposite directions. The identification in $s$ reverses the transverse $t$-coordinate, reversing one additional orientation sign. These two contributions consequently have the same sign. Choosing the orientation of $b$ gives $\partial q=2b$.

One can check the coefficient directly from the [cell attachment](../../../algebraic-topology.md#cell-attachment) of the top cell: its boundary word is $aba^{-1}b$, with exponent sums zero on the base loop $a$ and two on the fiber loop $b$. Thus the [integral Morse complex of the Klein bottle](../../../differential-geometry.md#integral-morse-complex-of-the-klein-bottle) is

$$
0\longrightarrow\mathbb Zq\xrightarrow{\binom{0}{2}}\mathbb Za\oplus\mathbb Zb\xrightarrow{0}\mathbb Zm\longrightarrow0,
$$

and

$$
\boxed{H_0(K;\mathbb Z)=\mathbb Z,\quad H_1(K;\mathbb Z)=\mathbb Z\oplus\mathbb Z/2,\quad H_2(K;\mathbb Z)=0.}
$$

Counting trajectories without signs, or working only modulo two, would miss the order-two class.

## 4

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Work over $\mathbb Q$. A closed connected [orientable surface](../../../differential-geometry.md#orientable-surface) of [genus](../../../topology.md#genus-of-a-surface) $g$ has [Betti numbers](../../../homology.md#betti-number) $(1,2g,1)$; the [circle](../../../topology.md#circle) has Betti numbers $(1,1)$. The [Künneth theorem](../../../cohomology.md#kunneth-theorem) therefore gives

$$
(b_0,b_1,b_2,b_3)(S^1\times\Sigma_g)=(1,2g+1,2g+1,1).
$$

We use the following precise consequence of the [Morse handle-attachment theorem](../../../differential-geometry.md#morse-handle-attachment-theorem): a closed [manifold](../../../topology.md#topological-manifold) with a [Morse function](../../../differential-geometry.md#morse-function) has the [homotopy type](../../../algebraic-topology.md#homotopy-type) of a finite [CW complex](../../../algebraic-topology.md#cw-complex) with one index-$j$ cell for each index-$j$ [critical point](../../../analysis.md#critical-point). Its degree-$j$ rational [cellular chain group](../../../homology.md#cellular-chain-group) has dimension $c_j$, so its [homology](../../../homology.md) has dimension at most $c_j$. Consequently $c_j\geq b_j$, the weak [Morse inequalities](../../../differential-geometry.md#morse-inequalities). Summing yields

$$
\boxed{\#\operatorname{Crit}(f)\geq1+(2g+1)+(2g+1)+1=4g+4.}
$$

This counts every critical point, regardless of whether some critical values coincide.

To attain the bound, construct a surface [Morse function](../../../differential-geometry.md#morse-function) $h:\Sigma_g\to\mathbb R$ from the standard orientable [handle decomposition](../../../topology.md#handle-decomposition): start with a disk, attach $2g$ orientable bands in the usual paired pattern forming the genus-$g$ surface with one boundary component, and cap that boundary with a disk. Give the first disk a minimum, each band one saddle with local form $-x^2+y^2$, and the final cap a maximum. Regular collar coordinates join successive levels without additional critical points. This constructs $h$ with counts $(1,2g,1)$.

On the product take

$$
F(\theta,x)=h(x)+\delta\cos\theta,\qquad\delta>0.
$$

Its [critical points](../../../analysis.md#critical-point) are exactly the pairs of a critical point of $h$ with $\theta=0,\pi$. The [Hessian matrix](../../../calculus.md#hessian-matrix) is block diagonal, with surface block $\operatorname{Hess}h$ and circle entry $-\delta\cos\theta$. It is nonsingular and its [Morse index](../../../differential-geometry.md#morse-index) is the sum of the two factor indices. Thus this [product of Morse functions](../../../differential-geometry.md#product-of-morse-functions) has counts

$$
(c_0,c_1,c_2,c_3)=(1,2g+1,2g+1,1),
$$

and exactly **$4g+4$ critical points**. If distinct critical values are desired, choose $\delta$ outside the finite set producing collisions after first choosing distinct critical values for $h$. The [minimal Morse critical count on a circle times an orientable surface](../../../differential-geometry.md#minimal-morse-critical-count-on-a-circle-times-an-orientable-surface) is therefore attained for every $g\geq0$.

## 5

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Here projection means [Hermitian](../../../hilbert-space.md#hermitian-operator) [orthogonal projection](../../../hilbert-space.md#orthogonal-projection): $P=P^*=P^2$ with $\operatorname{tr}P=k$, as indicated by the unitary conjugation in the question. These matrices represent the [complex Grassmannian as orthogonal projections](../../../differential-geometry.md#complex-grassmannian-as-orthogonal-projections), a compact manifold of complex dimension $k(n-k)$. The constants $c_i$ are real. Let $A^*=-A$ and use the given tangent directions $[A,P]$. Cyclicity of the [matrix trace](../../../linear-algebra.md#matrix-trace) gives

$$
df_P([A,P])=\operatorname{tr}(C[A,P])=\operatorname{tr}([P,C]A).
$$

The [commutator](../../../lie-algebra.md#commutator) $B=[P,C]$ is skew-Hermitian. If this derivative vanishes for every skew-Hermitian $A$, choose $A=B$ to obtain

$$
0=\operatorname{tr}(B^2)=-\operatorname{tr}(B^*B),
$$

so $B=0$. Conversely $[P,C]=0$ makes every tangent derivative zero. Because the diagonal entries of $C$ are distinct, a commuting [matrix](../../../vector-space.md#matrix) $P$ is diagonal. Its idempotent entries are zero or one. Thus the critical projections are exactly

$$
\boxed{P_I=\operatorname{diag}(\mathbf1_{1\in I},\ldots,\mathbf1_{n\in I}),\qquad |I|=k,}
$$

with $\binom nk$ [critical points](../../../analysis.md#critical-point) and values $f(P_I)=\sum_{i\in I}c_i$.

To compute the [Hessian matrix](../../../calculus.md#hessian-matrix), write $E=\operatorname{span}\{e_i:i\in I\}$ and $E^\perp=\operatorname{span}\{e_j:j\notin I\}$. A neighboring plane is the graph of a complex [linear map](../../../vector-space.md#linear-map) $Z:E\to E^\perp$. With $W=\binom I Z$, its orthogonal projection is $P(Z)=W(I+Z^*Z)^{-1}W^*$. Writing $C_E,C_{E^\perp}$ for the diagonal blocks, we get

$$
f(P(Z))=\operatorname{tr}\bigl(C_E(I+Z^*Z)^{-1}\bigr)+\operatorname{tr}\bigl(C_{E^\perp}Z(I+Z^*Z)^{-1}Z^*\bigr).
$$

Expanding $(I+Z^*Z)^{-1}=I-Z^*Z+O(\|Z\|^4)$ yields

$$
f(P(Z))=f(P_I)+\sum_{i\in I,\ j\notin I}(c_j-c_i)|z_{ji}|^2+O(\|Z\|^4).
$$

Each complex coordinate has two real components, each with Hessian coefficient $2(c_j-c_i)$. Every coefficient is nonzero, proving that $f$ is a [Morse function](../../../differential-geometry.md#morse-function). Its negative directions correspond to $j<i$. For $I=\{i_1<\cdots<i_k\}$ there are $i_a-a$ complementary indices below $i_a$, giving

$$
\boxed{\operatorname{ind}(P_I)=2\#\{(i,j):i\in I,\ j\notin I,\ j<i\}=2\sum_{a=1}^k(i_a-a).}
$$

This is the [diagonal trace Morse function on a complex Grassmannian](../../../differential-geometry.md#diagonal-trace-morse-function-on-a-complex-grassmannian). Its critical values need not be distinct; ties between sums do not make its critical points degenerate.

All [Morse indices](../../../differential-geometry.md#morse-index) are even. Choose a [Morse-Smale gradient flow](../../../analysis.md#morse-smale-gradient-flow) and form its integral [Morse chain complex](../../../differential-geometry.md#morse-chain-complex). The odd-degree chain groups vanish, so every differential vanishes. Equivalently the [Morse handle-attachment theorem](../../../differential-geometry.md#morse-handle-attachment-theorem) supplies only even-dimensional cells. The [integral homology of complex Grassmannians](../../../differential-geometry.md#integral-homology-of-complex-grassmannians) is therefore

$$
\boxed{H_{2r}(\operatorname{Gr}(k,n);\mathbb Z)=\mathbb Z^{N_r},\quad H_{2r+1}(\operatorname{Gr}(k,n);\mathbb Z)=0,}
$$

where $N_r$ counts the subsets with $\sum_a(i_a-a)=r$, and $0\leq r\leq k(n-k)$. In particular there is no torsion. The nondecreasing sequence $i_a-a$ lies between zero and $n-k$, so reversing it identifies these subsets with [partitions of an integer](../../../representation-theory-of-the-symmetric-group.md#partition-of-an-integer) $r$ fitting in a $k$ by $(n-k)$ rectangle. The [Poincaré polynomial](../../../homology.md#poincare-polynomial) is explicitly

$$
\sum_{|I|=k}t^{2\sum_a(i_a-a)}.
$$

For the permitted example $\operatorname{Gr}(2,4)$, the subsets $12,13,14,23,24,34$ have indices $0,2,4,4,6,8$. Thus

$$
\boxed{H_0=H_2=H_6=H_8=\mathbb Z,\quad H_4=\mathbb Z^2,\quad H_{\mathrm{odd}}=0.}
$$

The general calculation above applies throughout $2\leq k\leq n-2$; it does not reduce to any of the excluded rank-one cases.

## 6

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

An index-$\lambda$ [handle](../../../topology.md#handle) in dimension $d$ is $D^\lambda\times D^{d-\lambda}$. A [handle attachment](../../../topology.md#handle-attachment) glues its attaching region $S^{\lambda-1}\times D^{d-\lambda}$ to a corresponding neighborhood in the boundary of the preceding [manifold with boundary](../../../differential-geometry.md#manifold-with-boundary). Besides the embedding of the [attaching sphere](../../../topology.md#attaching-sphere), one specifies a [framing of an embedded sphere](../../../algebraic-geometry.md#framing-of-an-embedded-sphere), namely the normal-disk directions used in this gluing. Corners are then smoothed.

In dimension four, a [two-handle](../../../topology.md#two-handle) is $D^2\times D^2$ and attaches along $S^1\times D^2$. Its attaching circle is a [knot](../../../knot-theory.md#knot) in the boundary of the [zero-handle](../../../topology.md#zero-handle) $D^4$. Identify that boundary with $S^3$ and remove a point away from the circles to draw them in $\mathbb R^3$. Disjoint attaching circles give a [framed link](../../../knot-theory.md#framed-link). Each integer records the twist of its normal framing relative to the zero [Seifert framing](../../../knot-theory.md#seifert-framing); the integer is also the [linking number](../../../knot-theory.md#linking-number) of the circle and its framed push-off. The resulting boundary change is [Dehn surgery on a framed link](../../../knot-theory.md#dehn-surgery-on-a-framed-link). This is the two-handle part of a [Kirby diagram](../../../knot-theory.md#kirby-diagram).

For $S^2\times S^2$, use the following explicit [handle decomposition](../../../topology.md#handle-decomposition). Write each factor as two disks, $S^2=D_-^2\cup D_+^2$, glued along their boundary circles. The four product pieces give

$$
h^0=D_-^2\times D_-^2,\qquad h^2_1=D_+^2\times D_-^2,\qquad h^2_2=D_-^2\times D_+^2,\qquad h^4=D_+^2\times D_+^2.
$$

The first is a four-dimensional [zero-handle](../../../topology.md#zero-handle) after rounding its corners. Its boundary is the union of the solid tori $S^1\times D^2$ and $D^2\times S^1$. The two middle product pieces attach along these tori. Their attaching circles $S^1\times\{0\}$ and $\{0\}\times S^1$ form the standard [Hopf link](../../../knot-theory.md#hopf-link), with [linking number](../../../knot-theory.md#linking-number) one after choosing orientations.

Both framings are zero. For example, the normal disk of $S^1\times\{0\}$ is the second disk factor. Its constant normal push-off has linking number zero with the original circle: the circle bounds $D^2\times\{0\}$ in the four-ball, and a parallel push-off bounds a disjoint translated disk. Thus the framed self-intersection is zero; the same argument applies with the factors interchanged. These product framings are the zero [Seifert framings](../../../knot-theory.md#seifert-framing).

<a id="6/image-zero-framed-hopf-link-for-the-two-two-handles-of-s2-times-s2-the-upper-crossing-has-blue-over-orange-and-the-lower-crossing-has-orange-over-blue"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-27-hopf.png)

**[Figure 1](#6/image-zero-framed-hopf-link-for-the-two-two-handles-of-s2-times-s2-the-upper-crossing-has-blue-over-orange-and-the-lower-crossing-has-orange-over-blue). Zero-framed Hopf link for the two two-handles of S2 times S2; the upper crossing has blue over orange and the lower crossing has orange over blue**.

After these two [two-handles](../../../topology.md#two-handle), the remaining product piece $D_+^2\times D_+^2$ is a four-ball. Its boundary is exactly the boundary of the assembled first three pieces, so it attaches as a [four-handle](../../../topology.md#four-handle). Equivalently, [zero surgery on the Hopf link](../../../knot-theory.md#zero-surgery-on-the-hopf-link) gives $S^3$, which this handle caps. We have therefore constructed the actual product, proving

$$
\boxed{S^2\times S^2=\text{one zero-handle}+\text{two zero-framed Hopf-linked two-handles}+\text{one four-handle}.}
$$

There are no one- or three-handles. As a check, the two factor spheres have self-intersection zero and meet once, giving the [intersection form](../../../homology.md#intersection-form) $\left(\begin{smallmatrix}0&1\\1&0\end{smallmatrix}\right)$. The explicit product construction, rather than the intersection form alone, identifies the smooth four-manifold. This is the [zero-framed Hopf-link handle decomposition of the sphere product](../../../topology.md#zero-framed-hopf-link-handle-decomposition-of-the-sphere-product).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
