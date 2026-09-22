# Conjugacy classes of the symmetric group on three letters

↑ **Parent:** [Conjugacy class](conjugacy-class.md)

The [symmetric group](symmetric-group.md) $S_3$ has exactly six [permutations](permutation.md), written using [permutation cycles](permutation-cycle.md):

$$
S_3=\{e,(12),(13),(23),(123),(132)\}.
$$

Here $e$ is the [identity element](identity-element.md); $(12)$, $(13)$ and $(23)$ are [transpositions](transposition-permutation.md); and $(123)$ and $(132)$ are [permutation cycles](permutation-cycle.md) of length three. With $t=(12)$ and $r=(123)$, rightmost-first [function composition](function-composition.md) gives $r^2=(132)$ and $r^{-1}=r^2$. The [conjugacy classes](conjugacy-class.md) and representative [centralizers](centralizer.md) are

$$
\begin{array}{c|c|c|c}
x&\operatorname{Cl}_{S_3}(x)&C_{S_3}(x)&|\operatorname{Cl}_{S_3}(x)|\\
\hline
e&\{e\}&S_3&6/6=1\\
t&\{(12),(13),(23)\}&\{e,t\}&6/2=3\\
r&\{(123),(132)\}&\{e,r,r^2\}&6/3=2
\end{array}
$$

<a id="image-all-six-permutations-of-the-symmetric-group-s-3-their-conjugacy-classes-and-representative-centralizers"></a>
![](s3-conjugacy-classes.png)

**[Figure 6](#image-all-six-permutations-of-the-symmetric-group-s-3-their-conjugacy-classes-and-representative-centralizers). All six permutations of the symmetric group $S_3$, their conjugacy classes, and representative centralizers**.

An explicit check of the [conjugation](conjugation.md) $gtg^{-1}$ with $g=r=(123)$ sends $1\mapsto3\mapsto3\mapsto1$, $2\mapsto1\mapsto2\mapsto3$, and $3\mapsto2\mapsto1\mapsto2$, where each chain applies $g^{-1}$, then $t$, then $g$. Thus $1$ is fixed and $2,3$ are exchanged: $gtg^{-1}=(23)$. Relabelling also produces $(13)$, so the three [transpositions](transposition-permutation.md) share one [conjugacy class](conjugacy-class.md). A [transposition](transposition-permutation.md) reverses the length-three [permutation cycle](permutation-cycle.md), since $trt^{-1}=(213)=(132)=r^{-1}$, putting both length-three [permutation cycles](permutation-cycle.md) in one [conjugacy class](conjugacy-class.md).

Checking each of the six possible [permutations](permutation.md) against $gx=xg$ gives the displayed [centralizers](centralizer.md). Only $e$ has a one-element [conjugacy class](conjugacy-class.md), so the [center of a group](center-of-a-group.md) here is $Z(S_3)=\{e\}$. The [class equation](class-equation.md) is $6=1+3+2$. The second diagram in [centralizer and normalizer](centralizer-and-normalizer.md) uses the same $r$ and $t$ to show how preserving a [cyclic subgroup](cyclic-subgroup.md) differs from fixing its [group generator](generator-of-a-group.md).

## ↑ Ancestors (8)

1. [Conjugacy class](conjugacy-class.md)
2. [Conjugation action](conjugation-action.md)
3. [Group action](group-action-split.md)
4. [Group theory](group-theory-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Centralizer](centralizer.md)
- [Class equation](class-equation.md)
- [Conjugacy class](conjugacy-class.md)
- [Normal subgroups and quotients of the symmetric group on three letters](normal-subgroups-and-quotients-of-the-symmetric-group-on-three-letters.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-2/9/c/solution.md)
