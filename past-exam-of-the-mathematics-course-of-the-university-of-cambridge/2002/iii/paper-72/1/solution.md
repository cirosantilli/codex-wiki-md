<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use sequential semicolon indices: $X^a{}_{;kl}=\nabla_l(\nabla_kX^a)$, where the second [covariant derivative](../../../../../covariant-derivative.md) also differentiates the lower index of $\nabla_kX^a$. For a [torsion-free connection](../../../../../torsion-free-connection.md), direct expansion gives

$$
X^a{}_{;kl}=X^a{}_{,kl}+\Gamma^a{}_{bk,l}X^b+\Gamma^a{}_{bk}X^b{}_{,l}
+\Gamma^a{}_{bl}X^b{}_{,k}+\Gamma^a{}_{pl}\Gamma^p{}_{bk}X^b
-\Gamma^p{}_{kl}X^a{}_{,p}-\Gamma^p{}_{kl}\Gamma^a{}_{bp}X^b.
$$

Subtract the expression with $k,l$ exchanged. Commuting partial derivatives cancel the first term; the first-derivative terms cancel in pairs; symmetry of the lower [Christoffel symbol](../../../../../christoffel-symbol.md) indices cancels both terms containing $\Gamma^p{}_{kl}$. What remains is

$$
X^a{}_{;kl}-X^a{}_{;lk}
=\left(\Gamma^a{}_{bk,l}-\Gamma^a{}_{bl,k}
+\Gamma^a{}_{pl}\Gamma^p{}_{bk}-\Gamma^a{}_{pk}\Gamma^p{}_{bl}\right)X^b
=R^a{}_{bkl}X^b.
$$

This is the [Ricci identity](../../../../../curvature-commutator-on-a-covariant-tensor.md) with the curvature convention printed on the PDF's first page. In terms of derivative operators it is $[\nabla_l,\nabla_k]X^a=R^a{}_{bkl}X^b$; writing the operator order explicitly avoids reversing the sign.

The lower-index rule follows by applying the commutator to the scalar contraction $Y_aX^a$. Its second derivatives commute, so the [product rule](../../../../../product-rule.md) implies $Y_{a;kl}-Y_{a;lk}=-R^p{}_{akl}Y_p$. The derivative commutator is a derivation on tensor products, since the cross terms cancel. It therefore acts once on every index, with a positive sign on each upper index and a negative sign on each lower index. For an arbitrary [tensor](../../../../../tensor.md) of valence $(r,s)$,

$$
\boxed{
T^{a_1\cdots a_r}{}_{b_1\cdots b_s;kl}
-T^{a_1\cdots a_r}{}_{b_1\cdots b_s;lk}
=\sum_{\alpha=1}^rR^{a_\alpha}{}_{pkl}
T^{a_1\cdots p\cdots a_r}{}_{b_1\cdots b_s}
-\sum_{\beta=1}^sR^p{}_{b_\beta kl}
T^{a_1\cdots a_r}{}_{b_1\cdots p\cdots b_s}.}
$$

Local sums of decomposable tensors establish the formula for every [tensor field](../../../../../tensor-field.md), rather than only for a single tensor product.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 72](../../paper-72-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
