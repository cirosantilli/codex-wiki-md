<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $K=\ker f_\rho$ and $C=Y_j/\operatorname{im}g_\rho$. Consider the map from the arrow term of the [extension complex of quiver representations](../../../../../../extension-complex-of-quiver-representations.md) to $\operatorname{Hom}_k(K,C)$ that restricts its $\rho$-component to $K$ and then takes the quotient in $Y_j$. This map is surjective: a map $K\to C$ can be lifted to $Y_j$ and extended from $K$ to $X_i$.

Every coboundary is killed by this map, since for $x\in K$,

$$
(\delta h)_\rho(x)=g_\rho h_i(x)-h_jf_\rho(x)=g_\rho h_i(x)\in\operatorname{im}g_\rho.
$$

It therefore induces a surjection

$$
\operatorname{Ext}^1_Q(X,Y)\twoheadrightarrow\operatorname{Hom}_k(\ker f_\rho,\operatorname{coker}g_\rho).
$$

Both vector spaces in the final [Hom functor](../../../../../../hom-functor.md) are nonzero, so its dimension is positive. Hence **$\operatorname{Ext}^1_Q(X,Y)\ne0$**. This is the [kernel-cokernel obstruction to splitting a quiver extension](../../../../../../kernel-cokernel-obstruction-to-splitting-a-quiver-extension.md) and remains valid for loops and repeated arrows elsewhere in the [quiver](../../../../../../quiver.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
