<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [dynamical proof of Hindman's theorem](../../../../../../dynamical-proof-of-hindman-s-theorem.md) gives the following result. The [Hindman theorem](../../../../../../hindman-theorem.md) asserts that every [finite coloring](../../../../../../finite-coloring.md) of the [positive integers](../../../../../../positive-integer.md) admits an infinite strictly increasing [sequence](../../../../../../sequence.md) $(a_i)$ for which all nonempty finite sums of distinct terms have one color. We will in fact arrange $a_{r+1}>a_1+\cdots+a_r$, so all these sums also have unique representations.

Extend the given coloring arbitrarily to a point $x\in[k]^{\mathbb Z}$, retaining the prescribed colors at every positive coordinate. Let $X$ be its forward [orbit closure](../../../../../../orbit-closure.md) under the [left shift](../../../../../../left-shift.md). The [product topology](../../../../../../product-topology.md) makes $X$ a [compact metric space](../../../../../../compact-metric-space.md), and the [left shift](../../../../../../left-shift.md) is a [continuous map](../../../../../../continuous-map.md). There is a nonempty [minimal subsystem](../../../../../../minimal-subsystem.md) $Y\subseteq X$: order the nonempty closed forward-invariant [subsets](../../../../../../subset.md) by reverse inclusion, use [compactness](../../../../../../compact-space.md) and the [finite intersection property](../../../../../../finite-intersection-property.md) to intersect any chain, and apply the [Zorn lemma](../../../../../../zorn-s-lemma.md). Minimality also implies $\mathcal L(Y)=Y$. The result permitted in the question now supplies a [minimal point](../../../../../../minimal-point.md) $y\in Y$ [proximal](../../../../../../proximality.md) to $x$.

We need the [joint return lemma for a proximal minimal pair](../../../../../../joint-return-lemma-for-a-proximal-minimal-pair.md), which we prove here. It suffices to consider an open [neighborhood](../../../../../../neighbourhood-mathematics.md) $U$ of $y$ in $X$. Choose an open [neighborhood](../../../../../../neighbourhood-mathematics.md) $V$ of $y$ with $\overline V\subseteq U$. Every forward [orbit](../../../../../../orbit-dynamical-system.md) in $Y$ meets $V$, and a finite subcover of $\{\mathcal L^{-j}V:j\geq0\}$ on $Y$ supplies a bound $J$ on the needed return index. For a [compatible metric](../../../../../../compatible-metric.md) $d$, choose $\eta>0$ smaller than the distance from $\overline V$ to $X\setminus U$ when the latter is nonempty. By [uniform continuity](../../../../../../uniform-continuity.md) of the finitely many maps $\mathcal L^j$, $0\leq j\leq J$, some $\delta>0$ ensures

$$
d(z,z')<\delta\ \Longrightarrow
d(\mathcal L^jz,\mathcal L^jz')<\eta\quad(0\leq j\leq J).
$$

[Proximality](../../../../../../proximality.md) supplies arbitrarily large $t$ with $d(\mathcal L^t x,\mathcal L^t y)<\delta$. To see that the times can be large under the definition using an infimum over $t\geq0$, either $x=y$, in which case this is automatic, or injectivity of the [left shift](../../../../../../left-shift.md) makes every finite collection of distances strictly positive, so a sufficiently smaller [proximal](../../../../../../proximality.md) distance occurs beyond that collection. Some $j\leq J$ has $\mathcal L^{t+j}y\in V$. Then $\mathcal L^{t+j}x\in U$ also. Hence arbitrarily large positive $n$ satisfy

$$
\mathcal L^n x\in U,\qquad \mathcal L^n y\in U.
$$

This uses the [minimal point](../../../../../../minimal-point.md) property for bounded returns and [proximality](../../../../../../proximality.md) for closeness; closeness alone would not guarantee a return near $y$.

Put $q=y(0)$. Inductively, let $F_r=\{0\}\cup\operatorname{FS}(a_1,\ldots,a_r)$, where $\operatorname{FS}$ denotes the [finite-sums set](../../../../../../finite-sums-set.md), and maintain

$$
y(s)=q\quad(s\in F_r),\qquad x(s)=q\quad(s\in F_r\setminus\{0\}).
$$

The initial condition at $r=0$ is just $y(0)=q$; no condition on $x(0)$ is required. The [cylinder set](../../../../../../cylinder-set.md) $U_r=\{z:z(s)=q\text{ for every }s\in F_r\}$ is a [neighborhood](../../../../../../neighbourhood-mathematics.md) of $y$. Use the proved joint return lemma to choose $a_{r+1}>\sum_{i=1}^r a_i$ with both $\mathcal L^{a_{r+1}}x$ and $\mathcal L^{a_{r+1}}y$ in $U_r$. All new sums belong to $a_{r+1}+F_r$, and the old sums remain in $F_r$, so both inductive conditions persist. Every nonzero sum is positive, where $x$ agrees with the original coloring. Therefore

$$
\boxed{\chi(s)=q\quad\text{for every }s\in\operatorname{FS}(a_1,a_2,\ldots).}
$$

This proves the [Hindman theorem](../../../../../../hindman-theorem.md) using only the permitted proximal-minimal existence result and the [compactness](../../../../../../compact-space.md) and return arguments supplied above.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
