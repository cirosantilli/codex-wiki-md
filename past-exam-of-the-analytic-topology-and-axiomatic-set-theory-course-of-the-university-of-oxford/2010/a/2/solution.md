<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For $y\in Y$, every neighborhood of $y$ in the subspace is of the form $V\cap Y$ with $V$ an ambient [open neighborhood](../../../../open-neighbourhood.md). Since $A\subseteq Y$, this meets $A$ exactly when $V$ meets $A$. Thus

$$
\boxed{\overline A^{\,Y}=Y\cap\overline A^{\,X}.}
$$

A [Hausdorff compactification](../../../../hausdorff-compactification.md) is a [topological embedding](../../../../topological-embedding.md) $h:X\to K$ with [dense](../../../../dense-set.md) image in a [compact Hausdorff space](../../../../compact-hausdorff-space.md) $K$. Define the domination preorder by

$$
\boxed{(h,K)\leq(h',K')\ \Longleftrightarrow\ \exists q:K'\to K\text{ continuous with }q\circ h'=h.}
$$

It is reflexive by the identity map and transitive by composition. Any comparison map is onto: its image is [compact](../../../../compact-space.md) and hence closed in $K$, and contains the [dense](../../../../dense-set.md) set $h(X)$. Two compactifications are equivalent if a [homeomorphism](../../../../homeomorphism.md) $u:K\to K'$ satisfies $u\circ h=h'$.

Such a [homeomorphism](../../../../homeomorphism.md) and its inverse give domination both ways. Conversely, if comparison maps exist in both directions, each composite agrees with the identity on the [dense](../../../../dense-set.md) embedded copy of $X$. Two [continuous maps](../../../../continuous-map.md) to a [Hausdorff](../../../../hausdorff-space.md) space agreeing on a [dense](../../../../dense-set.md) set agree everywhere. The comparison maps are therefore inverse [homeomorphisms](../../../../homeomorphism.md). Thus equivalence is exactly mutual domination.

The [Stone-Čech extension property](../../../../stone-cech-extension-property.md) says that every [continuous map](../../../../continuous-map.md) from $X$ into any [compact Hausdorff space](../../../../compact-hausdorff-space.md) extends continuously to the compactification. The extension is unique by density. For two compactifications with this property, extend each embedding through the other compactification. This gives comparison maps both ways, hence equivalence by the preceding argument.

For the [perfect-map characterization by Stone-Čech remainders](../../../../perfect-map-characterization-by-stone-cech-remainders.md), the universal property first gives a unique continuous $F:\beta X\to\beta Y$ extending the composite $X\xrightarrow fY\hookrightarrow\beta Y$. The required remainder condition is equivalent to

$$
\boxed{F^{-1}(Y)=X.}
$$

One inclusion is already forced by the extension property; the other forbids any point of the remainder mapping into $Y$.

Suppose first that $f$ is a [perfect map](../../../../perfect-map.md). Fix $y\in Y$ and let $K=f^{-1}(y)$, a [compact subset](../../../../compact-space.md) of $X$ and hence a [closed subset](../../../../closed-set.md) of $\beta X$. If $p\in F^{-1}(y)\setminus K$, normality of $\beta X$ supplies an open $U$ with $K\subseteq U$ and $p\notin\overline U$. Because $f$ is closed,

$$
V=Y\setminus f(X\setminus U)
$$

is an [open neighborhood](../../../../open-neighbourhood.md) of $y$ and $f^{-1}(V)\subseteq U\cap X$. Choose an open $V'$ of $\beta Y$ with $V'\cap Y=V$. The [open set](../../../../open-set.md) $F^{-1}(V')$ contains $p$, and its [intersection](../../../../set-intersection.md) with the [dense](../../../../dense-set.md) subset $X$ lies in $U$. Every point of that [open set](../../../../open-set.md) is consequently in $\overline U$, contradicting the choice of $p$. Therefore $F^{-1}(y)=K\subseteq X$ for every $y\in Y$, proving the remainder condition. This argument also handles an empty [fiber](../../../../fiber-of-a-function.md).

Conversely suppose the remainder condition holds. Every [fiber](../../../../fiber-of-a-function.md) $f^{-1}(y)=F^{-1}(y)$ is a [closed subset](../../../../closed-set.md) of $\beta X$, hence [compact](../../../../compact-space.md), and lies in $X$. To show that $f$ is closed, let $A$ be closed in $X$ and set $D=\overline A^{\,\beta X}$. The initial [closure](../../../../closure-topology.md) identity gives $D\cap X=A$. [Compactness](../../../../compact-space.md) makes $F(D)$ closed in $\beta Y$, and the remainder condition gives

$$
f(A)=F(D)\cap Y.
$$

Indeed any preimage in $D$ of a point of $Y$ must belong to $X$ and hence to $A$. Thus $f(A)$ is closed in $Y$. Together with [compact](../../../../compact-space.md) [fibers](../../../../fiber-of-a-function.md) this proves

$$
\boxed{f\text{ perfect}\ \Longleftrightarrow\ F(\beta X\setminus X)\subseteq\beta Y\setminus Y.}
$$

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../split.md)
5. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
