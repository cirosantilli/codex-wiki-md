<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $q=1-p$, $\mu=q-p$, $\sigma=2\sqrt{pq}$, and $\phi_S(x)=\prod_{j\in S}(x_j-\mu)/\sigma$. The functions $\phi_S$ form the [p-biased product measure](../../../../../../p-biased-product-measure.md) [orthonormal basis](../../../../../../orthonormal-basis.md), so the [Fourier expansion](../../../../../../p-biased-fourier-coefficient.md) is $f=\sum_S\widehat f_p(S)\phi_S$. The normalized [discrete derivative of a Boolean function](../../../../../../discrete-derivative-of-a-boolean-function.md) satisfies

$$
D_i f=\sum_{S\ni i}\widehat f_p(S)\phi_{S\setminus\{i\}}.
$$

Applying [Parseval identity](../../../../../../parseval-identity.md) and then exchanging two finite sums gives

$$
\operatorname{Inf}_i(f)=\lVert D_i f\rVert_2^2
=\sum_{S\ni i}\widehat f_p(S)^2,
\qquad
\mathbf I(f)=\sum_S|S|\widehat f_p(S)^2.
$$

The [noise operator on the Boolean hypercube](../../../../../../noise-operator-on-the-boolean-hypercube.md) acts diagonally on the same basis: $T_\rho\phi_S=\rho^{|S|}\phi_S$. Hence the [noise stability](../../../../../../noise-stability.md) is

$$
\operatorname{Stab}_\rho(f)=\langle f,T_\rho f\rangle
=\sum_S\rho^{|S|}\widehat f_p(S)^2.
$$

Its [derivative](../../../../../../derivative.md) is

$$
\frac d{d\rho}\operatorname{Stab}_\rho(f)
=\sum_{S\ne\varnothing}|S|\rho^{|S|-1}\widehat f_p(S)^2.
$$

Taking the right-hand value at $\rho=0$ leaves exactly the [linear Fourier weight](../../../../../../linear-fourier-weight.md) $\sum_i\widehat f_p(\{i\})^2$, while taking the left-hand value at $\rho=1$ gives $\mathbf I(f)$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 168](../../../paper-168-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
