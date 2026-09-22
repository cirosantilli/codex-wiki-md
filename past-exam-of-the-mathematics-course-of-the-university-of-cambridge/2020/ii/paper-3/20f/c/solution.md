<h1 id="20f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define a [simplicial map](../../../../../../simplicial-map.md) $j:K\to L$ on vertices by

$$
j(v_1)=v_1,qquad j(v_2)=v_2,qquad
j(v_3)=v_1,qquad j(v_4)=v_4.
$$

The image of every simplex is a simplex of $L$, and $j\circ i=\operatorname{id}_L$. The maps $i\circ j$ and $\operatorname{id}_K$ are [contiguous simplicial maps](../../../../../../contiguous-simplicial-maps.md), since the union of their images on every simplex is contained in a simplex of $K$. Their realizations are therefore homotopic, so $|j|$ is a [homotopy inverse](../../../../../../homotopy-inverse.md) of $|i|$.

Here is an explicit [chain homotopy](../../../../../../chain-homotopy.md). Put $f=i_\bullet j_\bullet$ and use the orientations from part (b). Define

$$
h_0(v_3)=e_{13},
\qquad h_0(v_1)=h_0(v_2)=h_0(v_4)=0,
$$



$$
h_1(e_{23})=t,
\qquad h_1(e_{12})=h_1(e_{13})=h_1(e_{14})=h_1(e_{24})=0,
\qquad h_2=0.
$$

We verify

$$
\partial h+h\partial=\operatorname{id}-f.
$$

It is immediate on every vertex except $v_3$, where $\partial h_0(v_3)=v_3-v_1=v_3-f(v_3)$. It is immediate on the fixed edges. For the remaining edges,

$$
(\partial h+h\partial)e_{13}=h_0(v_3-v_1)=e_{13}
=e_{13}-f(e_{13}),
$$



$$
(\partial h+h\partial)e_{23}
=\partial t+h_0(v_3-v_2)
=(e_{23}-e_{13}+e_{12})+e_{13}
=e_{23}+e_{12}
=e_{23}-f(e_{23}),
$$

because $f(e_{23})=[v_2v_1]=-e_{12}$. Finally,

$$
(\partial h+h\partial)t=h_1(e_{23}-e_{13}+e_{12})=t=t-f(t),
$$

since $f(t)$ is degenerate and hence zero. Thus $h$ is the required chain homotopy.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [20F](../../20f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
