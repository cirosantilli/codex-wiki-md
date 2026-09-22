<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use the source's notation for the vanishing-at-zero ideal $I=\{f\in C[0,1]:f(0)=0\}$. It is the kernel of bounded evaluation at zero, hence closed. It is stable under pointwise multiplication and [complex conjugation](../../../../complex-conjugation.md), so inherits the [C-star identity](../../../../c-star-identity.md) and completeness. If it had an identity $e$, multiplication against $f(t)=t$ would give $e(t)=1$ for $t>0$, contradicting continuity and $e(0)=0$. Thus **$I$ is a non-unital [C-star subalgebra](../../../../c-star-subalgebra.md)**. This explicit meaning of the notation matters because the usual notation $C_0$ for a compact space has a different convention.

Define the [unitization](../../../../unitization-of-an-algebra.md) map by $\Phi(f,\lambda)=f+\lambda\mathbf1$. Its inverse is $h\mapsto(h-h(0),h(0))$. The specified multiplication and [involution](../../../../involution.md) are preserved by direct substitution. The pullback [norm](../../../../norm.md) $\|(f,\lambda)\|=\|f+\lambda\mathbf1\|_\infty$ is a C-star [norm](../../../../norm.md), so equals the unique [unitization](../../../../unitization-of-an-algebra.md) [norm](../../../../norm.md) supplied in the question. Therefore **$\Phi$ is a unital isometric [C-star isomorphism](../../../../c-star-isomorphism.md) onto $C[0,1]$**.

For the approximation put $h(s)=a(\sqrt s)$ on $[0,1]$, so $h$ is continuous and $h(0)=0$. The [Stone-Weierstrass theorem](../../../../stone-weierstrass-theorem.md) supplies a [polynomial](../../../../polynomial-split.md) $p(s)$ with $\|h-p\|_\infty<\varepsilon/2$. Then $b(t)=p(t^2)-p(0)$ is a [polynomial](../../../../polynomial-split.md) in the positive even powers of $t$, with zero constant term, and

$$
\boxed{\|a-b\|_\infty\leq\|h-p\|_\infty+|p(0)|<\varepsilon.}
$$

This gives exactly the required finite form.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../split.md)
5. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
