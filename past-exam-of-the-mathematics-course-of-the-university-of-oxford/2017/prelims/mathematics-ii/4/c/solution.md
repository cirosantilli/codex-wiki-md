<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If $f$ is a [continuous function](../../../../../../continuous-function.md), the [intermediate value theorem](../../../../../../intermediate-value-theorem.md) ensures that every value between $f(a)$ and $f(b)$ is attained. [Monotonicity](../../../../../../monotonic-function.md) excludes values outside that range, so $f([a,b])=[f(a),f(b)]$.

Conversely, suppose this equality of [sets](../../../../../../set-split.md) holds. At an interior point, if $f^-(x_0)<f(x_0)$, any $y$ strictly between these two numbers lies in $[f(a),f(b)]$. Yet inputs below $x_0$ have values at most $f^-(x_0)$ and inputs at or above $x_0$ have values at least $f(x_0)$, so no input attains $y$. This contradicts [surjectivity](../../../../../../surjective-function.md). The same argument excludes $f(x_0)<f^+(x_0)$, so part (b) gives [continuity](../../../../../../continuous-function.md) at every interior point.

At $a$, a strict gap $f(a)<f^+(a)$ likewise leaves every value between them unattained; hence $f^+(a)=f(a)$, giving right [continuity](../../../../../../continuous-function.md). At $b$, the corresponding argument gives $f^-(b)=f(b)$ and left [continuity](../../../../../../continuous-function.md). These are the appropriate endpoint notions on $[a,b]$. Hence

$$
\boxed{f\text{ continuous on }[a,b]\iff f([a,b])=[f(a),f(b)].}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
