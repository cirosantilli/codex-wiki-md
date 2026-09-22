<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $r=f-p_n$ be the [continuous function](../../../../../continuous-function.md) describing the error. The preceding [orthogonality](../../../../../orthogonal-vectors.md) equations say

$$
\int_{-1}^1w(x)r(x)q(x)\,dx=0\qquad(q\in\mathcal P_n).
$$

If $r$ vanishes identically, any $n+1$ distinct points work. If $r$ already has at least $n+1$ distinct zeros, the assertion also follows. Suppose instead that it has at most $n$ distinct zeros. Among its interior zeros, list those at which its sign changes as $t_1<\cdots<t_m$, where $m\leq n$, and define the [polynomial](../../../../../polynomial-split.md)

$$
q(x)=\prod_{j=1}^m(x-t_j),
$$

with $q=1$ if $m=0$. Between consecutive zeros of $r$, its sign is constant by the [intermediate value theorem](../../../../../intermediate-value-theorem.md). At each $t_j$, both $r$ and $q$ change sign; at every other zero of $r$, neither sign changes. Hence $rq$ has one fixed sign throughout $[-1,1]$ wherever it is nonzero. Replacing $q$ by $-q$ if necessary makes $rq\geq0$ everywhere.

Since $r$ is not identically zero and $q$ has only finitely many zeros, $rq$ is strictly positive on some open interval. Positivity of $w$ gives

$$
\int_{-1}^1w(x)r(x)q(x)\,dx>0,
$$

contradicting [orthogonality](../../../../../orthogonal-vectors.md) because $q\in\mathcal P_n$. Thus

$$
\boxed{f(x_i)=p_n(x_i)\text{ at at least }n+1\text{ distinct points in }[-1,1].}
$$

This is the [interpolation property of weighted least-squares polynomial approximation](../../../../../interpolation-property-of-weighted-least-squares-polynomial-approximation.md). It supplies [interpolation nodes](../../../../../interpolation-node.md) depending on $f$ and $w$, rather than nodes prescribed in advance.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
