<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The assertion that fails is weak compactness of the $L^1$ unit ball; the abstract [Banach-Alaoglu theorem](../../../../../../banach-alaoglu-theorem.md) for dual balls never fails. Consider the [concentration prevents weak compactness in L1](../../../../../../concentration-prevents-weak-compactness-in-l1.md) example

$$
\boxed{f_j(x)=j^n\mathbf1_{[0,1/j]^n}(x),\qquad f_j\geq0,\qquad \|f_j\|_1=1.}
$$

Suppose a subsequence converged weakly in $L^1$ to $f$. For each $m$, all sufficiently late supports lie inside $B_{1/m}(0)$. Testing against every bounded measurable function supported outside that ball shows that $f=0$ almost everywhere there. Taking the countable union over $m$ proves $f=0$ almost everywhere on $\mathbb R^n$. But testing against the bounded constant function one gives $\int f=\lim_j\int f_j=1$, a contradiction.

The same argument applies to every subnet whose indices tend to infinity, so the sequence has no weak cluster point in the ball and the ball is not weakly compact. It converges against smooth compactly supported tests to a point mass, which is not an $L^1$ density. Thus **boundedness in $L^1$ does not imply the weak compactness proved in part (b)**; concentration is the obstruction.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
