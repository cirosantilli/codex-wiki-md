<h1 id="21j/solution">Solution</h1>

↑ **Parent:** [21J](../21j.md)

For $K=M\cup N$, the simplicial Mayer--Vietoris [sequence](../../../../../sequence.md) is

$$
\cdots\to H_i(M\cap N)\xrightarrow{(j_*,-k_*)}
H_i(M)\oplus H_i(N)\to H_i(K)
\xrightarrow{\partial}H_{i-1}(M\cap N)\to\cdots.
$$

Construct a simplicial mapping cone of a degree-$k$ map of a circle. Explicitly, let the target circle have vertices $v_0,v_1,v_2$, and let the source circle have vertices $w_0,\ldots,w_{3k-1}$. Map $w_j$ to $v_{j\bmod3}$, triangulate each quadrilateral of its mapping cylinder, and cone the source circle to one new vertex. The resulting finite simplicial complex is the mapping cone $K_k$.

Its reduced cellular, or equivalently simplicial, chain complex collapses to

$$
0\to\mathbb Z\xrightarrow{\times k}\mathbb Z\to0
$$

in degrees two and one. Consequently

$$
H_i(K_k)\cong
\begin{cases}
\mathbb Z,&i=0,\\
\mathbb Z/k,&i=1,\\
0,&\text{otherwise}.
\end{cases}
$$

The same computation follows from Mayer--Vietoris applied to the cone and the mapping-cylinder neighborhood.

## ↑ Ancestors (10)

1. [21J](../21j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
