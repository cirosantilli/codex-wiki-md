<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $D_n=\hat n_{n\uparrow}\hat n_{n\downarrow}$. On a site, empty and doubly occupied states have spin zero, while either singly occupied state has spin $1/2$. Thus

$$
\hat{\mathbf S}_n^2=\frac34(\hat n_n-2D_n),\qquad
\boxed{\hat{\mathbf S}_n^2-\frac34\hat n_n=-\frac32D_n=:\hat{\mathbf S}_n^2:.}
$$

The [on-site spin-square normal-ordering identity](../../../../../../on-site-spin-square-normal-ordering-identity.md) rewrites the interaction as $3U\sum_nD_n$. Its contact coefficient is $3U$ in this parameterization, rather than the $U$ convention often used for the [Hubbard model](../../../../../../hubbard-model.md).

Using a [fermionic coherent-state trace](../../../../../../fermionic-coherent-state-trace.md) and time slicing, replace each normal-ordered monomial by its [Grassmann field](../../../../../../grassmann-field.md) symbol. With $\xi_{\mathbf k}=\epsilon_{\mathbf k}-\mu$,

$$
\boxed{\mathcal Z=\int\mathcal D(\bar\psi,\psi)e^{-\mathcal S},\qquad
\mathcal S=\int_0^\beta d\tau\left[\sum_{\mathbf k\sigma}\bar\psi_{\mathbf k\sigma}(\partial_\tau+\xi_{\mathbf k})\psi_{\mathbf k\sigma}
+3U\sum_n\bar\psi_{n\uparrow}\bar\psi_{n\downarrow}\psi_{n\downarrow}\psi_{n\uparrow}\right].}
$$

The independent fields have antiperiodic thermal boundary conditions. [Normal ordering](../../../../../../normal-ordering.md) is crucial: the explicit $3\hat n/4$ subtraction removes the spin-square contraction, so there is no extra chemical-potential shift from it.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
