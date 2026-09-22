<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a block with nonzero typical dimension, write $P=P_\varepsilon^{(n)}$ and $Q=I-P$. Let the compressed register be a copy of the typical space plus a one-dimensional orthogonal failure flag. Choose an isometry $V:P\mathcal H^{\otimes n}\to\mathcal K_n$ onto the successful code sector, extended by zero on $Q$, and a normalized flag $|f\rangle$ orthogonal to its range. Choose any normalized vector $|\varphi\rangle$ in the source [Hilbert space](../../../../../../hilbert-space-split.md). Define

$$
\mathcal C_n(X)=VPXPV^\dagger+\operatorname{Tr}(QX)|f\rangle\langle f|,
$$



$$
\mathcal D_n(Y)=V^\dagger YV+\langle f|Y|f\rangle|\varphi\rangle\langle\varphi|.
$$

These are [CPTP maps](../../../../../../quantum-channel.md): the first performs the projective test and either encodes or prepares a flag; the second embeds the successful sector and prepares a fixed state on failure. Their trace identities follow from $V^\dagger V=P$ and $VV^\dagger+|f\rangle\langle f|=I_{\mathcal K_n}$. Thus [typical-subspace compression with a failure flag](../../../../../../typical-subspace-compression-with-a-failure-flag.md) implements

$$
\Lambda_n(X)=PXP+\operatorname{Tr}(QX)|\varphi\rangle\langle\varphi|.
$$

For a source vector $|\Psi_k\rangle$, let $a_k=\langle\Psi_k|P|\Psi_k\rangle=\alpha_k^2$. Its overlap with the decoded state is

$$
f_k=a_k^2+(1-a_k)|\langle\Psi_k|\varphi\rangle|^2\geq a_k^2\geq2a_k-1,
$$

where the final step is $(1-a_k)^2\geq0$. Averaging proves [average pure-source fidelity after typical projection](../../../../../../average-pure-source-fidelity-after-typical-projection.md):

$$
\boxed{F_n\geq\sum_kp_k^{(n)}\alpha_k^4\geq2\sum_kp_k^{(n)}\alpha_k^2-1=2\operatorname{Tr}(\rho^{(n)}P)-1.}
$$

No orthogonality of the emitted vectors was used. The code dimension is $\dim\mathcal T_\varepsilon^{(n)}+1$; the extra flag has vanishing asymptotic rate cost. Exceptional small block lengths with empty typical space can use any channel, since they do not affect reliability.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
