<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume a finite-dimensional memoryless [quantum channel](../../../../../../quantum-channel.md), no shared [entanglement](../../../../../../entangled-state.md), and a code of $M_n$ messages with $n^{-1}\log_2M_n\to R$. Use a uniform message $M$ to relate average and maximum error. Each permitted input is a [product state](../../../../../../product-state.md) $\rho_m^{(n)}=\bigotimes_{i=1}^n\rho_{m,i}$, giving output $\sigma_m^{(n)}=\bigotimes_i\Lambda(\rho_{m,i})$. The factors may depend on both the message and the channel use.

Let $\chi^*(\Lambda)$ denote the one-use [Holevo capacity](../../../../../../holevo-capacity.md) in the question. The [Subadditivity of Von Neumann entropy](../../../../../../subadditivity-of-von-neumann-entropy.md) for the average output, and entropy additivity for each product output, imply

$$
\begin{aligned}
\chi_n
&=S\left(\frac1{M_n}\sum_m\sigma_m^{(n)}\right)
-\frac1{M_n}\sum_m\sum_iS(\Lambda(\rho_{m,i}))\\
&\leq\sum_i\left[S\left(\frac1{M_n}\sum_m\Lambda(\rho_{m,i})\right)
-\frac1{M_n}\sum_mS(\Lambda(\rho_{m,i}))\right]
\leq n\chi^*(\Lambda).
\end{aligned}
$$

This is the key step of the [product-input classical-capacity converse](../../../../../../product-input-classical-capacity-converse.md); it does not assume that the average output itself is a product.

Bob may measure all outputs jointly. The [Holevo bound](../../../../../../holevo-s-theorem.md) still gives $I(M:\widehat M)\leq\chi_n$. Let $P_e$ be his average message-error probability. [Fano's inequality](../../../../../../fano-s-inequality.md) gives

$$
\log_2M_n=I(M:\widehat M)+H(M\mid\widehat M)
\leq n\chi^*(\Lambda)+1+P_e\log_2M_n.
$$

Since the maximum error $P_{\max}$ is at least $P_e$,

$$
\boxed{\liminf_{n\to\infty}P_{\max}
\geq1-\frac{\chi^*(\Lambda)}R>0}
$$

when $R>\chi^*(\Lambda)$. Thus the maximum error cannot vanish asymptotically.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
