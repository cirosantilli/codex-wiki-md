# Paper 130

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_130.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_130.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [Solution](#4/solution)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)

## 1

↑ **Parent:** [Paper 130](paper-130.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Fix a number $k$ of colors. For a two-point set whose points are distance $d$ apart, take the vertices of a [regular simplex](../../../algebraic-topology.md#regular-simplex) with $k+1$ vertices and side length $d$. The [pigeonhole principle](../../../algebra.md#pigeonhole-principle) gives two vertices of one color, and they form the required congruent copy. Thus every two-point set, equivalently every [line segment](../../../mathematical-optimization.md#line-segment), is a [Euclidean Ramsey set](../../../ramsey-theory.md#euclidean-ramsey-set).

For an [equilateral triangle](../../../geometry-and-topology.md#equilateral-triangle) of side length $d$, take a [regular simplex](../../../algebraic-topology.md#regular-simplex) with $2k+1$ vertices and side length $d$. The [pigeonhole principle](../../../algebra.md#pigeonhole-principle) gives three vertices of one color, and every three vertices of a regular simplex form an equilateral triangle. Hence every equilateral triangle is Euclidean Ramsey.

To prove the [product theorem for Euclidean Ramsey sets](../../../ramsey-theory.md#product-theorem-for-euclidean-ramsey-sets), let $S_X$ be a finite Ramsey witness for $X$ under $k$ colors. There are at most $k^{|S_X|}$ possible color patterns on $S_X$. Choose a finite Ramsey witness $S_Y$ for $Y$ under that many colors. Given a $k$-coloring of $S_X\times S_Y$, color each $y\in S_Y$ by the complete pattern

$$
x\longmapsto c(x,y),\qquad x\in S_X.
$$

There is a copy $Y'\cong Y$ on which this pattern is constant. The common pattern on $S_X$ contains a monochromatic copy $X'\cong X$. Every point of $X'\times Y'$ then has the same original color, and the orthogonal product is congruent to $X\times Y$.

A rectangle is the [Cartesian product](../../../set-theory.md#cartesian-product) of two line segments, so it is Euclidean Ramsey. Three suitable vertices of a rectangle form a [right triangle](../../../geometry-and-topology.md#right-triangle); any subset of a monochromatic set is monochromatic. Thus every right triangle is Euclidean Ramsey.

It remains to show that the collinear set $\{0,1,2\}$ behaves differently. In every $\mathbb R^m$, use the [finite coloring](../../../ramsey-theory.md#finite-coloring)

$$
c(x)=\lfloor2\|x\|^2\rfloor\pmod {10}.
$$

A congruent copy has the form $a-v,a,a+v$ with $\|v\|=1$ for the [Euclidean norm](../../../functional-analysis.md#euclidean-norm). The [parallelogram law](../../../linear-algebra.md#parallelogram-law) gives

$$
2\|a+v\|^2+2\|a-v\|^2-4\|a\|^2=4.
$$

Put $n_+=\lfloor2\|a+v\|^2\rfloor$, $n_-=\lfloor2\|a-v\|^2\rfloor$, and $n_0=\lfloor2\|a\|^2\rfloor$. The errors introduced by the three [floor functions](../../../calculus.md#floor-function) show that

$$
2<n_++n_--2n_0<6.
$$

If all three points had one color, the integer in the middle would be divisible by ten, which is impossible. This proves the [three-term unit arithmetic progression is not Euclidean Ramsey](../../../ramsey-theory.md#three-term-unit-arithmetic-progression-is-not-euclidean-ramsey) assertion.

## 2

↑ **Parent:** [Paper 130](paper-130.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [Hales-Jewett theorem](../../../ramsey-theory.md#hales-jewett-theorem) says that, for every finite alphabet $A$ and number of colors $r$, there is $N$ such that every $r$-coloring of $A^N$ contains a monochromatic [combinatorial line](../../../ramsey-theory.md#combinatorial-line).

We use the standard insensitivity lemma. Assuming the Hales-Jewett theorem for alphabets of size $m-1$, fix two letters $a,b$ in an $m$-letter alphabet. For every $r$ and $d$, there is $N$ such that each $r$-coloring of $A^N$ has a $d$-dimensional [combinatorial subspace](../../../ramsey-theory.md#combinatorial-subspace) on which changing any selection of variable coordinates from $a$ to $b$, or from $b$ to $a$, leaves the color unchanged.

Here is the finite fusion proof of the lemma. Choose the sizes of $d$ successive coordinate blocks backwards. On the last block, omit $b$ and color a word over $A\setminus\{b\}$ by the vector of all colors obtained after filling the previously chosen blocks in every possible way and then replacing any chosen occurrences of $a$ by $b$. This is a finite derived coloring. The induction hypothesis supplies a combinatorial line on which that entire vector is constant. Treat its active coordinates as one new variable block and repeat. After $d$ repetitions, each replacement of $a$ by $b$ can be pushed into the last block where it was created, and equality of the derived color vectors shows that it does not alter the original color. This proves the insensitivity lemma.

Now induct on $m=|A|$. The case $m=1$ is immediate. For $m>1$, choose the target dimensions backwards and apply the insensitivity lemma successively to the pairs

$$
(a_m,a_1),\ldots,(a_m,a_{m-1}).
$$

At every step pass to the resulting nested combinatorial subspace, so the insensitivities already obtained are retained. On the final positive-dimensional subspace, replacing $a_m$ by any other letter does not change the color. Any two words can be connected by such replacements, so the whole subspace is monochromatic. It contains a combinatorial line, completing the induction and the proof.

The [Gallai theorem for an integer lattice](../../../ramsey-theory.md#gallai-theorem-for-an-integer-lattice) says that, for every finite $S\subseteq\mathbb N^d$ and every finite coloring of $\mathbb N^d$, there are $u\in\mathbb N^d$ and $q\geq1$ such that the homothetic copy

$$
u+qS=\{u+qs:s\in S\}
$$

is monochromatic.

Write $S=\{s_1,\ldots,s_m\}$ and apply the Hales-Jewett theorem to the alphabet $[m]$. Color a word $w\in[m]^N$ by the color of

$$
\Phi(w)=t+\sum_{j=1}^Ns_{w_j},
$$

where a fixed positive vector $t$ keeps the image in $\mathbb N^d$ under either convention for the natural numbers. On a monochromatic combinatorial line, let $I$ be the active coordinate set. The fixed coordinates contribute a vector $u-t$, while the word whose active letter is $i$ maps to

$$
u+|I|s_i.
$$

These points form a monochromatic copy $u+|I|S$, proving Gallai's theorem.

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

This is always true. Pull the given coloring of $\mathbb N^2$ back along the dilation

$$
(x,y)\longmapsto(2x,2y).
$$

Apply the [Gallai theorem for an integer lattice](../../../ramsey-theory.md#gallai-theorem-for-an-integer-lattice) to the four vertices of the unit square. The image of the resulting homothetic square has side length $2q$, which is even, and all four vertices have one color.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

This can fail. Color $(x,y)$ by the parity of $x$. If a square has odd side length $q$, then the two endpoints of each horizontal side have first coordinates of opposite parity, so the square cannot be monochromatic.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

This can also fail. Color $(x,y)$ by $x\pmod3$. No power of two is divisible by three, so the endpoints of a horizontal side whose length is a power of two receive different colors.

## 3

↑ **Parent:** [Paper 130](paper-130.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A rational matrix is a [partition regular matrix](../../../ramsey-theory.md#partition-regular-matrix) when every finite coloring of the positive integers admits a monochromatic positive vector in its kernel. Its columns have the [columns property](../../../ramsey-theory.md#columns-property) if their indices can be partitioned into ordered nonempty blocks $B_1,\ldots,B_s$ such that the columns in $B_1$ sum to zero and, for $j>1$, the sum over $B_j$ lies in the rational linear span of the columns in the earlier blocks. [Rado's theorem](../../../ramsey-theory.md#rado-s-theorem) states that a rational matrix is partition regular if and only if its columns have this property.

For one equation, clear denominators and write

$$
c_1x_1+\cdots+c_nx_n=0,
\qquad c_i\in\mathbb Z\setminus\{0\}.
$$

The one-row columns property is equivalent to the existence of a nonempty $I\subseteq[n]$ with

$$
\sum_{i\in I}c_i=0.
$$

First suppose such an $I$ exists. Choose $i_0\in I$, put $c=|c_{i_0}|$, $C=\sum_{j\notin I}c_j$, and choose $p\geq|C|$. The [monochromatic m-p-c set theorem](../../../ramsey-theory.md#monochromatic-m-p-c-set-theorem), whose finite induction proof uses the [Van der Waerden theorem](../../../ramsey-theory.md#van-der-waerden-theorem), gives positive $z_1,z_2$ for which all numbers

$$
cz_1+\lambda z_2\quad(|\lambda|\leq p),
\qquad cz_2
$$

are positive and have one color. Set

$$
x_i=cz_1\quad(i\in I\setminus\{i_0\}),
\qquad
x_{i_0}=cz_1-\frac{Cc}{c_{i_0}}z_2,
\qquad
x_j=cz_2\quad(j\notin I).
$$

The middle coefficient is the integer $-C\operatorname{sgn}(c_{i_0})$, of absolute value at most $p$, so all the $x_i$ belong to the monochromatic set. Their $z_1$ contribution vanishes because the coefficients over $I$ sum to zero, and their $z_2$ contribution is

$$
c_{i_0}\left(-\frac{Cc}{c_{i_0}}\right)+Cc=0.
$$

Thus the equation is partition regular.

Conversely, suppose no nonempty subset of the coefficients sums to zero. Choose a [prime number](../../../number-theory.md#prime-number) $p$ that divides none of the finitely many nonzero subset sums. Color each positive integer by its [last nonzero digit coloring](../../../ramsey-theory.md#last-nonzero-digit-coloring) in base $p$. If a monochromatic solution existed, let $v$ be the smallest [P-adic valuation](../../../number-theory.md#p-adic-valuation) among its coordinates and let $I$ index the coordinates of valuation $v$. After division by $p^v$ and reduction modulo $p$, all $x_i$ with $i\in I$ have the same nonzero last digit $r$, while the other terms vanish. The equation would give

$$
r\sum_{i\in I}c_i\equiv0\pmod p,
$$

contrary to the choice of $p$. This proves the [Rado theorem for one equation](../../../ramsey-theory.md#rado-theorem-for-one-equation).

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

**No.** Take

$$
(a_1,a_2,a_3,a_4)=(1,1,-1,-1).
$$

The full set of coefficients sums to zero, so the equation is partition regular by the [Rado theorem for one equation](../../../ramsey-theory.md#rado-theorem-for-one-equation). Every solution satisfies

$$
x_1+x_2-x_3-x_4=0,
$$

which can never be positive.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

**No.** Consider

$$
(a_1,a_2,a_3,a_4)=(1,1,1,-4).
$$

Every finite coloring of the positive integers has an infinite color class. Choose $x<y$ in that class with $y/x$ as large as needed. Assigning $y$ to the three positive-coefficient variables and $x$ to the negative-coefficient variable makes the linear form

$$
3y-4x
$$

positive. Reversing the assignments makes it $3x-4y<0$. Thus both strict-sign hypotheses hold in every finite coloring.

The nonempty subset sums of $1,1,1,-4$ are among $1,2,3,-1,-2,-3,-4$, so none is zero. The [Rado theorem for one equation](../../../ramsey-theory.md#rado-theorem-for-one-equation) therefore says that this coefficient vector is not partition regular.

## 4

↑ **Parent:** [Paper 130](paper-130.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [filter on a set](../../../set-theory.md#filter-set-theory) $X$ is a nonempty family $\mathcal F\subseteq\mathcal P(X)$ that excludes the empty set, is upward closed, and is closed under finite intersections. An [ultrafilter](../../../set-theory.md#ultrafilter) is a proper filter that contains exactly one of $A$ and $X\setminus A$ for every subset $A\subseteq X$.

To prove the [ultrafilter lemma](../../../set-theory.md#ultrafilter-lemma), order the proper filters containing $\mathcal F$ by inclusion. The union of any chain is again a proper filter, so [Zorn lemma](../../../set-theory.md#zorn-s-lemma) gives a maximal extension $\mathcal U$. If neither $A$ nor $X\setminus A$ belonged to $\mathcal U$, adjoining either one would generate an improper filter. There would then be $U,V\in\mathcal U$ with $U\cap A=\varnothing$ and $V\cap(X\setminus A)=\varnothing$. But $U\cap V=\varnothing$, contradicting propriety. Hence $\mathcal U$ is an ultrafilter.

The [Stone-Čech compactification of the natural numbers](../../../set-theory.md#stone-cech-compactification-of-the-natural-numbers) $\beta\mathbb N$ is the set of all ultrafilters on $\mathbb N$, with basic sets

$$
\overline A=\{\mathcal U:A\in\mathcal U\},
\qquad A\subseteq\mathbb N.
$$

The identities

$$
\overline A\cap\overline B=\overline{A\cap B},
\qquad
\beta\mathbb N\setminus\overline A=\overline{\mathbb N\setminus A}
$$

show that these sets form a basis of [clopen sets](../../../topology.md#clopen-set). Distinct ultrafilters disagree on some $A$; one lies in $\overline A$ and the other in the disjoint set $\overline{\mathbb N\setminus A}$. Thus $\beta\mathbb N$ is a [Hausdorff space](../../../topology.md#hausdorff-space).

If a family of basic closed sets $\overline{A_i}$ has the [finite intersection property](../../../topology.md#finite-intersection-property), then the sets $A_i$ have the same property. They generate a proper filter, which extends to an ultrafilter lying in every $\overline{A_i}$. The [Alexander subbase theorem](../../../topology.md#alexander-s-subbase-lemma) now implies that $\beta\mathbb N$ is a [compact space](../../../topology.md#compact-space).

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Assume condition ii. In a finite coloring

$$
\mathbb N=C_1\sqcup\cdots\sqcup C_r,
$$

an [ultrafilter](../../../set-theory.md#ultrafilter) contains exactly one color class: at least one must belong to it because their union is $\mathbb N$, and two disjoint classes cannot both belong to a proper filter. The chosen $C_i$ contains a member of $\mathcal S$, which is therefore monochromatic. This proves condition i.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Assume condition i and call a set $B\subseteq\mathbb N$ bad when it contains no member of $\mathcal S$. No finite collection of bad sets covers $\mathbb N$: if it did, assigning each integer to the first bad set containing it would give a finite coloring whose color classes are bad, contrary to condition i. Consequently

$$
\{\mathbb N\setminus B:B\text{ is bad}\}
$$

has the finite-intersection property. It generates a proper [filter on a set](../../../set-theory.md#filter-set-theory), which the [ultrafilter lemma](../../../set-theory.md#ultrafilter-lemma) extends to an ultrafilter $\mathcal U$. If some $A\in\mathcal U$ were bad, then $\mathbb N\setminus A$ would also belong to $\mathcal U$ by construction, contradicting propriety. Hence every $A\in\mathcal U$ contains a member of $\mathcal S$, proving condition ii.

For the final question, let $\mathcal S$ consist of the pairs $\{x,2x\}$ and $\{x,3x\}$. Color $n$ by

$$
v_2(n)+v_3(n)\pmod2.
$$

Multiplication by either two or three reverses this parity, so this two-coloring has no monochromatic member of $\mathcal S$. Condition i fails, and the equivalence just proved shows that no ultrafilter with the stated property exists.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
