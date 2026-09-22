<h1 id="18h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An element $\alpha$ is [separable](../../../../../../separable-algebraic-element.md) over $K$ when its [minimal polynomial](../../../../../../minimal-polynomial.md) has [distinct](../../../../../../distinct-elements.md) roots in a [splitting field](../../../../../../splitting-field.md). A [polynomial](../../../../../../polynomial-split.md) has a [repeated root](../../../../../../multiple-root.md) exactly when it has a [common root](../../../../../../common-root.md) with its [formal derivative](../../../../../../formal-derivative-in-positive-characteristic.md). Hence  
$\gcd(f,f')=1$ implies that $f$ has no repeated root and $\alpha$ is separable.

Let $f$ be the [minimal polynomial](../../../../../../minimal-polynomial.md) of $\beta$. Repeatedly factor through the [Frobenius](../../../../../../frobenius-endomorphism.md) until

$$
f(X)=g(X^{p^h}),
$$

where $g'\ne0$. Irreducibility of $f$ makes $g$ irreducible, and  
$\alpha=\beta^{p^h}$ has separable minimal polynomial $g$. Put

$$
M=K(\alpha)=K(\beta^{p^h}).
$$

Then $M/K$ is separable and

$$
[L:M]=p^h.
$$

Every $\gamma\in L=K(\beta)$ is a polynomial in $\beta$ of degree below $[L:K]$. The freshman's-dream identity gives

$$
\gamma^{p^h}\in K(\beta^{p^h})=M,
$$

so $L/M$ is [purely inseparable](../../../../../../purely-inseparable-extension.md).

Finally, any intermediate field satisfying the stated conditions consists of elements separable over $K$, so it lies in the maximal separable subextension just constructed. Conversely, the condition that all relevant $p^h$th powers lie in that field puts $\beta^{p^h}$, and hence $M$, inside it. The two inclusions prove uniqueness.

## ↑ Ancestors (11)

1. [B](../b.md)
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
