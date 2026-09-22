<h1 id="7e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [group action](../../../../../../group-action.md), the [orbit of a group action](../../../../../../orbit-of-a-group-action.md) of $x$ is $Gx=\{gx:g\in G\}$, and its [stabilizer subgroup](../../../../../../stabilizer-subgroup.md) is $G_x=\{g:gx=x\}$. The [orbit-stabilizer theorem](../../../../../../orbit-stabilizer-theorem.md) gives $|Gx||G_x|=|G|$: the map $gG_x\mapsto gx$ is a well-defined [bijection](../../../../../../bijection.md) from stabilizer [cosets](../../../../../../coset.md) to the orbit.

Within one orbit, the [stabilizer subgroups](../../../../../../stabilizer-subgroup.md) are conjugate, since $G_{hx}=hG_xh^{-1}$. Their sizes are therefore equal. Summing stabilizer sizes over a single orbit gives $|Gx||G_x|=|G|$, and summing over all $n$ orbits yields

$$
\boxed{\sum_{x\in X}|\operatorname{Stab}(x)|=n|G|.}
$$

Now count the pairs $(g,x)$ fixed by the action in two ways. Holding $x$ fixed gives $|G_x|$ choices of $g$, whereas holding $g$ fixed gives $|\operatorname{Fix}(g)|$ choices of $x$. Thus

$$
|S|=\sum_{x\in X}|G_x|=\sum_{g\in G}|\operatorname{Fix}(g)|.
$$

Combining the two identities proves [Burnside lemma](../../../../../../burnside-s-lemma.md):

$$
\boxed{n=\frac1{|G|}\sum_{g\in G}|\operatorname{Fix}(g)|.}
$$

The finiteness hypotheses justify these cardinality sums. If $X$ is empty, every sum and the orbit count are zero, so the formula still applies.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7E](../../7e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
