<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Take the diagonal [Cartan subalgebra](../../../../../cartan-subalgebra.md) of $\mathfrak{sl}_3$ and let $\varepsilon_i$ select its $i$th diagonal entry, so $\varepsilon_1+\varepsilon_2+\varepsilon_3=0$ on it. Use [simple roots](../../../../../simple-root.md) $\alpha_1=\varepsilon_1-\varepsilon_2$, $\alpha_2=\varepsilon_2-\varepsilon_3$. The [fundamental weights](../../../../../fundamental-weight.md) are $\omega_1=\varepsilon_1$ and $\omega_2=-\varepsilon_3=\varepsilon_1+\varepsilon_2$. The defining representation $V$ has highest vector $e_1$ and the dual has highest vector $e_3^*$. Thus

$$
\boxed{\operatorname{hw}(V)=\omega_1,\qquad\operatorname{hw}(V^*)=\omega_2.}
$$

Their [crystal basis](../../../../../crystal-basis.md) diagrams are $B:1\xrightarrow{1}2\xrightarrow{2}3$ and $B^\vee:\bar3\xrightarrow{2}\bar2\xrightarrow{1}\bar1$, with weights $\varepsilon_i$ and $-\varepsilon_i$ respectively. Use the same [crystal tensor-product rule](../../../../../crystal-tensor-product-rule.md) as in2(d): lowering acts on the first factor when $\varphi_i(u)>\varepsilon_i(v)$; otherwise on the second. Raising uses the first factor when $\varphi_i(u)\ge\varepsilon_i(v)$, so it reverses each lowering arrow. An edge is absent if the selected factor operation is zero.

For $B\otimes B$, abbreviate $i\otimes j$ by $ij$. The complete color-one edge list is $11\to21\to22$, $31\to32$, $13\to23$; the complete color-two list is $21\to31$, $22\to32\to33$, $12\to13$. There are two connected components:

$$
\begin{array}{c|c|c}
\text{highest vertex}&\text{all vertices}&\text{highest weight}\\\hline
11&11,21,22,31,32,33&2\omega_1\\
12&12,13,23&\omega_2
\end{array}
$$

For example $\widetilde f_1(1\otimes1)=2\otimes1$ because $\varphi_1(1)=1>\varepsilon_1(1)=0$, whereas $\widetilde f_1(1\otimes2)=0$ because equality selects the second factor and $\widetilde f_1(2)=0$. This explains which ordered tensor labels lie in each component. At the representation level, the two components are the six-dimensional [symmetric square](../../../../../symmetric-square.md) and the three-dimensional [exterior square](../../../../../exterior-square.md):

$$
\boxed{V\otimes V\cong L(2\omega_1)\oplus L(\omega_2).}
$$

For $B\otimes B^\vee$, abbreviate $i\otimes\bar j$ by $i\bar j$. The complete color-one edge list is $1\bar3\to2\bar3$, $1\bar2\to2\bar2\to2\bar1$, $3\bar2\to3\bar1$; the complete color-two list is $1\bar3\to1\bar2$, $2\bar3\to3\bar3\to3\bar2$, $2\bar1\to3\bar1$. The isolated vertex is $1\bar1$. Thus the two highest vertices are $1\bar3$ of weight $\varepsilon_1-\varepsilon_3=\omega_1+\omega_2$, and $1\bar1$ of weight zero. Lowering from the former visits all eight other vertices. Consequently

$$
\boxed{V\otimes V^*\cong L(\omega_1+\omega_2)\oplus L(0).}
$$

This also follows concretely from $V\otimes V^*\cong\operatorname{End}(V)=\mathfrak{sl}_3\oplus\mathbb C I$: the first term is the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md), with highest weight the highest root, and the second is the [trivial Lie algebra representation](../../../../../trivial-lie-algebra-representation.md). The ordinary invariant vector is $\sum_i e_i\otimes e_i^*$, not the bare tensor suggested by the singleton's crystal label. The explicit edge lists and the diagrams exhibit all eighteen tensor vertices and justify the four highest weights.

<a id="3/image-all-components-of-the-defining-a2-tensor-square-and-defining-tensor-dual-crystals-with-every-lowering-edge-labeled-by-its-simple-root-color"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-5-a2-tensors.png)

**[Figure 3](#3/image-all-components-of-the-defining-a2-tensor-square-and-defining-tensor-dual-crystals-with-every-lowering-edge-labeled-by-its-simple-root-color). All components of the defining A2 tensor square and defining tensor dual crystals, with every lowering edge labeled by its simple-root color**.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
