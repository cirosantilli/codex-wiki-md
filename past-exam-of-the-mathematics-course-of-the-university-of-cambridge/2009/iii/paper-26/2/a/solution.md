<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Bad reduction of an elliptic curve](../../../../../../bad-reduction-of-an-elliptic-curve.md) must be tested on a [Minimal Weierstrass equation](../../../../../../minimal-weierstrass-equation.md), not inferred merely from primes dividing the displayed [elliptic-curve discriminant](../../../../../../elliptic-curve-discriminant.md). For an odd prime $p$, write $v_p(D)=2k+\epsilon$ with $\epsilon\in\{0,1\}$. The coordinate change $x=p^{2k}X$, $y=p^{3k}Y$ gives the same form with parameter $D/p^{2k}$. If $\epsilon=0$, that parameter is a unit at $p$ and its discriminant is a unit, so reduction is good.

If $\epsilon=1$, the new discriminant valuation is six. Discriminants of isomorphic Weierstrass models differ by a twelfth power under a coordinate change, so their valuations differ by a multiple of twelve. An integral model has nonnegative discriminant valuation; consequently a model of valuation six cannot be replaced by one of valuation zero. Reduction is bad. At $p=2$, oddness of $D$ makes the original discriminant valuation six, and the same argument gives [bad reduction of an elliptic curve](../../../../../../bad-reduction-of-an-elliptic-curve.md) there as well. Thus

$$
\boxed{\operatorname{Bad}(E_D)=\{2\}\cup\{p\text{ odd}:v_p(D)\text{ is odd}\}.}
$$

These are the [bad primes of a congruent number curve with odd parameter](../../../../../../bad-primes-of-a-congruent-number-curve-with-odd-parameter.md). If $D$ is squarefree this simplifies to the primes dividing $2D$. Squarefreeness is not stated in the PDF: for example, $D=9$ gives a curve isomorphic to $E_1$ by $x=9X,y=27Y$, so it has [good reduction](../../../../../../good-reduction-of-an-elliptic-curve.md) at three although the displayed discriminant is divisible by three.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
