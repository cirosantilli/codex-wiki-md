<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In fact $J=R$, so the [quotient module](../../../../../quotient-module.md) is zero. This requires an argument using [left ideals](../../../../../left-ideal.md): a [left ideal](../../../../../left-ideal.md) is not generally closed under multiplication on the right.

Write $x=x_1$, $y=y_1$, so that $yx-xy=1$. The [commutator product rule](../../../../../commutator-product-rule.md) gives

$$
yx^2=x^2y+2x,\qquad y^2x^2=x^2y^2+4xy+2.
$$

Both $y^2x^2$ and $x^2y^2$ lie in $J=Rx^2+Ry^2$, so their difference

$$
h=y^2x^2-x^2y^2=4xy+2
$$

belongs to $J$. Multiplying on the left and subtracting another known element of the [left ideal](../../../../../left-ideal.md) gives

$$
yh-4xy^2=4(yx-xy)y+2y=6y\in J.
$$

Because the scalar $6$ is invertible in $\mathbb C$, it follows that $y\in J$, and hence $xy\in J$. Therefore $h-4xy=2\in J$, giving $1\in J$. We conclude

$$
\boxed{R/J=0,\qquad\dim_{\mathbb C}(R/J)=0.}
$$

Thus the answer is yes for every $n\geq1$. All ideal operations in the proof use left multiplication. In particular, simply replacing $J$ by the commutative [ideal](../../../../../ideal.md) $(x_1^2,\xi_1^2)$ of the [associated graded ring](../../../../../associated-graded-ring.md) would miss the lower-order consequences that force $J=R$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the non-commutative rings course of the University of Oxford](../../../../split.md)
6. [Non-commutative rings course of the University of Oxford](../../../../../non-commutative-rings-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
