<h1 id="3/iii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the [standard perturbation theory velocity kernel](../../../../../../../standard-perturbation-theory-velocity-kernel.md) by

$$
\theta^{(n)}(\mathbf k)=\int_{\mathbf q_1\cdots\mathbf q_n}
(2\pi)^3\delta_D\left(\mathbf k-\sum_a\mathbf q_a\right)
G_n(\mathbf q_1,\ldots,\mathbf q_n)\prod_a\delta_1(\mathbf q_a),
$$

where $\int_{\mathbf q}=\int d^3q/(2\pi)^3$ and $P(q)=\langle|\delta_1(\mathbf q)|^2\rangle'$. For $\mathbf k_1+\mathbf k_2+\mathbf k_3=0$, one representative external labelling of the tree contribution is

$$
\boxed{B_{211}=2G_2(\mathbf k_1,\mathbf k_2)P(k_1)P(k_2)}.
$$

The four one-loop representatives are

$$
\boxed{B_{222}=8\int_{\mathbf q}
G_2(-\mathbf q,\mathbf q+\mathbf k_1)
G_2(-\mathbf q-\mathbf k_1,\mathbf q-\mathbf k_2)
G_2(\mathbf k_2-\mathbf q,\mathbf q)
P(q)P(|\mathbf q+\mathbf k_1|)P(|\mathbf q-\mathbf k_2|)},
$$



$$
\boxed{B_{321}^{I}=6P(k_3)\int_{\mathbf q}
G_3(-\mathbf k_3,-\mathbf q,\mathbf q-\mathbf k_2)
G_2(\mathbf q,\mathbf k_2-\mathbf q)
P(q)P(|\mathbf k_2-\mathbf q|)},
$$



$$
\boxed{B_{321}^{II}=6P(k_1)P(k_3)G_2(\mathbf k_1,\mathbf k_3)
\int_{\mathbf q}G_3(\mathbf k_1,\mathbf q,-\mathbf q)P(q)},
$$



$$
\boxed{B_{411}=12P(k_2)P(k_3)
\int_{\mathbf q}G_4(-\mathbf k_2,-\mathbf k_3,\mathbf q,-\mathbf q)P(q)}.
$$

The full answer adds the distinct permutations of the external labels; the question asks for only one labelling of each topology.

<a id="3/iii/b/image-tree-and-one-loop-matter-bispectrum-topologies"></a>
![](../../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-312-one-loop-matter-bispectrum.png)

**[Figure 1](#3/iii/b/image-tree-and-one-loop-matter-bispectrum-topologies). Tree and one-loop matter-bispectrum topologies**. The five panels show representative external labellings of B211, B222, the two B321 topologies, and B411. Filled dots denote perturbation-theory vertices and colored internal lines make the loop structures visible.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Iii](../../iii.md)
3. [3](../../../3.md)
4. [Paper 312](../../../../paper-312-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
