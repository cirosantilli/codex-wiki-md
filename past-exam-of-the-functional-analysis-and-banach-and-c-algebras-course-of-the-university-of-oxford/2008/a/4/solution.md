<h1 id="a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [open mapping theorem](../../../../open-mapping-theorem-functional-analysis.md) says that a bounded [surjective](../../../../surjective-function.md) [linear map](../../../../linear-map.md) $T:E\to F$ between Banach spaces is open. Here is a proof using only Baire and completeness. Surjectivity gives $F=\bigcup_{n\geq1}T(n\overline B_E)$, hence also a cover by their closures. Baire makes one such [closure](../../../../closure-topology.md) contain a ball $B(y_0,r)$. Taking differences gives $B(0,r)\subseteq\overline{T(2n\overline B_E)}$. Scaling yields some $\delta>0$ with

$$
B(0,\delta)\subseteq\overline{T(\overline B_E)}.
$$

If $\|y\|<\delta/2$, recursively use scaled versions of this inclusion to choose $x_k$ with $\|x_k\|\leq2^{-k}$ and residual $\|y-T\sum_{j=1}^kx_j\|<\delta2^{-k-1}$. The sum converges in $E$ to an element of [norm](../../../../norm.md) at most one, whose image is $y$. Thus $B(0,\delta/2)\subseteq T(\overline B_E)$, and scaling gives $B(0,\delta/4)\subseteq T(\tfrac12\overline B_E)\subseteq T(B_E)$. Translating and scaling proves openness on every open set. This proof does not use the closed graph or inverse mapping theorem.

Apply it to the evaluation map $E:X\to\ell^\infty$, $Ef=(f(z_n))_n$. It is bounded with [norm](../../../../norm.md) at most one and onto by hypothesis. Hence its image of the [unit ball](../../../../unit-ball.md) contains a ball about zero, yielding a constant $c$ and, for every $\alpha$, an interpolant $g$ with

$$
\boxed{g(z_n)=\alpha_n,\qquad\|g\|_\infty\leq c\|\alpha\|_\infty.}
$$

For completeness, scale a ball of radius $\eta$ inside $E(B_X)$ by $2\|\alpha\|_\infty/\eta$ to obtain $c=2/\eta$; zero data use $g=0$.

For each $n$, interpolate the data which are one at index $n$ and zero elsewhere, obtaining $g_n$ of [norm](../../../../norm.md) at most $c$. The supplied factorization property gives $g_n=k_nh_n$ with $\|k_n\|_\infty=\|g_n\|_\infty\leq c$. Evaluation at $z_n$ gives $1=|k_n(z_n)h_n(z_n)|\leq c|h_n(z_n)|$, so

$$
\boxed{\inf_n|h_n(z_n)|\geq1/c>0.}
$$

The three enumerated properties of $h_n$ are supplied hypotheses for this argument, rather than additional requests to prove them.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../split.md)
5. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
