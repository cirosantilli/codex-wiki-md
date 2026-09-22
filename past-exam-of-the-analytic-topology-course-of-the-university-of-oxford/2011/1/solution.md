<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**The extension.** [Urysohn's lemma](../../../urysohn-s-lemma.md) states that disjoint [closed subsets](../../../closed-set.md) $A,B$ of a [normal topological space](../../../normal-space.md) can be separated by a [continuous function](../../../continuous-function.md) $u:X\to[0,1]$ with $u|_A=0$ and $u|_B=1$.

For the bounded [Tietze extension theorem](../../../tietze-extension-theorem.md), first suppose $g:C\to[-M,M]$ is continuous. The subsets $A=\{g\leq-M/3\}$ and $B=\{g\geq M/3\}$ are closed in $X$, because $C$ is closed. [Urysohn's lemma](../../../urysohn-s-lemma.md) supplies a [continuous function](../../../continuous-function.md) $h:X\to[-M/3,M/3]$ with $h=-M/3$ on $A$ and $h=M/3$ on $B$. Directly checking the two outer ranges and the middle range of $g$ gives

$$
\|h\|_\infty\leq M/3,\qquad\|g-h|_C\|_\infty\leq2M/3.
$$

Empty level sets cause no difficulty: take the appropriate constant, or zero if both are empty. This is the [Urysohn two-thirds approximation](../../../urysohn-two-thirds-approximation.md).

Apply this successively to the residual on $C$, beginning with $f$ and $M_0=1$. We get $h_n$ with $\|h_n\|_\infty\leq\tfrac13(\tfrac23)^n$ and residual after the first $n$ terms at most $(2/3)^n$. The [Weierstrass M-test](../../../weierstrass-m-test.md) gives [uniform convergence](../../../uniform-convergence.md) of $F=\sum_{n\geq0}h_n$. By the [uniform limit theorem](../../../uniform-limit-theorem.md), $F$ is continuous; the residual bound proves $F|_C=f$, and the sum of the norm bounds is one. Thus

$$
\boxed{F:X\to[-1,1]\text{ is continuous and }F|_C=f.}
$$

**Closed sets as exact zero sets.** If $X$ is a [perfectly normal space](../../../perfectly-normal-space.md), write a closed $C$ as $\bigcap_{n\geq0}U_n$ with each $U_n$ open. Apply [Urysohn's lemma](../../../urysohn-s-lemma.md) to $C$ and $X\setminus U_n$ to obtain $f_n:X\to[0,1]$ vanishing on $C$ and equal to one on $X\setminus U_n$. The uniformly convergent series

$$
\boxed{f=\sum_{n\geq0}2^{-n-1}f_n\quad\text{satisfies}\quad f^{-1}(0)=C.}
$$

Indeed all summands vanish on $C$; outside $C$, at least one summand is strictly positive. The [uniform limit theorem](../../../uniform-limit-theorem.md) proves continuity. This realizes the [closed G-delta set as a zero set](../../../closed-g-delta-set-as-a-zero-set.md) construction.

Conversely, suppose each closed set is the [zero set of a continuous function](../../../zero-set-of-a-continuous-function.md). For disjoint closed $C,D$, select $f,g:X\to[0,1]$ with zero sets $C,D$. Their sum never vanishes, and

$$
\boxed{h=\frac{f}{f+g}:X\to[0,1],\qquad h^{-1}(0)=C,\quad h^{-1}(1)=D.}
$$

The quotient is continuous. This also proves normality by inverse images of disjoint endpoint neighborhoods. Each zero set is a [G-delta set](../../../g-delta-set.md), since $f^{-1}(0)=\bigcap_{n\geq1}f^{-1}([0,1/n))$; thus this property characterizes [perfectly normal spaces](../../../perfectly-normal-space.md) among [T1 spaces](../../../t1-space.md).

**Subspaces.** Let $Y\subseteq X$ and let $A,B$ be disjoint [closed subsets](../../../closed-set.md) of $Y$. Put $C=\overline A^{\,X}$ and $D=\overline B^{\,X}$. Since $C\cap Y=A$ and $D\cap Y=B$, the intersection $C\cap D$ misses $Y$. Choose [continuous functions](../../../continuous-function.md) $f,g$ on $X$ whose zero sets are $C,D$. On the [open neighborhood](../../../open-neighbourhood.md) $W=X\setminus(C\cap D)$ of $Y$, the same quotient $f/(f+g)$ is continuous and is zero on $A$, one on $B$. Its inverse images of $[0,1/3)$ and $(2/3,1]$, restricted to $Y$, are disjoint [open neighborhoods](../../../open-neighbourhood.md). Therefore **every subspace is a [normal topological space](../../../normal-space.md)**: [perfect normality implies hereditary normality](../../../perfect-normality-implies-hereditary-normality.md).

**A strict counterexample to the converse.** Let $D$ be an uncountable [discrete space](../../../discrete-space.md), and let $X=D\cup\{\infty\}$ be its [one-point compactification](../../../alexandroff-extension.md). Its neighborhoods of $\infty$ have finite complement in $D$, because compact subsets of a [discrete space](../../../discrete-space.md) are finite. The space is compact Hausdorff, hence a [T1 space](../../../t1-space.md) and normal. A subspace missing $\infty$ is discrete. A subspace containing $\infty$ is closed in $X$, since its complement is a subset of the open discrete part; it is therefore compact Hausdorff and normal. Thus all subspaces are normal.

But $\{\infty\}$ is not a [G-delta set](../../../g-delta-set.md). A countable intersection of its [open neighborhoods](../../../open-neighbourhood.md) omits at most countably many elements of $D$, and cannot omit all of uncountable $D$. Hence $X$ is not a [perfectly normal space](../../../perfectly-normal-space.md). This is the [uncountable discrete one-point compactification counterexample](../../../uncountable-discrete-one-point-compactification-counterexample.md).

## ↑ Ancestors (11)

1. [1](../1.md)
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
