<h1 id="p/p3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The singular weight requires care about the space of admissible polynomials. Since $n\ge1$, $x^n$ has finite squared [norm](../../../../../norm.md). A [polynomial](../../../../../polynomial-split.md) $q$ has finite error relative to $x^n$ near zero exactly when $q(0)=0$: a nonzero constant term makes the integrand asymptotic to $q(0)^2/x$, whose integral diverges. If $q(0)=0$, the residual is $O(x)$ and the integrand is $O(x)$.

Thus **the full space $\Pi_{n-1}$ is not a subspace of $V$**, so the projection theorem cannot be applied to it as written. Nevertheless a unique best finite-error approximation does exist in

$$
W=\Pi_{n-1}\cap V=\operatorname{span}\{x,x^2,\ldots,x^{n-1}\}.
$$

For $n=1$, this is the zero space and the answer is $q=0$. For $n\ge2$, $W$ is finite dimensional and its [Gram matrix](../../../../../gram-matrix.md) is positive definite, because a nonzero [polynomial](../../../../../polynomial-split.md) cannot vanish on an interval. Solving the normal equations therefore gives its unique [orthogonal projection](../../../../../orthogonal-projection.md) of $x^n$. All omitted polynomials have infinite error, so this also minimizes the extended error over the full [polynomial](../../../../../polynomial-split.md) set. The distinction is **an invalid full-space projection premise, not nonexistence of every finite-error best approximation**. As throughout weighted $L^2$, use equivalence classes for the underlying measure.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [P3](../../p3.md)
3. [P](../../../p.md)
4. [2008 printed variant](../../../../2008-printed-variant-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
