<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Differentiation](../../../../differentiation.md) satisfies $D(af+bg)=aD(f)+bD(g)$ for constant scalars $a,b$, so it is a [linear map](../../../../linear-map.md) on suitable [vector spaces](../../../../vector-space-split.md) of differentiable functions. An arbitrary set $S$ need not even be a [vector space](../../../../vector-space-split.md), and an endomorphism interpretation also requires $D(S)\subseteq S$.

For a noninvertible example, take $S=\operatorname{span}\{1,x\}$. Then $D(a+bx)=b$ and the [kernel of a linear map](../../../../kernel-of-a-linear-map-split.md) is the nonzero [linear span](../../../../linear-span.md) of $1$, so $D:S\to S$ is not injective. The [matrix](../../../../matrix.md) in this [basis](../../../../basis.md) is $\begin{pmatrix}0&1\\0&0\end{pmatrix}$.

For an invertible example, take $S=\operatorname{span}\{e^x,e^{2x}\}$. In this [basis](../../../../basis.md), $D$ has [matrix](../../../../matrix.md) $\operatorname{diag}(1,2)$, and

$$
\boxed{D^{-1}(ae^x+be^{2x})=ae^x+\frac b2e^{2x}.}
$$

Thus [differentiation](../../../../differentiation.md) is not always invertible; the domain and codomain determine the answer.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [2021 resit](../../../2021-resit-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
