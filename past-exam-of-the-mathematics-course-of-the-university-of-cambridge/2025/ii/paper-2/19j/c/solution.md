<h1 id="19j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The induced representation is

$$
\operatorname{Ind}_H^G(V)=\mathbb C[G]\otimes_{\mathbb C[H]}V,
$$

with $G$ acting by left multiplication on the first tensor factor. If $R$ is a set of representatives for the left cosets $G/H$, then as a vector space it is $\bigoplus_{r\in R}r\otimes V$.

The operator $g$ permutes these summands. A summand indexed by $xH$ contributes to the trace exactly when $gxH=xH$, equivalently when $x^{-1}gx\in H$, and its contribution is $\chi_V(x^{-1}gx)$. Accounting for the $|H|$ representatives of each coset gives

$$
\boxed{
\chi_{\operatorname{Ind}_H^G V}(g)
=\frac1{|H|}
\sum_{\substack{x\in G\\x^{-1}gx\in H}}
\chi_V(x^{-1}gx).}
$$

For a $G$-representation $W$, restrict $W$ to $H$ in the left-hand induced representation. Define

$$
\Phi:\mathbb C[G]\otimes_{\mathbb C[H]}(W\otimes V)
\longrightarrow
W\otimes\bigl(\mathbb C[G]\otimes_{\mathbb C[H]}V\bigr)
$$

by

$$
\Phi\bigl(x\otimes(w\otimes v)\bigr)
=xw\otimes(x\otimes v).
$$

It is well-defined because both representatives of the balancing relation give

$$
xhw\otimes(x\otimes hv).
$$

It is $G$-equivariant, and its inverse is

$$
w\otimes(x\otimes v)\longmapsto
x\otimes(x^{-1}w\otimes v).
$$

Consequently

$$
\boxed{
\operatorname{Ind}_H^G(\operatorname{Res}_H^G W\otimes V)
\cong W\otimes\operatorname{Ind}_H^G(V).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [19J](../../19j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
