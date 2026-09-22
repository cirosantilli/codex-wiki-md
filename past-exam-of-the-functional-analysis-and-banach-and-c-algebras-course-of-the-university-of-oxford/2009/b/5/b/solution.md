<h1 id="b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An element is a [Positive element of a C-star algebra](../../../../../positive-element-of-a-c-star-algebra.md) if it is [self-adjoint](../../../../../self-adjoint-operator.md) and its spectrum lies in $[0,\infty)$, equivalently if $a=b^*b$ for some $b$.

For a normal $a$, the [continuous functional calculus](../../../../../continuous-functional-calculus.md) is the unique unital isometric \*-isomorphism $C(\sigma(a))\to C^*(1,a)$ sending the coordinate function $z$ to $a$. It respects sums, products, conjugation and the unit, satisfies $\|f(a)\|=\max_{\sigma(a)}|f|$, and has $\sigma(f(a))=f(\sigma(a))$. For [self-adjoint](../../../../../self-adjoint-operator.md) $a$ it preserves the order of real-valued functions.

The piecewise definition of $g_n$ is consistent for $n\geq2$. **At $n=1$ the printed branches conflict**, even assigning both zero and one at $t=1/2$. All the requested limit and face arguments use only $n\geq2$; discarding this first index resolves that harmless initial-index defect without altering any limit.

For $n\geq2$, interpolate linearly from $(1/(2n),0)$ to $(1/n,g(1/n))$, and from $(1-1/n,g(1-1/n))$ to $(1-1/(2n),1)$. On the middle interval the error is zero. On the left both $g$ and $g_n$ lie between zero and $g(1/n)$; on the right both lie between $g(1-1/n)$ and one. Thus

$$
\|g-g_n\|_\infty\leq\max\{g(1/n),1-g(1-1/n)\}\longrightarrow0
$$

by continuity at the endpoints.

Put $\delta=1/(2n)$. To prove the bounds on $h_n$, it suffices to show $0\leq t-\delta g_n(t)\leq1-\delta$. For $t\leq\delta$, $g_n=0$; for $t\geq1-\delta$, $g_n=1$. On the remaining interval, $\delta\leq t\leq1-\delta$ and $0\leq g_n\leq1$, so both inequalities follow. Consequently **$g_n$ and $h_n$ are positive contractions**.

For the face assertion, write $r=\|a\|$. Since $a\in[0,1_A]$ and $0\notin F$, $0<r\leq1$. If $r<1$, then $a=r(a/r)+(1-r)0$, with both endpoints in $[0,1_A]$. The face property would force $0\in F$, a contradiction. Thus $\|a\|=1$. Its spectrum contains one by positivity and the [norm](../../../../../norm.md) formula, and contains zero because it is noninvertible.

Applying functional calculus to the scalar identity gives

$$
a=\delta g_n(a)+(1-\delta)h_n(a),\qquad g_n(a),h_n(a)\in[0,1_A].
$$

Since $0<\delta<1$ and $a\in F$, the face property gives $g_n(a)\in F$. [Isometry](../../../../../isometry.md) of functional calculus gives $g_n(a)\to g(a)$ in [norm](../../../../../norm.md); closedness of $F$ therefore proves

$$
\boxed{\|a\|=1,\qquad g(a)\in F.}
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../split.md)
6. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
