<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $q_0$ be the [conductor of a Dirichlet character](../../../../../../conductor-of-a-dirichlet-character.md) and $\chi_0$ the inducing primitive even character. Removing the Euler factors absent from $L(s,\chi)$ gives the [imprimitive Dirichlet L-function Euler correction](../../../../../../imprimitive-dirichlet-l-function-euler-correction.md)

$$
L(s,\chi)=P(s)L(s,\chi_0),\qquad
P(s)=\prod_{\substack{p\mid q\\p\nmid q_0}}(1-\chi_0(p)p^{-s}).
$$

The primitive [functional equation](../../../../../../functional-equation.md) therefore gives

$$
L(s,\chi)=\varepsilon_{\chi_0}\left(\frac{q_0}{\pi}\right)^{1/2-s}
\frac{\Gamma((1-s)/2)}{\Gamma(s/2)}P(s)L(1-s,\overline\chi_0).
$$

Equivalently, replace the final primitive function by $L(1-s,\overline\chi)/P_{\overline\chi}(1-s)$, interpreted as a [meromorphic](../../../../../../meromorphic-function.md) identity with removable values handled by continuation. It is the [conductor of a Dirichlet character](../../../../../../conductor-of-a-dirichlet-character.md) $q_0$, rather than the possibly inflated modulus $q$, that enters the gamma factor and root number. The [complex conjugation](../../../../../../complex-conjugation.md) bar in the original PDF is lost in the converted TeX.

The zeros are those of $L(s,\chi_0)$ together with the zeros of the finite [Euler product](../../../../../../euler-product.md), and multiplicities add. Since $|\chi_0(p)|=1$ at each extra [prime](../../../../../../prime-number.md), an extra factor vanishes at the imaginary points determined by

$$
p^{-s}=\overline{\chi_0(p)}.
$$

Each extra [prime](../../../../../../prime-number.md) creates infinitely many such points. Its nonzero-imaginary points are not zeros of the primitive function: the [functional equation](../../../../../../functional-equation.md) and [nonvanishing of Dirichlet L-functions on the line one](../../../../../../nonvanishing-of-dirichlet-l-functions-on-the-line-one.md) exclude them. Thus the zero sets are identical precisely when every [prime](../../../../../../prime-number.md) dividing $q$ already divides $q_0$, making $P=1$. Increasing prime-power exponents alone can make a character imprimitive without changing its L-function. If $q_0=1$, the primitive function is zeta; the same Euler correction applies, with its [pole](../../../../../../pole.md) at one retained.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
