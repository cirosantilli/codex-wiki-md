<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Begin with the [configuration model](../../../../../../configuration-model.md) for $n$ labelled vertices of degree $r$. Let $Y_\ell$ count [cycles in a graph](../../../../../../cycle-in-a-graph.md) with specified paired edges, so parallel-edge choices are counted separately before conditioning. Choose a cyclic ordering of $\ell$ distinct vertices in $(n)_\ell/(2\ell)$ ways, where division by $2\ell$ removes rotation and reversal. At each vertex choose an ordered pair of distinct [half-edges](../../../../../../half-edge-of-a-graph.md) for the entering and leaving edges, in $r(r-1)$ ways. These $\ell$ prescribed pairs appear with the pairing probability from part (i), giving

$$
\mathbb EY_\ell=\frac{(n)_\ell}{2\ell}\frac{[r(r-1)]^\ell}{(rn-1)(rn-3)\cdots(rn-2\ell+1)}\longrightarrow\frac{(r-1)^\ell}{2\ell}.
$$

It remains to justify conditioning on simplicity: merely dividing by a positive simplicity probability would give an incorrect constant.

Unconditionally, part (i) with no forbidden graph has $\lambda=r-1$, so

$$
\Pr(\text{simple})=\exp\left(-\frac{r-1}{2}-\frac{(r-1)^2}{4}\right)+o(1).
$$

Condition on one specified cycle pairing. The unpaired half-edges form a uniform [configuration model](../../../../../../configuration-model.md) with degree $r-2$ at its $\ell$ vertices and degree $r$ elsewhere. A completion of the full graph is simple exactly when the residual graph is simple and has no additional edge along one of the already prescribed cycle edges. This forbidden graph has [maximum degree](../../../../../../maximum-degree.md) two. Because $r,\ell$ are fixed,

$$
M'=rn-2\ell,\qquad \lambda'=r-1+O(1/n),\qquad \mu'=O(1/n).
$$

After permuting labels if needed to sort the degrees, the assumptions of part (i) still hold, including residual degrees at least one. Its [bounded-degree pairing avoidance estimate](../../../../../../bounded-degree-pairing-avoidance-estimate.md) therefore shows that

$$
\frac{\Pr(\text{simple}\mid\text{specified cycle pairs})}{\Pr(\text{simple})}\longrightarrow1.
$$

This ratio is the same for each prescribed cycle, by symmetry. Sum over their indicators to obtain $\mathbb E(Y_\ell\mid\text{simple})=(1+o(1))\mathbb EY_\ell$. Conditioning is uniform over all simple $r$-regular graphs because each has $(r!)^n$ pairing representations. On simplicity, $Y_\ell$ is the ordinary cycle count. Hence the [short-cycle expectation in a uniform regular graph](../../../../../../short-cycle-expectation-in-a-uniform-regular-graph.md) is

$$
\boxed{\mathbb E C_\ell(G_{n,r\text{-reg}})\longrightarrow\frac{(r-1)^\ell}{2\ell}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
