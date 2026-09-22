<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A sufficient geometric form of the [Hahn-Banach separation theorem](../../../../../../hahn-banach-separation-theorem.md) is this: if $C$ is a nonempty closed [convex set](../../../../../../convex-set.md) in a real [normed vector space](../../../../../../normed-vector-space.md) and $x\notin C$, there exists a [continuous linear functional](../../../../../../continuous-linear-functional.md) $\ell$ such that

$$
\sup_{c\in C}\ell(c)<\ell(x).
$$

We use this form without proving it, as permitted. We will prove the [Krein-Milman theorem](../../../../../../krein-milman-theorem.md) for a nonempty compact [convex set](../../../../../../convex-set.md) $K$: **$K$ is the closed convex hull of its extreme points**.

First prove the existence of [extreme points](../../../../../../extreme-point.md) by the [minimal compact face argument](../../../../../../minimal-compact-face-argument.md). A [face of a convex set](../../../../../../face-of-a-convex-set.md) $K$ is a convex subset $F$ such that, whenever $ta+(1-t)b\in F$ with $a,b\in K$ and $0<t<1$, both $a$ and $b$ belong to $F$. Consider all nonempty compact faces of $K$, ordered by reverse inclusion. The set $K$ itself is such a face. A chain has a nonempty compact intersection, by the [finite intersection property](../../../../../../finite-intersection-property.md) and compactness of $K$. This intersection is convex and a face, since membership in every face forces the same membership of endpoints. It is an upper bound in the reverse order. The [Zorn lemma](../../../../../../zorn-s-lemma.md) therefore gives a minimal nonempty compact face $F$.

If $F$ contained distinct $a,b$, geometric separation of one point from the other would give a continuous real linear $\ell$ with $\ell(a)\ne\ell(b)$. Compactness supplies a maximum $m=\max_F\ell$. The set $F'=\{v\in F:\ell(v)=m\}$ is a nonempty proper compact convex subset. It is also a face of $K$: if a strict convex combination belongs to $F'$, first the face property of $F$ puts both endpoints in $F$, and then linearity and maximality of $m$ force both their values to equal $m$. Thus $F'$ contradicts minimality of $F$. Hence $F=\{e\}$, whose face property says precisely that $e$ is an [extreme point](../../../../../../extreme-point.md) of $K$. The same argument starts with any nonempty compact face, so every such face contains an [extreme point](../../../../../../extreme-point.md) of $K$.

Let $E$ be the set of all [extreme points](../../../../../../extreme-point.md) of $K$ and $C=\overline{\operatorname{conv}}E$. It is nonempty, and $C\subseteq K$ because $K$ is closed and convex. Suppose $x\in K\setminus C$. Geometric separation gives a continuous real linear $\ell$ with $\ell(x)>\sup_C\ell$. Let $m=\max_K\ell$ and consider the maximizer face $F=\{v\in K:\ell(v)=m\}$. It is nonempty, compact and a face of $K$, so the previous argument gives an extreme point $e\in F$. But $e\in E\subseteq C$, while

$$
\ell(e)=m\ge\ell(x)>\sup_C\ell,
$$

a contradiction. Therefore **every point of $K$ belongs to the closed convex hull of its extreme points**, proving

$$
\boxed{K=\overline{\operatorname{conv}}\operatorname{ext}K.}
$$

Neither completeness of the ambient normed space nor finite dimensionality was used; compactness is the key hypothesis.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
