<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**The printed assertion is false in the usual pointwise meaning of nowhere continuous.** The original PDF explicitly has this wording. Part (c) proves that $S$ has nondecreasing càdlàg paths; such paths can have only countably many discontinuities, so they are continuous at uncountably many levels. We prove the precise valid statement:

$$
\boxed{\text{Almost surely, }S\text{ has a countable dense set of jump levels and is continuous at every other level.}}
$$

For countability, fix a path and a bounded level interval $[0,K]$. A discontinuity is a jump $S_a-S_{a-}>0$, since right continuity is already known. The sum of any finite family of these jumps is at most $S_K-S_0$. Thus there are only finitely many jumps of size at least $1/j$, for each positive integer $j$. Taking the countable union over $j$ and over integer $K$ proves that all discontinuities form a countable set.

For density, work on the common probability-one event of Brownian continuity, unboundedness above, and the conclusion of part (a). The inverse $S$ is strictly increasing: for every level $a$, path continuity gives $X_{S_a}=a$, so two distinct levels cannot have the same passage time. Suppose there were a nonempty open level interval on which $S$ had no discontinuity. Choose $0<a<b$ inside it. Its restriction to $[a,b]$ would be continuous and strictly increasing, hence onto $[S_a,S_b]$. For every time $t$ in this positive-length interval there would be a unique $c\in[a,b]$ with $t=S_c$, and then $X_t=X_{S_c}=c$. Increasing $t$ increases $c$, so the Brownian path would be nondecreasing throughout $[S_a,S_b]$. This contradicts part (a).

Therefore every open level interval contains a jump. This establishes [Countable dense jumps of the Brownian first-passage subordinator](../../../../../../countable-dense-jumps-of-the-brownian-first-passage-subordinator.md), and in particular rules out any interval on which $S$ is continuous throughout. It does not rule out continuity at an individual level. In fact, for every fixed deterministic $a>0$, part (b) gives $S_a=H_a=S_{a-}$ almost surely, so $S$ is almost surely continuous at that specified level. Its dense discontinuities occur at random levels.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
