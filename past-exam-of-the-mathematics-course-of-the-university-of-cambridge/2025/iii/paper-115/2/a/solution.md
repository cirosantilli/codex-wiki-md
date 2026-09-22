<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [wedge product of differential forms](../../../../../../wedge-product-of-differential-forms.md) is the alternating tensor product

$$
(\alpha\wedge\beta)(v_1,\ldots,v_{p+q})
=\frac1{p!q!}\sum_{\sigma\in S_{p+q}}\operatorname{sgn}(\sigma)
\alpha(v_{\sigma(1)},\ldots,v_{\sigma(p)})
\beta(v_{\sigma(p+1)},\ldots,v_{\sigma(p+q)}).
$$

For nonzero $\eta\in\Lambda^{n-1}((\mathbb R^n)^*)$, choose a volume form $\mu$. There is a nonzero vector $v$ with $\eta=\iota_v\mu$. Extend $v$ to a basis and use its dual coframe; then $\eta$ is a scalar multiple of $e^2\wedge\cdots\wedge e^n$, hence equals $\xi\wedge\eta_0$. The zero form is immediate.

To integrate a top form on a compact oriented $n$-manifold, choose a finite oriented atlas and a subordinate [partition of unity](../../../../../../partition-of-unity.md); integrate each compactly supported coordinate expression and sum. A smooth map pulls forms back by

$$
(\phi^*\alpha)_x(v_1,\ldots,v_p)=
\alpha_{\phi(x)}(d\phi_xv_1,\ldots,d\phi_xv_p).
$$

If $F^*\omega=\omega$ for a nowhere-zero top form, $F$ preserves its orientation. The change-of-variables theorem gives

$$
\boxed{\int_M(h\circ F)\omega
=\int_MF^*(h\omega)
=\int_Mh\omega.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
