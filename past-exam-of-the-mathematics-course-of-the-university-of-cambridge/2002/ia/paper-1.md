# Paper 1

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2002/PaperIA_1.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2002/PaperIA_1.pdf)

**Table of contents**

- [Section I](#section-i)
  - [1B](#1b)
    - [a](#1b/a)
      - [Solution](#1b/a/solution)
    - [b](#1b/b)
      - [Solution](#1b/b/solution)
  - [2D](#2d)
    - [Solution](#2d/solution)
  - [3C](#3c)
    - [Solution](#3c/solution)
  - [4C](#4c)
    - [Solution](#4c/solution)
- [Section II](#section-ii)
  - [5B](#5b)
    - [a](#5b/a)
      - [Solution](#5b/a/solution)
    - [b](#5b/b)
      - [Solution](#5b/b/solution)
  - [6B](#6b)
    - [a](#6b/a)
      - [Solution](#6b/a/solution)
    - [b](#6b/b)
      - [Solution](#6b/b/solution)
  - [7B](#7b)
    - [a](#7b/a)
      - [Solution](#7b/a/solution)
    - [b](#7b/b)
      - [Solution](#7b/b/solution)
  - [8D](#8d)
    - [Solution](#8d/solution)
  - [9C](#9c)
    - [Solution](#9c/solution)
    - [i](#9c/i)
      - [Solution](#9c/i/solution)
    - [ii](#9c/ii)
      - [Solution](#9c/ii/solution)
    - [iii](#9c/iii)
      - [Solution](#9c/iii/solution)
    - [iv](#9c/iv)
      - [Solution](#9c/iv/solution)
  - [10C](#10c)
    - [Solution](#10c/solution)
    - [i](#10c/i)
      - [Solution](#10c/i/solution)
    - [ii](#10c/ii)
      - [Solution](#10c/ii/solution)
    - [iii](#10c/iii)
      - [Solution](#10c/iii/solution)
    - [iv](#10c/iv)
      - [Solution](#10c/iv/solution)
  - [11C](#11c)
    - [Solution](#11c/solution)
  - [12C](#12c)
    - [Solution](#12c/solution)

## Section I

↑ **Parent:** [Paper 1](paper-1.md)

### 1B

↑ **Parent:** [Section I](#section-i)

<h4 id="1b/a">a</h4>

↑ **Parent:** [1B](#1b)

<h5 id="1b/a/solution">Solution</h5>

↑ **Parent:** [A](#1b/a)

For a finite [group](../../../group.md) $G$ acting on a [set](../../../set.md) $X$, write $G_x=\{g\in G:gx=x\}$ for the [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup) and $Gx=\{gx:g\in G\}$ for the [orbit](../../../dynamical-systems.md#orbit-dynamical-system) of $x$. The [orbit-stabilizer theorem](../../../group-theory.md#orbit-stabilizer-theorem) gives

$$
\boxed{|G|=|G_x|\,|Gx|.}
$$

Indeed, $gG_x\mapsto gx$ is a [bijection](../../../function.md#bijection) from the left [cosets](../../../group-theory.md#coset) of $G_x$ onto $Gx$: two images agree precisely when $h^{-1}g\in G_x$. Each [coset](../../../group-theory.md#coset) has $|G_x|$ elements, proving the formula.

<h4 id="1b/b">b</h4>

↑ **Parent:** [1B](#1b)

<h5 id="1b/b/solution">Solution</h5>

↑ **Parent:** [B](#1b/b)

Place the cube vertices at $(\pm1,\pm1,\pm1)$. The four vertices whose coordinate product is $+1$ form $T$; those with product $-1$ form $T'$. Within either [set](../../../set.md), two distinct vertices differ in exactly two coordinates, so every edge has length $2\sqrt2$ and each [set](../../../set.md) is a [regular tetrahedron](../../../geometry-and-topology.md#regular-tetrahedron).

A member of the [cube rotation group](../../../group-theory.md#rotational-symmetry-group-of-a-cube) is a [signed permutation matrix](../../../vector-space.md#signed-permutation-matrix) of [determinant](../../../linear-algebra.md#determinant) one. There are $3!$ permutations of the coordinate axes and four choices of signs for each permutation that give [determinant](../../../linear-algebra.md#determinant) one, so $|G|=24$. Such a [matrix](../../../vector-space.md#matrix) maps a coordinate-product class to a coordinate-product class. Moreover, the [rotation](../../../riemannian-geometry.md#rotation-mathematics) through a quarter-turn $(x,y,z)\mapsto(-y,x,z)$ interchanges the classes. Thus the [orbit](../../../dynamical-systems.md#orbit-dynamical-system) of $T$ consists of exactly $T,T'$. By the [orbit-stabilizer theorem](../../../group-theory.md#orbit-stabilizer-theorem), the [tetrahedron stabilizer in the cube rotation group](../../../group-theory.md#tetrahedron-stabilizer-in-the-cube-rotation-group) has order

$$
\boxed{|G_T|=24/2=12.}
$$

### 2D

↑ **Parent:** [Section I](#section-i)

<h4 id="2d/solution">Solution</h4>

↑ **Parent:** [2D](#2d)

The [fundamental theorem of algebra](../../../algebra.md#fundamental-theorem-of-algebra) says that every nonconstant [polynomial](../../../polynomial.md) with [complex number](../../../complex-analysis.md#complex-number) coefficients has a root in the [complex numbers](../../../complex-analysis.md#complex-number). Repeated [polynomial division](../../../polynomial.md#polynomial-division) by a factor of degree one therefore factors a degree-three [polynomial](../../../polynomial.md) with [complex number](../../../complex-analysis.md#complex-number) coefficients into three factors of degree one, with [algebraic multiplicities](../../../linear-operator-theory.md#algebraic-multiplicity) included.

For a [matrix](../../../vector-space.md#matrix) with [complex number](../../../complex-analysis.md#complex-number) entries $A$ of size three, its [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) is $\chi_A(t)=\det(tI-A)$, and its characteristic equation is $\chi_A(t)=0$. A [complex number](../../../complex-analysis.md#complex-number) $\lambda$ is an [eigenvalue](../../../linear-operator-theory.md#eigenvalue) exactly when $\lambda I-A$ is singular, equivalently when its [null space](../../../linear-algebra.md#kernel-of-a-linear-map) contains a nonzero [vector](../../../vector-space.md#vector). Thus the three roots of the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) are the three [eigenvalues](../../../linear-operator-theory.md#eigenvalue) counted with [algebraic multiplicity](../../../linear-operator-theory.md#algebraic-multiplicity).

For the specified [matrix](../../../vector-space.md#matrix), expansion along the first row gives

$$
\chi_A(t)=(t-1)\det\begin{pmatrix}t&-i\\i&t\end{pmatrix}
=(t-1)(t^2-1)=(t-1)^2(t+1).
$$

Hence **the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $1,1,-1$**. Corresponding [eigenvectors](../../../linear-operator-theory.md#eigenvector) are

$$
v_1=\begin{pmatrix}1\\0\\0\end{pmatrix},\qquad
v_2=\begin{pmatrix}0\\i\\1\end{pmatrix},\qquad
v_3=\begin{pmatrix}0\\-i\\1\end{pmatrix},
\qquad Av_1=v_1,\quad Av_2=v_2,\quad Av_3=-v_3.
$$

The [matrix](../../../vector-space.md#matrix) with these three columns has [determinant](../../../linear-algebra.md#determinant) $2i\ne0$, so these [eigenvectors](../../../linear-operator-theory.md#eigenvector) are [linearly independent](../../../vector-space.md#linear-independence). A repeated [eigenvalue](../../../linear-operator-theory.md#eigenvalue) does not in general guarantee two independent [eigenvectors](../../../linear-operator-theory.md#eigenvector); here they have been exhibited directly.

### 3C

↑ **Parent:** [Section I](#section-i)

<h4 id="3c/solution">Solution</h4>

↑ **Parent:** [3C](#3c)

The [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence) of [real numbers](../../../arithmetic.md#real-number) is $a$ if, for every $\varepsilon>0$, there is an [integer](../../../number-theory.md#integer) $N$ such that $n\ge N$ implies $|a_n-a|<\varepsilon$. It tends to positive infinity if, for every real $M$, there is an [integer](../../../number-theory.md#integer) $N$ such that $n\ge N$ implies $a_n>M$.

If $a_n\to+\infty$, choose the latter threshold with $M=1/\varepsilon$. Then $a_n>1/\varepsilon>0$ eventually, so $|1/a_n|<\varepsilon$. Thus $1/a_n\to0$. **The converse is false:** $a_n=-n$ has reciprocal tending to zero and tends to negative infinity. The precise sign-free statement is given by [reciprocal limits and escape in absolute value](../../../real-analysis.md#reciprocal-limits-and-escape-in-absolute-value): $1/a_n\to0$ is equivalent to $|a_n|\to\infty$.

If $a_n\to a\ne0$, eventually $|a_n-a|<|a|/2$, and the [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives $|a_n|>|a|/2$. Consequently

$$
\left|\frac1{a_n}-\frac1a\right|
=\frac{|a_n-a|}{|a_n||a|}\le\frac{2|a_n-a|}{|a|^2}.
$$

Given $\varepsilon>0$, take $N$ large enough that $|a_n-a|<\min(|a|/2,\varepsilon|a|^2/2)$ for all $n\ge N$. This proves **$1/a_n\to1/a$** directly from the definition of the [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence).

### 4C

↑ **Parent:** [Section I](#section-i)

<h4 id="4c/solution">Solution</h4>

↑ **Parent:** [4C](#4c)

Here is a nested-interval proof of the [Bolzano-Weierstrass theorem](../../../real-analysis.md#bolzano-weierstrass-theorem). Put every term of the bounded real [sequence](../../../real-analysis.md#sequence) in a [closed interval](../../../real-analysis.md#closed-real-interval) $I_0=[-M,M]$, with $M>0$. Bisect this interval and choose a closed half containing infinitely many terms. Repeating gives nested [closed intervals](../../../real-analysis.md#closed-real-interval) $I_j=[l_j,r_j]$, each containing infinitely many [sequence](../../../real-analysis.md#sequence) terms, with length $2M/2^j$.

By the [least-upper-bound property](../../../real-analysis.md#least-upper-bound-property), $x_* =\sup_j l_j$ exists. For each $j$, every lower endpoint lies at most $r_j$, while $l_j\le x_*$; hence $x_*\in I_j$. Choose increasing indices $n_j$ with $a_{n_j}\in I_j$, possible because each interval contains infinitely many terms. Then

$$
|a_{n_j}-x_*|\le 2M/2^j\longrightarrow0.
$$

Thus **every bounded real [sequence](../../../real-analysis.md#sequence) has a [convergent subsequence](../../../real-analysis.md#convergent-subsequence)**.

For a [sequence](../../../real-analysis.md#sequence) with no [convergent subsequence](../../../real-analysis.md#convergent-subsequence), take $a_n=n$: any [subsequence](../../../real-analysis.md#subsequence) has $n_j\ge j$, so its terms tend to positive infinity rather than to a finite [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence). For an unbounded [sequence](../../../real-analysis.md#sequence) with a [convergent subsequence](../../../real-analysis.md#convergent-subsequence), take $a_{2n}=0$ and $a_{2n-1}=n$. Its odd terms are unbounded, while its even [subsequence](../../../real-analysis.md#subsequence) converges to zero.

## Section II

↑ **Parent:** [Paper 1](paper-1.md)

### 5B

↑ **Parent:** [Section II](#section-ii)

<h4 id="5b/a">a</h4>

↑ **Parent:** [5B](#5b)

<h5 id="5b/a/solution">Solution</h5>

↑ **Parent:** [A](#5b/a)

Take the scalene triangle vertex [set](../../../set.md) $T=\{(0,0),(1,0),(0,2)\}$. Its edge lengths are $1,2,\sqrt5$. Each vertex has a different unordered pair of incident edge lengths. A [Euclidean isometry](../../../riemannian-geometry.md#euclidean-isometry) preserving the [set](../../../set.md) must preserve these pairs, and therefore fixes every vertex.

To justify [rigidity of a scalene triangle](../../../riemannian-geometry.md#rigidity-of-a-scalene-triangle) fully, [Euclidean distances](../../../topological-analysis.md#euclidean-distance) from an arbitrary plane point to these three [fixed points](../../../function.md#fixed-point) determine that point uniquely: subtracting its squared [Euclidean distance](../../../topological-analysis.md#euclidean-distance) to the origin from the other two squared [Euclidean distances](../../../topological-analysis.md#euclidean-distance) determines its two coordinates. Thus an [isometry](../../../riemannian-geometry.md#isometry) fixing the three vertices fixes every plane point. **Only the identity preserves $T$.**

For the general union of [group](../../../group.md) translates, let $h\in G$. Left multiplication by $h$ permutes $G$, so

$$
h(S)=\bigcup_{g\in G}hg(T)=\bigcup_{k\in G}k(T)=S.
$$

Therefore **$G\subseteq H$**. This containment uses only the [group action](../../../group-theory.md#group-action); the absence of symmetries of $T$ is not needed for the containment itself.

<h4 id="5b/b">b</h4>

↑ **Parent:** [5B](#5b)

<h5 id="5b/b/solution">Solution</h5>

↑ **Parent:** [B](#5b/b)

Use the same triangle and let $G$ consist of [translations](../../../geometry-and-topology.md#translation-geometry) $x\mapsto x+m$ for $m\in\mathbb Z^2$. All its vertices have [integer](../../../number-theory.md#integer) coordinates, and one vertex is the origin, so

$$
S=\bigcup_{m\in\mathbb Z^2}(m+T)=\mathbb Z^2.
$$

The [rotation](../../../riemannian-geometry.md#rotation-mathematics) through a quarter-turn $(x,y)\mapsto(-y,x)$ preserves this [integer lattice](../../../geometry-and-topology.md#integer-lattice), and hence belongs to $H$. It fixes the origin and is not the identity, whereas the only [translation](../../../geometry-and-topology.md#translation-geometry) fixing the origin is the identity. It is therefore outside $G$, proving **$G\subsetneq H$**. This is [symmetry enlargement under group translates](../../../group-theory.md#symmetry-enlargement-under-group-translates) even though $T$ itself has trivial [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup).

### 6B

↑ **Parent:** [Section II](#section-ii)

<h4 id="6b/a">a</h4>

↑ **Parent:** [6B](#6b)

<h5 id="6b/a/solution">Solution</h5>

↑ **Parent:** [A](#6b/a)

Write a [Möbius transformation](../../../group-theory.md#mobius-transformation) as $g(z)=(az+b)/(cz+d)$, with $ad-bc\ne0$, on the [Riemann sphere](../../../complex-analysis.md#riemann-sphere). If $c\ne0$, infinity is not fixed, and its finite [fixed points](../../../function.md#fixed-point) solve

$$
cz^2+(d-a)z-b=0.
$$

The pole $-d/c$ cannot solve this equation, since substitution gives $(ad-bc)/c\ne0$. The quadratic has one or two distinct complex roots, so these give exactly one or two [fixed points](../../../function.md#fixed-point).

If $c=0$, then $a,d\ne0$ and infinity is fixed. If $a\ne d$, there is one additional finite [fixed point](../../../function.md#fixed-point), namely $b/(d-a)$. If $a=d$ and $b\ne0$, the transformation is a nonzero [translation](../../../geometry-and-topology.md#translation-geometry), with no finite [fixed point](../../../function.md#fixed-point). If $a=d$ and $b=0$, it is the identity and fixes the entire sphere.

Thus **a nonidentity [Möbius transformation](../../../group-theory.md#mobius-transformation) has one or two [fixed points](../../../function.md#fixed-point); the identity has infinitely many**. The examples $z\mapsto z+1$, $z\mapsto2z$, and $z\mapsto z$ realize the three possibilities respectively.

<h4 id="6b/b">b</h4>

↑ **Parent:** [6B](#6b)

<h5 id="6b/b/solution">Solution</h5>

↑ **Parent:** [B](#6b/b)

[Complex conjugation](../../../complex-analysis.md#complex-conjugation) fixes $0,1,\infty$, but sends $i$ to $-i$, so it is not the identity. The preceding classification of [fixed points of a Möbius transformation](../../../group-theory.md#fixed-point-of-a-mobius-transformation) says that a nonidentity [Möbius transformation](../../../group-theory.md#mobius-transformation) has at most two [fixed points](../../../function.md#fixed-point). Since [complex conjugation](../../../complex-analysis.md#complex-conjugation) has at least three, **it cannot be a [Möbius transformation](../../../group-theory.md#mobius-transformation)**.

### 7B

↑ **Parent:** [Section II](#section-ii)

<h4 id="7b/a">a</h4>

↑ **Parent:** [7B](#7b)

<h5 id="7b/a/solution">Solution</h5>

↑ **Parent:** [A](#7b/a)

Take positive angles counterclockwise. The [rotation](../../../riemannian-geometry.md#rotation-mathematics) sends the [standard basis](../../../vector-space.md#standard-basis) [vectors](../../../vector-space.md#vector) to $(\cos\alpha,\sin\alpha)$ and $(-\sin\alpha,\cos\alpha)$. These images form the columns of its [matrix](../../../vector-space.md#matrix), so

$$
\boxed{R_2(\alpha)=\begin{pmatrix}\cos\alpha&-\sin\alpha\\\sin\alpha&\cos\alpha\end{pmatrix}.}
$$

The columns are an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) and the [determinant](../../../linear-algebra.md#determinant) is one, as required for a plane [rotation](../../../riemannian-geometry.md#rotation-mathematics).

<h4 id="7b/b">b</h4>

↑ **Parent:** [7B](#7b)

<h5 id="7b/b/solution">Solution</h5>

↑ **Parent:** [B](#7b/b)

Orient the axis towards $n=(3/5,4/5,0)$ and measure positive angles by the [right-hand rule](../../../electromagnetism.md#right-hand-rule) about $n$. The [vectors](../../../vector-space.md#vector) $n$, $m=(-4/5,3/5,0)$ and $e_3=(0,0,1)$ form a positively oriented [orthonormal basis](../../../linear-algebra.md#orthonormal-basis), since $n\times m=e_3$. Its [change-of-basis matrix](../../../linear-algebra.md#change-of-basis-matrix) is

$$
Q=\begin{pmatrix}3/5&-4/5&0\\4/5&3/5&0\\0&0&1\end{pmatrix},\qquad Q^{-1}=Q^T.
$$

Relative to this [basis](../../../vector-space.md#basis), the [rotation](../../../riemannian-geometry.md#rotation-mathematics) fixes the first coordinate and rotates the last two. Writing $c=\cos\alpha$ and $s=\sin\alpha$, its [matrix](../../../vector-space.md#matrix) in the [standard basis](../../../vector-space.md#standard-basis) is therefore

$$
\boxed{R=Q\begin{pmatrix}1&0&0\\0&c&-s\\0&s&c\end{pmatrix}Q^T
=\begin{pmatrix}(9+16c)/25&12(1-c)/25&4s/5\\12(1-c)/25&(16+9c)/25&-3s/5\\-4s/5&3s/5&c\end{pmatrix}.}
$$

In particular $Rn=n$, $Rm=cm+se_3$, and $Re_3=-sm+ce_3$, verifying the axis and the direction of [rotation](../../../riemannian-geometry.md#rotation-mathematics). Reversing the chosen orientation of the axis replaces $\alpha$ by $-\alpha$.

### 8D

↑ **Parent:** [Section II](#section-ii)

<h4 id="8d/solution">Solution</h4>

↑ **Parent:** [8D](#8d)

A [vector space](../../../vector-space.md) over the [real numbers](../../../arithmetic.md#real-number) is a [set](../../../set.md) $V$ with an [addition](../../../arithmetic.md#addition) making it an [abelian group](../../../group.md#abelian-group) and a [scalar multiplication](../../../vector-space.md#scalar-multiplication) by $\mathbb R$ satisfying, for [scalars](../../../vector-space.md#scalar) $a,b$ and [vectors](../../../vector-space.md#vector) $u,v$, the identities $a(u+v)=au+av$, $(a+b)v=av+bv$, $a(bv)=(ab)v$ and $1v=v$. A [vector subspace](../../../vector-space.md#vector-subspace) is a nonempty subset closed under [addition](../../../arithmetic.md#addition) and [scalar multiplication](../../../vector-space.md#scalar-multiplication); a [proper vector subspace](../../../vector-space.md#proper-vector-subspace) is one unequal to $V$. A [spanning set](../../../vector-space.md#spanning-set) is a [set](../../../set.md) whose finite [linear combinations](../../../vector-space.md#linear-combination) give every [vector](../../../vector-space.md#vector) of $V$. A [basis](../../../vector-space.md#basis) is a [linearly independent](../../../vector-space.md#linear-independence) [spanning set](../../../vector-space.md#spanning-set). The [dimension](../../../vector-space.md#dimension-vector-space) is the number of [vectors](../../../vector-space.md#vector) in a [basis](../../../vector-space.md#basis), or its cardinality when the [basis](../../../vector-space.md#basis) is infinite.

The [sum of vector subspaces](../../../vector-space.md#sum-of-vector-subspaces) and their [intersection of vector subspaces](../../../vector-space.md#intersection-of-vector-subspaces) are

$$
U+W=\{u+w:u\in U,\ w\in W\},\qquad
U\cap W=\{v\in V:v\in U\text{ and }v\in W\}.
$$

Both are [vector subspaces](../../../vector-space.md#vector-subspace): [addition](../../../arithmetic.md#addition) and [scalar multiplication](../../../vector-space.md#scalar-multiplication) preserve the displayed forms or simultaneous membership. The [intersection of vector subspaces](../../../vector-space.md#intersection-of-vector-subspaces) is never empty because **$0\in U\cap W$**.

For the two given [hyperplanes](../../../vector-space.md#hyperplane), adding and subtracting their defining equations gives $x_1=x_2$ and $x_3=x_4$. Hence

$$
U\cap W=\{(a,a,b,b):a,b\in\mathbb R\}
=\operatorname{span}\{b_1,b_2\},\quad b_1=(1,1,0,0),\quad b_2=(0,0,1,1).
$$

These two nonzero [vectors](../../../vector-space.md#vector) are [orthogonal](../../../linear-algebra.md#orthogonal-vectors), and consequently form an [orthogonal basis](../../../linear-algebra.md#orthogonal-basis) of the [intersection of vector subspaces](../../../vector-space.md#intersection-of-vector-subspaces). Put $u=(1,-1,-1,1)$ and $w=(1,-1,1,-1)$. Direct substitution gives $u\in U$, $w\in W$. Their [dot products](../../../linear-algebra.md#dot-product) with $b_1,b_2$ vanish, and $u\cdot w=0$. Each defining equation of $U$ or $W$ is one nonzero linear constraint in four variables, so each [vector subspace](../../../vector-space.md#vector-subspace) has [dimension](../../../vector-space.md#dimension-vector-space) three. Thus each space has the indicated [orthogonal basis](../../../linear-algebra.md#orthogonal-basis):

$$
\boxed{U:\ (b_1,b_2,u),\qquad W:\ (b_1,b_2,w),\qquad U+W:\ (b_1,b_2,u,w).}
$$

The last four [vectors](../../../vector-space.md#vector) are nonzero and mutually [orthogonal](../../../linear-algebra.md#orthogonal-vectors), so they are a [basis](../../../vector-space.md#basis) of $\mathbb R^4$. They lie in $U+W$, proving $U+W=V$. The [dimension](../../../vector-space.md#dimension-vector-space) identity is therefore verified numerically:

$$
\boxed{\dim U+\dim W=3+3=4+2=\dim(U+W)+\dim(U\cap W).}
$$

### 9C

↑ **Parent:** [Section II](#section-ii)

<h4 id="9c/solution">Solution</h4>

↑ **Parent:** [9C](#9c)

Use the [least-upper-bound property](../../../real-analysis.md#least-upper-bound-property) as the least upper bound axiom: every nonempty [set](../../../set.md) of [real numbers](../../../arithmetic.md#real-number) bounded above has a least upper bound in $\mathbb R$. It implies convergence of a bounded increasing [sequence](../../../real-analysis.md#sequence): if $L$ is the [supremum](../../../real-analysis.md#supremum) of its terms, then for every $\varepsilon>0$ some term exceeds $L-\varepsilon$, and all subsequent terms lie between that term and $L$. A bounded decreasing [sequence](../../../real-analysis.md#sequence) converges by applying this argument to its negative.

The [alternating series test](../../../real-analysis.md#alternating-series-test) states that if $b_n\ge0$, $b_{n+1}\le b_n$, and $b_n\to0$, then $\sum_{n\ge1}(-1)^{n-1}b_n$ converges. To prove it, let $S_N$ denote its [partial sums](../../../real-analysis.md#partial-sum). The even [partial sums](../../../real-analysis.md#partial-sum) are increasing because $S_{2m+2}-S_{2m}=b_{2m+1}-b_{2m+2}\ge0$. The odd [partial sums](../../../real-analysis.md#partial-sum) are decreasing because $S_{2m+3}-S_{2m+1}=-b_{2m+2}+b_{2m+3}\le0$. Moreover,

$$
0\le S_{2m}\le S_{2m+1}\le b_1.
$$

[Completeness of the real numbers](../../../real-analysis.md#completeness-of-the-real-numbers) therefore gives a [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence) for each subsequence, denoted $L_e,L_o$ respectively for the even and odd [subsequences](../../../real-analysis.md#subsequence). Their difference is $S_{2m+1}-S_{2m}=b_{2m+1}\to0$, so $L_e=L_o$. Every sufficiently late [partial sum](../../../real-analysis.md#partial-sum) belongs to one of these two [subsequences](../../../real-analysis.md#subsequence), proving convergence of the full [sequence](../../../real-analysis.md#sequence) of [partial sums](../../../real-analysis.md#partial-sum). Multiplying the terms by $-1$ leaves convergence unchanged.

<h4 id="9c/i">i</h4>

↑ **Parent:** [9C](#9c)

<h5 id="9c/i/solution">Solution</h5>

↑ **Parent:** [I](#9c/i)

The positive terms $b_n=1/\log(n+1)$ decrease to zero. The [alternating series test](../../../real-analysis.md#alternating-series-test) just proved therefore gives **convergence** of the signed [series](../../../real-analysis.md#series-mathematics). It is [conditional convergence](../../../real-analysis.md#conditional-convergence): $\log(n+1)\le n$, so $b_n\ge1/n$, and the absolute-value [series](../../../real-analysis.md#series-mathematics) dominates the divergent [harmonic series](../../../real-analysis.md#harmonic-series).

The [comparison test for series](../../../real-analysis.md#comparison-test-for-series) used here says that if $0\le c_n\le d_n$, convergence of $\sum d_n$ implies convergence of $\sum c_n$, while divergence of $\sum c_n$ implies divergence of $\sum d_n$. This follows by comparing increasing [partial sums](../../../real-analysis.md#partial-sum). For completeness, the [harmonic series](../../../real-analysis.md#harmonic-series) diverges because every block from $2^k$ to $2^{k+1}-1$ has sum at least $1/2$.

<h4 id="9c/ii">ii</h4>

↑ **Parent:** [9C](#9c)

<h5 id="9c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#9c/ii)

The absolute-value [series](../../../real-analysis.md#series-mathematics) can be grouped in pairs of nonnegative terms:

$$
\sum_{n\ge1}\bigl(|a_{2n-1}|+|a_{2n}|\bigr)
=\frac54\sum_{n\ge1}\frac1{n^2}<\infty.
$$

Indeed, $1/n^2\le\int_{n-1}^{n}x^{-2}\,dx$ for $n\ge2$, so these positive [partial sums](../../../real-analysis.md#partial-sum) are bounded by two. [Completeness of the real numbers](../../../real-analysis.md#completeness-of-the-real-numbers) proves their convergence. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) bounds every late signed sum by the corresponding late absolute-value sum, so [absolute convergence](../../../real-analysis.md#absolute-convergence) implies convergence. Thus **the [series](../../../real-analysis.md#series-mathematics) converges absolutely**.

<h4 id="9c/iii">iii</h4>

↑ **Parent:** [9C](#9c)

<h5 id="9c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#9c/iii)

[Group](../../../group.md) three consecutive terms. Their block sum is

$$
b_n=-\frac1{2n-1}+\frac1{4n-1}+\frac1{4n}
=-\frac{6n-1}{4n(2n-1)(4n-1)}.
$$

Since $2n-1\ge n$ and $4n-1\ge3n$ for $n\ge1$, we have $|b_n|\le1/(2n^2)$. The [comparison test for series](../../../real-analysis.md#comparison-test-for-series) and the preceding proof of convergence of $\sum n^{-2}$ show that $\sum b_n$ converges absolutely.

This establishes convergence of the original [partial sums](../../../real-analysis.md#partial-sum) at indices $3N$. Each intermediate [partial sum](../../../real-analysis.md#partial-sum) differs from one of these by at most two of the original terms; those terms tend to zero. Thus all [partial sums](../../../real-analysis.md#partial-sum) have the same [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence), which is the mechanism of [convergence from fixed-length series blocks](../../../real-analysis.md#convergence-from-fixed-length-series-blocks). The original [series](../../../real-analysis.md#series-mathematics) is not absolutely convergent, since its absolute-value [series](../../../real-analysis.md#series-mathematics) contains $\sum_n(2n-1)^{-1}\ge\tfrac12\sum_n n^{-1}$. Therefore **the original [series](../../../real-analysis.md#series-mathematics) converges conditionally**.

<h4 id="9c/iv">iv</h4>

↑ **Parent:** [9C](#9c)

<h5 id="9c/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#9c/iv)

Let $S_N=\sum_{k=1}^Na_k$, with $S_0=0$. The indices in the $n$th dyadic block have one sign, so

$$
\left|S_{2^{n+1}-1}-S_{2^n-1}\right|
=\sum_{r=0}^{2^n-1}\frac1{2^n+r}>\frac{2^n}{2^{n+1}}=\frac12.
$$

A convergent [sequence](../../../real-analysis.md#sequence) of [partial sums](../../../real-analysis.md#partial-sum) must be a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence): for every $\varepsilon>0$, all sufficiently late pairs of [partial sums](../../../real-analysis.md#partial-sum) differ by less than $\varepsilon$. The displayed differences violate this necessary condition with $\varepsilon=1/4$, at arbitrarily late endpoints. Thus **the [series](../../../real-analysis.md#series-mathematics) diverges**, even though its individual terms tend to zero. This [dyadic-block alternation of reciprocal terms](../../../real-analysis.md#dyadic-block-alternation-of-reciprocal-terms) has growing block lengths; the fixed-length block argument of the previous part does not apply.

### 10C

↑ **Parent:** [Section II](#section-ii)

<h4 id="10c/solution">Solution</h4>

↑ **Parent:** [10C](#10c)

Let $f$ be [continuous](../../../calculus.md#continuous-function) on a closed bounded interval $[a,b]$. First prove that $f$ is a [bounded function](../../../function.md#bounded-function). If it failed, we could choose $x_n\in[a,b]$ with $|f(x_n)|>n$. The [Bolzano-Weierstrass theorem](../../../real-analysis.md#bolzano-weierstrass-theorem) gives a [subsequence](../../../real-analysis.md#subsequence) $x_{n_j}\to x_*$. Because the interval is closed, $x_*\in[a,b]$. [Continuity](../../../calculus.md#continuous-function) gives $f(x_{n_j})\to f(x_*)$, contradicting $|f(x_{n_j})|>n_j\to\infty$.

Now let $M=\sup\{f(x):x\in[a,b]\}$, which exists by [completeness of the real numbers](../../../real-analysis.md#completeness-of-the-real-numbers) and the bound just proved. Choose $y_n\in[a,b]$ with $f(y_n)>M-1/n$. A [convergent subsequence](../../../real-analysis.md#convergent-subsequence) has [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence) $y_*\in[a,b]$, and [continuity](../../../calculus.md#continuous-function) gives $f(y_*)=M$. Applying the same argument to $-f$ gives attainment of the [infimum](../../../real-analysis.md#infimum). This proves the [extreme value theorem](../../../real-analysis.md#extreme-value-theorem): **the maximum and minimum both exist and are attained**. The argument also covers a one-point interval, where the conclusions are immediate.

<h4 id="10c/i">i</h4>

↑ **Parent:** [10C](#10c)

<h5 id="10c/i/solution">Solution</h5>

↑ **Parent:** [I](#10c/i)

Take **$f_1(x)=1/x$**. It is [continuous](../../../calculus.md#continuous-function) on $(0,1)$ and unbounded as $x\to0$ from the right.

<h4 id="10c/ii">ii</h4>

↑ **Parent:** [10C](#10c)

<h5 id="10c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#10c/ii)

Take **$f_2(x)=x$**. It is [continuous](../../../calculus.md#continuous-function) and bounded on $(0,1)$, with [infimum](../../../real-analysis.md#infimum) zero and [supremum](../../../real-analysis.md#supremum) one, neither attained on this open interval.

<h4 id="10c/iii">iii</h4>

↑ **Parent:** [10C](#10c)

<h5 id="10c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#10c/iii)

Take the [step function](../../../measure-theory.md#step-function)

$$
\boxed{f_3(x)=\begin{cases}0,&0\le x<1/2,\\1,&1/2\le x\le1.\end{cases}}
$$

It is bounded between zero and one, and is discontinuous at $x=1/2$.

<h4 id="10c/iv">iv</h4>

↑ **Parent:** [10C](#10c)

<h5 id="10c/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#10c/iv)

Use the [reduced-denominator function unbounded on every interval](../../../mathematics.md#reduced-denominator-function-unbounded-on-every-interval):

$$
\boxed{f_4(x)=\begin{cases}q,&x=p/q\text{ in lowest terms},\ q>0,\\0,&x\notin\mathbb Q.\end{cases}}
$$

Every value is a finite [real number](../../../arithmetic.md#real-number). In any nondegenerate interval $[a,b]\subseteq[0,1]$, its interior contains infinitely many [rational numbers](../../../number-theory.md#rational-number), whereas there are only finitely many reduced fractions in $[0,1]$ with denominator at most any fixed $M$. Some [rational number](../../../number-theory.md#rational-number) in $(a,b)$ therefore has denominator exceeding $M$. Hence the [function](../../../function.md) is unbounded on every such interval. It reverses the positive values of the [Thomae function](../../../mathematics.md#thomae-function) rather than requiring an infinite value at any point.

### 11C

↑ **Parent:** [Section II](#section-ii)

<h4 id="11c/solution">Solution</h4>

↑ **Parent:** [11C](#11c)

The [mean value theorem](../../../calculus.md#mean-value-theorem) states that, if $f$ is [continuous](../../../calculus.md#continuous-function) on $[a,b]$ and [differentiable](../../../analysis.md#differentiable-function) on $(a,b)$, with $a<b$, there is $c\in(a,b)$ such that

$$
f'(c)=\frac{f(b)-f(a)}{b-a}.
$$

To deduce it from [Rolle's theorem](../../../calculus.md#rolle-theorem), subtract the secant line: $k(t)=f(t)-f(a)-\frac{f(b)-f(a)}{b-a}(t-a)$. This [function](../../../function.md) has the same [continuity](../../../calculus.md#continuous-function) and [differentiability](../../../analysis.md#differentiability) properties and satisfies $k(a)=k(b)=0$. [Rolle's theorem](../../../calculus.md#rolle-theorem) gives an interior point with $k'(c)=0$, which is precisely the required equality.

If $h'=0$ on $\mathbb R$, apply the [mean value theorem](../../../calculus.md#mean-value-theorem) on any $[x,y]$ with $x<y$. It gives $h(y)-h(x)=(y-x)h'(c)=0$. Hence **$h$ is constant**.

For the [differential equation](../../../differential-equation.md), the [product rule](../../../calculus.md#product-rule) gives

$$
\frac{d}{dx}\bigl(e^{-ax}f(x)\bigr)=e^{-ax}\bigl(f'(x)-af(x)\bigr)=0.
$$

The preceding result makes this product constant. Thus **all solutions are $f(x)=Ce^{ax}$**, and differentiation verifies every such solution.

For the [integral](../../../calculus.md#integral) assertion, [continuity](../../../calculus.md#continuous-function) ensures that $f$ is [Riemann integrable](../../../real-analysis.md#riemann-integrable-function) on every finite [closed interval](../../../real-analysis.md#closed-real-interval). Use the usual orientation for an [integral](../../../calculus.md#integral) with negative upper endpoint. For $h\ne0$, additivity of the [integral](../../../calculus.md#integral) gives

$$
\frac{F(x+h)-F(x)}h-f(x)
=\frac1h\int_x^{x+h}\bigl(f(t)-f(x)\bigr)\,dt.
$$

The [absolute value](../../../real-analysis.md#absolute-value) of this expression is at most the [supremum](../../../real-analysis.md#supremum) of $|f(t)-f(x)|$ on the segment joining $x$ and $x+h$. [Continuity](../../../calculus.md#continuous-function) at $x$ makes this bound tend to zero for either sign of $h$. Consequently **$F'(x)=f(x)$**, proving this form of the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus).

Finally, a [differentiable](../../../analysis.md#differentiable-function) solution of the [integral equation](../../../analysis.md#integral-equation) is [continuous](../../../calculus.md#continuous-function), so the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) yields $g'=g$; setting $x=0$ gives $g(0)=A$. The differential-equation calculation above now forces

$$
\boxed{g(x)=Ae^x.}
$$

Conversely, $A+\int_0^xAe^t\,dt=A+A(e^x-1)=Ae^x$, so this [function](../../../function.md) satisfies the original [integral equation](../../../analysis.md#integral-equation). It is unique because every [differentiable](../../../analysis.md#differentiable-function) solution has already been forced to this form and this [initial condition](../../../differential-equation.md#initial-condition).

### 12C

↑ **Parent:** [Section II](#section-ii)

<h4 id="12c/solution">Solution</h4>

↑ **Parent:** [12C](#12c)

For a [function](../../../function.md) with [continuous](../../../calculus.md#continuous-function) [derivatives](../../../calculus.md#derivative) through order $m+1$ on the interval between $0$ and $x$, the [Taylor formula with integral remainder](../../../calculus.md#taylor-formula-with-integral-remainder) is

$$
f(x)=\sum_{j=0}^{m}\frac{f^{(j)}(0)}{j!}x^j+R_m(x),\qquad
R_m(x)=\frac1{m!}\int_0^x(x-t)^m f^{(m+1)}(t)\,dt.
$$

This is [Taylor's theorem](../../../calculus.md#taylor-theorem) about zero; [translation](../../../geometry-and-topology.md#translation-geometry) gives the formula about any other point. To prove it, the case $m=0$ is the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus). For $m\ge1$, [integration by parts](../../../calculus.md#integration-by-parts) gives

$$
R_m(x)=-\frac{f^{(m)}(0)x^m}{m!}
+\frac1{(m-1)!}\int_0^x(x-t)^{m-1}f^{(m)}(t)\,dt
=R_{m-1}(x)-\frac{f^{(m)}(0)x^m}{m!}.
$$

Substitution into the formula at order $m-1$ proves the formula at order $m$ by induction. The [integral](../../../calculus.md#integral) estimate, valid also for negative $x$, is

$$
|R_m(x)|\le\frac{|x|^{m+1}}{(m+1)!}
\sup_{t\text{ between }0\text{ and }x}|f^{(m+1)}(t)|.
$$

For the [smooth function](../../../analysis.md#smooth-function) satisfying $f^{(3)}=f$, each fixed [derivative](../../../calculus.md#derivative) is [continuous](../../../calculus.md#continuous-function) on $[-R,R]$ and hence is bounded there by the [extreme value theorem](../../../real-analysis.md#extreme-value-theorem). Thus a bound $M_j$ exists for every $j$. Differentiating the [differential equation](../../../differential-equation.md) repeatedly gives $f^{(j+3)}=f^{(j)}$. Only the three [functions](../../../function.md) $f,f',f''$ are needed: take $M$ to be the maximum of their absolute-value bounds on $[-R,R]$. Then $|f^{(j)}(x)|\le M$ simultaneously for every $j\ge0$ and $|x|\le R$.

At zero the [derivatives](../../../calculus.md#derivative) consequently repeat the values $1,0,0$. [Taylor's theorem](../../../calculus.md#taylor-theorem) therefore gives

$$
f(x)=\sum_{n=0}^{\lfloor m/3\rfloor}\frac{x^{3n}}{(3n)!}+R_m(x),\qquad
\sup_{|x|\le R}|R_m(x)|\le\frac{MR^{m+1}}{(m+1)!}\longrightarrow0.
$$

The last [limit of a sequence](../../../real-analysis.md#limit-of-a-sequence) follows because the ratio of consecutive majorants is $R/(m+2)$, eventually less than $1/2$. Since $R$ is arbitrary, [Taylor expansion from a periodic derivative equation](../../../calculus.md#taylor-expansion-from-a-periodic-derivative-equation) proves

$$
\boxed{f(x)=\sum_{n=0}^{\infty}\frac{x^{3n}}{(3n)!}\quad\text{for every }x\in\mathbb R.}
$$

This proves convergence to the [function](../../../function.md) using a remainder bound; it does not assume beforehand that a [smooth function](../../../analysis.md#smooth-function) equals its [Taylor series](../../../calculus.md#taylor-series).

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
