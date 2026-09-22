<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [categorical limit](../../../../../categorical-limit.md) of $D:\mathcal J\to\mathcal C$ is a terminal cone: it consists of an object $L$ and compatible maps $L\to D(j)$ through which every other cone factors uniquely. For a finite diagram, take the product $P=\prod_jD(j)$ and the product $Q=\prod_{u:i\to j}D(j)$. There are two maps $P\rightrightarrows Q$: on the $u:i\to j$ coordinate one uses respectively $D(u)$ after projection to $D(i)$ and direct projection to $D(j)$. Their [equalizer](../../../../../equaliser.md) is exactly the compatible-cone object. Hence finite products and equalizers construct every [finite limit](../../../../../finite-limit.md).

In the [category of metric spaces and non-expansive maps](../../../../../category-of-metric-spaces-and-non-expansive-maps.md), give $X\times Y$ the maximum metric

$$
d((x,y),(x',y'))=\max\{d_X(x,x'),d_Y(y,y')\}.
$$

The projections are non-expansive, and a pair of non-expansive maps into $X$ and $Y$ induces a non-expansive map into this product, proving the universal property.

Let two maps $1\rightrightarrows X$ select $a,b\in X$. On the set quotient identifying $a$ and $b$, define the [quotient metric](../../../../../quotient-metric.md) by shortest paths that may jump from $a$ to $b$ at zero cost. Explicitly,

$$
d_Q([x],[y])=min\{d(x,y),d(x,a)+d(b,y),d(x,b)+d(a,y)\}.
$$

This is the largest metric making the quotient map non-expansive. A map $X\to Z$ equalizing $a$ and $b$ factors through the set quotient and remains non-expansive by the path formula, so this is the coequalizer. Its underlying set is the set-theoretic coequalizer.

For $X=\{0,1,5,6\}$ with $0\sim6$, write $*=\{0,6\}$. The quotient has

$$
d_Q(*,1)=d_Q(*,5)=1,
\qquad d_Q(1,5)=2.
$$

Thus in $Q\times Y$, with $Y=\{0,3\}$,

$$
d_{Q\times Y}((1,0),(5,3))=\max\{2,3\}=3.
$$

After first taking $X\times Y$, the product of the parallel pair identifies $(0,y)$ with $(6,y)$ separately for $y=0,3$. In its quotient metric, every path from $(1,0)$ to $(5,3)$ has length at least $4$, and length $4$ is attained either directly or via one of those identifications. The canonical bijection from this coequalizer to $Q\times Y$ is therefore not an isometry. Hence $-\times Y$ does not preserve this coequalizer. In a [Cartesian closed category](../../../../../cartesian-closed-category.md), $-\times Y$ is a left adjoint and preserves all colimits, so $\mathbf{Met}$ is not cartesian closed.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
