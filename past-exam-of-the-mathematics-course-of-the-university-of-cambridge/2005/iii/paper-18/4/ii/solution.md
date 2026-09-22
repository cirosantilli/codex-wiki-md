<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [based path space and the path-loop fibration](../../../../../../based-path-space-and-the-path-loop-fibration.md) $\Omega S^r\to PS^r\to S^r$, where paths begin at a fixed basepoint and the projection evaluates their final endpoint. The total space is contractible: the [homotopy](../../../../../../homotopy.md) $\gamma(t)\mapsto\gamma(st)$, $s\downarrow0$, contracts every path to the constant path. The fiber is path-connected because $S^r$ is simply connected. Hence $H_0(\Omega S^r)=\mathbb Z$ and all positive [homology](../../../../../../homology-split.md) of $PS^r$ vanishes.

The [exact sequence](../../../../../../exact-sequence.md) from part (i), for $i\geq2$, gives $H_{i-r}(\Omega S^r)\cong H_{i-1}(\Omega S^r)$. Put $d=r-1$. Taking negative-degree [homology](../../../../../../homology-split.md) to be zero, this says $H_j\cong H_{j-d}$ for every $j\geq1$. Starting with $H_0=\mathbb Z$ determines every group:

$$
\boxed{H_j(\Omega S^r;\mathbb Z)=\begin{cases}\mathbb Z,&j\geq0\text{ and }d\mid j,\\0,&\text{otherwise}.\end{cases}}
$$

There are no torsion groups hidden in the recurrence, since each step is an actual integral isomorphism. This is the [integral homology of the loop space of a sphere](../../../../../../integral-homology-of-the-loop-space-of-a-sphere.md).

Choose the unit map $\eta:S^{r-1}\to\Omega S^r$ adjoint to the identity under $\Sigma S^{r-1}\cong S^r$. Loop adjunction gives $\pi_j(\Omega S^r)\cong\pi_{j+1}(S^r)$, so the [loop space](../../../../../../loop-space.md) is $(r-2)$-connected and $\pi_{r-1}(\Omega S^r)\cong\mathbb Z$. The adjoint of $\eta$ is the degree-one identity, so $\eta$ sends the generator of $\pi_{r-1}(S^{r-1})$ to that generator. The [Hurewicz theorem](../../../../../../hurewicz-theorem.md) for both $(r-2)$-connected spaces, and its naturality, then show that $\eta_*$ is an isomorphism on $H_{r-1}$. It also is on $H_0$, since both spaces are connected. All other positive degrees below $2r-2$ vanish in both spaces. Thus

$$
\boxed{\eta_*:H_j(S^{r-1};\mathbb Z)\xrightarrow{\cong}H_j(\Omega S^r;\mathbb Z),\qquad j\leq2r-3.}
$$

This proves the required existence with a specific map, without using the [suspension](../../../../../../suspension-topology.md) theorem in advance.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
