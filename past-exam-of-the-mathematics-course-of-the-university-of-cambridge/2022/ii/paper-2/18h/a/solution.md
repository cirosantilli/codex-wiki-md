<h1 id="18h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

If the [minimal polynomial](../../../../../../minimal-polynomial.md) of $\gamma$ has [degree](../../../../../../degree-of-a-polynomial.md) $d$, then  
$\mathbb F_p(\gamma)$ has $p^d$ elements and is an [intermediate field](../../../../../../intermediate-field.md) of  
$L/\mathbb F_p$. The [tower law for field extensions](../../../../../../tower-law-for-field-extensions.md) gives

$$
n=[L:\mathbb F_p]
=[L:\mathbb F_p(\gamma)]d,
$$

so $d\mid n$.

The [multiplicative group of a finite field is cyclic](../../../../../../multiplicative-group-of-a-finite-field-is-cyclic.md). Choose a generator  
$\gamma$ of $L^\times$, of [order](../../../../../../order-of-a-group-element.md) $p^n-1$. If $\gamma$ lay in a proper [intermediate field](../../../../../../intermediate-field.md) of degree $d<n$, its order would [divide](../../../../../../divisibility.md) $p^d-1<p^n-1$, a contradiction. Thus  
$\mathbb F_p(\gamma)=L$ and its [minimal polynomial](../../../../../../minimal-polynomial.md) has degree $n$.

For arbitrary $r\geq1$, let $E$ be the [splitting field](../../../../../../splitting-field.md) of  
$X^{p^r}-X$ over $\mathbb F_p$. Its [roots](../../../../../../root-of-a-polynomial.md) form a [field](../../../../../../field.md): the [Frobenius endomorphism](../../../../../../frobenius-endomorphism.md) shows they are closed under [addition](../../../../../../addition.md), [subtraction](../../../../../../subtraction.md), [multiplication](../../../../../../multiplication.md), and [inversion](../../../../../../multiplicative-inverse.md). The [derivative](../../../../../../derivative.md) is $-1$, so there are exactly $p^r$ distinct roots. Thus this root field has order $p^r$. Applying the preceding generator argument supplies an element whose [minimal polynomial](../../../../../../minimal-polynomial.md) over $\mathbb F_p$ has degree $r$, proving that an [irreducible polynomial](../../../../../../irreducible-polynomial.md) of every positive degree exists.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18H](../../18h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
