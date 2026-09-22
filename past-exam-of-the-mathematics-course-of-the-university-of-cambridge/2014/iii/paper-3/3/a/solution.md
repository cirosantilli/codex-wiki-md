<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [extension group](../../../../../../extension-group.md) $\operatorname{Ext}^1_Q(V,W)$ consists of equivalence classes of [short exact sequences](../../../../../../short-exact-sequence.md) $0\to W\to E\to V\to0$, with the zero class represented by a split sequence and addition given by the [Baer sum](../../../../../../baer-sum.md). The [extension complex of quiver representations](../../../../../../extension-complex-of-quiver-representations.md) gives

$$
0\to\operatorname{Hom}_Q(V,W)\to\bigoplus_i\operatorname{Hom}_k(V_i,W_i)\xrightarrow{\gamma_{V,W}}\bigoplus_{\rho:i\to j}\operatorname{Hom}_k(V_i,W_j)\to\operatorname{Ext}^1_Q(V,W)\to0.
$$

The printed map has $\gamma(u)_\rho=u_jf_\rho-g_\rho u_i$, so its [kernel](../../../../../../kernel-of-a-linear-map.md) is $\operatorname{Hom}_Q(V,W)$ and its [cokernel](../../../../../../cokernel.md) is $\operatorname{Ext}^1_Q(V,W)$. Reversing the overall differential sign changes neither identification.

For dimension vectors $\mathbf v,\mathbf w$, the [Ringel form](../../../../../../ringel-form.md) is

$$
\boxed{\langle\mathbf v,\mathbf w\rangle_Q=\sum_iv_iw_i-\sum_{\rho:i\to j}v_iw_j=\dim\operatorname{Hom}_Q(V,W)-\dim\operatorname{Ext}^1_Q(V,W)}.
$$

The first expression makes its dependence only on the dimension vectors explicit.

For the one-loop representation $V=k$ with loop scalar $\lambda$, $\gamma(u)=u\lambda-\lambda u=0$ on $k$. Both cochain spaces have dimension one, so **$\dim\operatorname{Ext}^1_Q(V,V)=1$**, for every $\lambda$. Concretely, a self-extension has loop matrix $\left(\begin{smallmatrix}\lambda&c\\0&\lambda\end{smallmatrix}\right)$, with $c$ the extension parameter.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
