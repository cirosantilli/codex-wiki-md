<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Split the best [polynomial](../../../../polynomial-split.md) into its [even](../../../../even-function.md) and [odd](../../../../odd-function.md) parts, $p_n=p_e+p_o$. Both parts belong to $\Pi_n$. Since $u$ is [odd](../../../../odd-function.md), $u-p_o$ is odd and $p_e$ is even. Their product is odd, so its integral on the symmetric interval vanishes. The [orthogonality](../../../../orthogonal-vectors.md) gives

$$
\|u-p_n\|^2=\|(u-p_o)-p_e\|^2=\|u-p_o\|^2+\|p_e\|^2.
$$

The candidate $p_o$ cannot have a strictly smaller error than a minimizer. Consequently $\|p_e\|^2=0$, and continuity gives $p_e=0$. Thus $\boxed{p_n(-x)=-p_n(x)}$. For $n=0$ this means $p_0=0$, which is indeed an odd function. More generally this is [parity preservation by polynomial least-squares projection](../../../../parity-preservation-by-polynomial-least-squares-projection.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
