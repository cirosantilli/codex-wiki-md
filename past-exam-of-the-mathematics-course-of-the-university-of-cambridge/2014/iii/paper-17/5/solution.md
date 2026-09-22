<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use the convention that a [Hermitian metric](../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md) $h$ is complex-linear in its first argument and conjugate-linear in its second. It is a smoothly varying [positive-definite](../../../../../positive-definite-bilinear-form.md) [Hermitian form](../../../../../hermitian-form.md) on each fibre. A [connection on a vector bundle](../../../../../connection-vector-bundle.md) is a complex-linear operator $D:\Gamma(E)\to\Omega^1(X,E)$ satisfying $D(as)=da\otimes s+aDs$ for smooth complex functions $a$. Metric compatibility means, for every real [vector field](../../../../../vector-field.md) $V$,

$$
 \boxed{Vh(s,t)=h(D_Vs,t)+h(s,D_Vt).}
$$

This is the [metric-compatible connection](../../../../../metric-connection.md) condition with the sesquilinear convention fixed.

Apply the smooth [Gram-Schmidt process](../../../../../gram-schmidt-process.md) to a local frame to obtain an $h$-orthonormal smooth frame $s_1,\ldots,s_r$. Positivity guarantees that all normalization denominators are nonzero and depend smoothly on the base point. Write $Ds_j=\sum_i A_{ij}s_i$. Differentiating $h(s_i,s_j)=\delta_{ij}$ and using compatibility gives

$$
 A_{ji}(V)+\overline{A_{ij}(V)}=0
$$

for every real $V$. Thus $\boxed{A(V)^\dagger=-A(V)}$: the connection matrix is skew-Hermitian. This [smooth unitary frame for a Hermitian connection](../../../../../smooth-unitary-frame-for-a-hermitian-connection.md) is generally not holomorphic; the requested local-frame assertion requires only a smooth frame.

The [holomorphic dual vector bundle](../../../../../holomorphic-dual-vector-bundle.md) $E^*$ is obtained by dualizing fibres and using transition matrices $g_{ij}^{-T}$ when $E$ has transitions $g_{ij}$. Their entries are holomorphic because matrix inversion is holomorphic on $GL_r(\mathbb C)$. Their cocycle property follows from preservation of the fibrewise evaluation pairing, defining the natural holomorphic bundle with fibre $(E_x)^*$.

The [conjugate vector bundle](../../../../../conjugate-vector-bundle.md) $\overline E$ has the same underlying real fibres but opposite scalar action: $\lambda\cdot\overline v=\overline{\overline\lambda v}$. Its smooth transition matrices are $\overline{g_{ij}}$; they need not be holomorphic on $X$. The conjugate bundle is used here as a smooth complex bundle, whereas $E^*$ is holomorphic.

Define the smooth dual tensor $H$ by

$$
 H(s\otimes\overline t)=h(s,t).
$$

It is complex-linear in each tensor factor, because conjugating the second bundle converts the conjugate-linearity of $h$ into linearity. Thus $H\in\Gamma((E\otimes\overline E)^*)$.

The [conjugate connection](../../../../../conjugate-connection.md) is defined on real [vector fields](../../../../../vector-field.md) by $\overline D_V(\overline s)=\overline{D_Vs}$ and extended complex-linearly on the conjugate bundle. The [tensor product connection](../../../../../tensor-product-connection.md) is

$$
 D_\otimes(s\otimes\overline t)=Ds\otimes\overline t+s\otimes\overline{Dt}.
$$

Its [dual connection](../../../../../dual-connection.md) $D_0$ is uniquely characterized by

$$
 (D_{0,V}H)(u)=V[H(u)]-H(D_{\otimes,V}u).
$$

The Leibniz rule makes this a genuine connection on $(E\otimes\overline E)^*$. Evaluate it on the decomposable tensor $u=s\otimes\overline t$:

$$
 \boxed{(D_{0,V}H)(s\otimes\overline t)
 =Vh(s,t)-h(D_Vs,t)-h(s,D_Vt).}
$$

Decomposable tensors span every fibre. Hence this tensor-valued one-form vanishes precisely when the compatibility identity holds for every $V,s,t$:

$$
 \boxed{D\text{ is compatible with }h\ \Longleftrightarrow\ D_0H=0.}
$$

This is [metric compatibility as parallelism of a Hermitian tensor](../../../../../metric-compatibility-as-parallelism-of-a-hermitian-tensor.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
