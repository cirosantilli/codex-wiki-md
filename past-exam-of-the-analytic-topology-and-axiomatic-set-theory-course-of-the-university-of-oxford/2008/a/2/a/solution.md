<h1 id="a/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For each point which belongs to at least one $U_t$, its membership-index [set](../../../../../set-split.md) is a nonempty [subset](../../../../../subset.md) of $[0,1]$, so has an infimum in $[0,1]$. Assigning the value one to the other points therefore defines $f:X\to[0,1]$ everywhere.

For $0<r\le1$,

$$
\{x:f(x)<r\}=\bigcup_{t\in D,\ t<r}U_t.
$$

An index $t<r$ gives $f(x)\le t<r$. Conversely if the infimum is below $r$, some membership index must be below $r$. Thus this strict sublevel [set](../../../../../set-split.md) is [open](../../../../../open-set.md).

For $0\le r<1$ we claim

$$
\{x:f(x)>r\}=\bigcup_{t\in D,\ t>r}(X\setminus\overline{U_t}).
$$

If $x\notin\overline{U_t}$ and $t>r$, then $x$ cannot belong to any $U_s$ with $s\le t$, since $U_s\subseteq U_t$ for $s<t$. Hence $f(x)\ge t>r$. Conversely, if $f(x)>r$, density of $D$ supplies $r<t<u<f(x)$ with $t,u\in D$. Since $x\notin U_u$ and $\overline{U_t}\subseteq U_u$, one has $x\notin\overline{U_t}$. This proves the identity, and its right-hand side is [open](../../../../../open-set.md).

The remaining sublevel and superlevel [sets](../../../../../set-split.md), for thresholds outside these ranges, are either empty or all of $X$. Preimages of [open](../../../../../open-set.md) rays are consequently [open](../../../../../open-set.md), and these rays generate the usual real [topology](../../../../../topology-split.md). Therefore **$f$ is [continuous](../../../../../continuous-function.md)**. The [closure](../../../../../closure-topology.md) inclusion is what supplies openness of the strict superlevel [sets](../../../../../set-split.md); mere nesting would not suffice.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../split.md)
6. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
