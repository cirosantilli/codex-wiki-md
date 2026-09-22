<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [zero-dimensional space](../../../zero-dimensional-space.md) has a base of [clopen sets](../../../clopen-set.md). A [totally disconnected space](../../../totally-disconnected-space.md) has no [connected subset](../../../connected-subset.md) with more than one point, equivalently all its [connected components](../../../connected-component.md) are singletons. We use these definitions in the stated Hausdorff setting.

If a [Hausdorff space](../../../hausdorff-space.md) has a clopen base, any two different points can be separated by a [clopen set](../../../clopen-set.md). A [connected subset](../../../connected-subset.md) containing both would be split into two nonempty disjoint relatively open sets. Thus **zero-dimensional implies totally disconnected** here.

**The compact converse, including the component lemma.** For a point $x$ of a compact Hausdorff $K$, put

$$
Q_x=\bigcap\{N:x\in N,\ N\text{ clopen in }K\}.
$$

This is its [quasicomponent](../../../quasicomponent.md), a closed compact set. We prove the [Šura-Bura component lemma](../../../sura-bura-component-lemma.md) that $Q_x$ equals the [connected component](../../../connected-component.md) of $x$.

Suppose $Q_x=A\cup B$ were a separation into nonempty disjoint relatively closed sets, with $x\in A$. Both are compact, hence closed in $K$. Normality of [compact Hausdorff spaces](../../../compact-hausdorff-space.md) gives disjoint [open neighborhoods](../../../open-neighbourhood.md) $U\supseteq A$, $V\supseteq B$. The compact set $H=K\setminus(U\cup V)$ misses $Q_x$. For each $y\in H$, choose a clopen neighborhood $N_y$ of $x$ missing $y$; these exist by the definition of $Q_x$. The open complements cover $H$, so finitely many suffice. Their intersection $N$ is clopen, contains $Q_x$, and lies in $U\cup V$. If $H$ is empty take $N=K$.

Now $N\cap U$ is clopen in $K$: it is open, and its complement is $(K\setminus N)\cup(N\cap V)$, also open. It contains $x$ and misses $B$, contradicting that $B\subseteq Q_x$ lies in every clopen neighborhood of $x$. Hence $Q_x$ is connected. Conversely every [connected subset](../../../connected-subset.md) containing $x$ lies in every clopen neighborhood of $x$, so the [connected component](../../../connected-component.md) is contained in $Q_x$. Equality follows.

If $K$ is [totally disconnected](../../../totally-disconnected-space.md), then $Q_x=\{x\}$. Given an [open neighborhood](../../../open-neighbourhood.md) $O$ of $x$, for each $y\in K\setminus O$ choose a clopen neighborhood of $x$ missing $y$. Compactness again gives a finite intersection $N$ with $x\in N\subseteq O$. These $N$ form a clopen base. Therefore

$$
\boxed{K\text{ compact Hausdorff}:\qquad K\text{ zero-dimensional}\iff K\text{ totally disconnected}.}
$$

**The Stone-Čech characterization.** The stated clopen separation property is [strong zero-dimensionality](../../../strong-zero-dimensionality.md) in this normal Hausdorff setting. A normal [T1 space](../../../t1-space.md) is a [Tychonoff space](../../../completely-regular-hausdorff-space.md), so its [Stone-Čech compactification](../../../stone-cech-compactification.md) exists. We use its extension property for maps into [compact Hausdorff spaces](../../../compact-hausdorff-space.md) and the density of $X$.

First assume $\beta X$ is a [zero-dimensional space](../../../zero-dimensional-space.md), and let $C,D$ be disjoint [closed subsets](../../../closed-set.md) of $X$. [Urysohn's lemma](../../../urysohn-s-lemma.md) gives $f:X\to[0,1]$ equal to zero on $C$ and one on $D$. Its continuous extension to $\beta X$ puts $\overline C^{\,\beta X}$ and $\overline D^{\,\beta X}$ in disjoint zero and one level sets. Using a clopen base, cover the first compact set by finitely many [clopen sets](../../../clopen-set.md) missing the second; their union $H$ is clopen and separates them. Thus $U=H\cap X$ and $V=X\setminus U$ are disjoint [clopen sets](../../../clopen-set.md) containing $C,D$.

Conversely, assume the stated clopen separation property on $X$. Let $A,B$ be disjoint [closed subsets](../../../closed-set.md) of $\beta X$. Normality supplies a [continuous function](../../../continuous-function.md) $f:\beta X\to[0,1]$ with $f|_A=0$, $f|_B=1$. The sets

$$
C=X\cap f^{-1}([0,1/3]),\qquad D=X\cap f^{-1}([2/3,1])
$$

are disjoint and closed in $X$. Select clopen $U\subseteq X$ containing $C$ and missing $D$; the given disjoint pair of clopen neighborhoods supplies such a $U$. Its [characteristic function](../../../characteristic-function-split.md), one on $U$ and zero outside, extends from $X$ to a [continuous map](../../../continuous-map.md) $\beta X\to\{0,1\}$. Let $H$ be its one level set, a [clopen set](../../../clopen-set.md).

Every $a\in A$ is in $\overline C^{\,\beta X}$: any neighborhood of $a$, intersected with $f^{-1}([0,1/3))$, is an [open neighborhood](../../../open-neighbourhood.md) meeting the dense set $X$. Likewise $B\subseteq\overline D^{\,\beta X}$. Since $C\subseteq H$ and $D\subseteq\beta X\setminus H$, it follows that $A\subseteq H$ and $B\cap H=\varnothing$.

Apply this to $A=\{z\}$ and $B=\beta X\setminus O$, for any point $z$ and [open neighborhood](../../../open-neighbourhood.md) $O$. It yields a clopen $H$ with $z\in H\subseteq O$, proving that $\beta X$ has a clopen base. Hence the [strong zero-dimensionality and Stone-Čech compactification](../../../strong-zero-dimensionality-and-stone-cech-compactification.md) criterion is

$$
\boxed{X\text{ has the stated clopen separation property}\iff\beta X\text{ is zero-dimensional}.}
$$

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2011](../../2011-split.md)
3. [Past exam of the analytic topology course of the University of Oxford](../../split.md)
4. [Analytic topology course of the University of Oxford](../../../analytic-topology-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
