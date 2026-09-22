<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

An [algebraic element](../../../../algebraic-element.md) is a [separable algebraic element](../../../../separable-algebraic-element.md) over $K$ if its [minimal polynomial of an algebraic element](../../../../minimal-polynomial-of-an-algebraic-element.md) has distinct roots in a [splitting field](../../../../splitting-field.md). A [field extension](../../../../field-extension.md) is a [separable extension](../../../../separable-extension.md) if all its elements are [separable algebraic elements](../../../../separable-algebraic-element.md).

The [formal derivative](../../../../formal-derivative.md) is additive and satisfies $D(X^m)=mX^{m-1}$. For monomials, $D(X^rX^s)=(r+s)X^{r+s-1}=X^rD(X^s)+X^sD(X^r)$. Distributing over the finitely many coefficients proves the [product rule](../../../../product-rule.md) $D(fg)=fDg+gDf$ over any [field](../../../../field.md). If $f=(X-\alpha)^2h$ in an extension, the rule gives $Df=2(X-\alpha)h+(X-\alpha)^2Dh$, so $Df(\alpha)=0$, including in [characteristic two](../../../../characteristic-two.md). If $f,Df$ were relatively prime in $K[X]$, the [Bézout's identity for polynomials](../../../../bezout-s-identity-for-polynomials.md) would give $uf+vDf=1$, whose evaluation at $\alpha$ is impossible. Hence they are not relatively prime.

In [characteristic zero](../../../../characteristic-zero.md), the [formal derivative](../../../../formal-derivative.md) of a positive-degree [irreducible polynomial](../../../../irreducible-polynomial.md) $m$ is nonzero and has smaller degree. Thus $\gcd(m,Dm)=1$, since an [irreducible polynomial](../../../../irreducible-polynomial.md) has no proper nonconstant factor. By the previous argument, $m$ has no repeated root. Every element of a [finite field extension](../../../../finite-field-extension.md) is algebraic, so the extension is a [separable extension](../../../../separable-extension.md).

For $K=\mathbb F_p(t)$, let $\alpha^p=t$. The characteristic-$p$ identity gives $X^p-t=(X-\alpha)^p$, so $K(\alpha)$ is already a [splitting field](../../../../splitting-field.md). It is a proper extension by the allowed no-root fact. More precisely, the [minimal polynomial of an algebraic element](../../../../minimal-polynomial-of-an-algebraic-element.md) $\alpha$ divides $X^p-t$ and, over $K(\alpha)$, equals $(X-\alpha)^r$ for some $1\le r\le p$. If $r<p$, its next-to-leading coefficient is $-r\alpha\in K$, forcing $\alpha\in K$ because $r\ne0$ in $\mathbb F_p$, a contradiction. Hence its [minimal polynomial of an algebraic element](../../../../minimal-polynomial-of-an-algebraic-element.md) is $X^p-t$, with its one root repeated $p$ times. The extension is therefore **inseparable**, of degree $p$.

By contrast, every [finite field extension](../../../../finite-field-extension.md) $L/\mathbb F_p$ is a [separable extension](../../../../separable-extension.md). If $[L:\mathbb F_p]=n$, then $|L|=p^n$. [Lagrange's theorem](../../../../lagrange-s-theorem.md) in its nonzero multiplicative [group](../../../../group-split.md) gives $a^{p^n}=a$ for all $a\in L$. Thus every element is a root of $X^{p^n}-X$, whose [formal derivative](../../../../formal-derivative.md) is $-1$; it has no repeated roots. Every [minimal polynomial of an algebraic element](../../../../minimal-polynomial-of-an-algebraic-element.md) divides this separable [polynomial](../../../../polynomial-split.md), proving the assertion.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the number theory course of the University of Oxford](../../../split.md)
5. [Number theory course of the University of Oxford](../../../../number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
