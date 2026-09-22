<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Discard ground points lying in no set. For every point $x$ that lies in at least two members, form

$$
L_x=\{i:x\in A_i\}\subseteq[n].
$$

Every pair of indices lies in exactly one $L_x$, and no $L_x$ equals $[n]$ because the total intersection is empty. Thus the $L_x$ form a [finite linear space](../../../../../../finite-linear-space.md) on the $n$ indices. The number of its lines through index $i$ is at most $a_i$, with equality unless $A_i$ contains private points.

The [De Bruijn--Erdos pair-covering inequality](../../../../../../de-bruijn-erdos-pair-covering-inequality.md) says that if $r_i$ is the number of lines through point $i$ in a nontrivial finite linear space on $n$ points, then

$$
\sum_{i=1}^n\binom{r_i}{2}\geq\binom n2.
$$

Applying it here gives

$$
\sum_{i=1}^n\binom{a_i}{2}
\geq\sum_{i=1}^n\binom{r_i}{2}
\geq\binom n2.
$$

Moreover, a pair of ground points can lie in at most one $A_i$, since two different members meet in only one point. Hence

$$
\sum_i\binom{a_i}{2}\leq\binom m2.
$$

Combining the inequalities gives $\binom m2\geq\binom n2$, and therefore $m\geq n$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
