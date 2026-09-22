<h1 id="1/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Hilbert space](../../../../../../../hilbert-space-split.md) interpretation of a linear [inverse problem](../../../../../../../inverse-problem-split.md), with a [bounded linear operator](../../../../../../../continuous-linear-operator.md) $K:\mathcal U\to\mathcal V$. A [least-squares solution](../../../../../../../least-squares-solution-of-a-linear-inverse-problem.md) minimizes $\|Ku-f\|_{\mathcal V}$ over $u\in\mathcal U$. A [minimum-norm least-squares solution](../../../../../../../minimum-norm-least-squares-solution.md) additionally has the smallest $\mathcal U$-[norm](../../../../../../../norm.md) among all [least-squares solutions](../../../../../../../least-squares-solution-of-a-linear-inverse-problem.md). When the equation is consistent this is the smallest-[norm](../../../../../../../norm.md) exact solution.

The [least-squares solutions](../../../../../../../least-squares-solution-of-a-linear-inverse-problem.md) form a nonempty closed [affine subspace](../../../../../../../affine-subspace.md) precisely when

$$
\boxed{f\in\mathcal R(K)\oplus\mathcal R(K)^\perp.}
$$

The [closest point theorem in a Hilbert space](../../../../../../../hilbert-projection-theorem.md) then gives a unique nearest point to zero, hence a unique [minimum-norm least-squares solution](../../../../../../../minimum-norm-least-squares-solution.md). Equivalently, it is the unique [least-squares solution](../../../../../../../least-squares-solution-of-a-linear-inverse-problem.md) in $\mathcal N(K)^\perp$. If $\mathcal R(K)$ is closed, this exists for every datum; a nonclosed [operator range](../../../../../../../range-of-a-bounded-linear-operator.md) can leave some data without any [least-squares solution](../../../../../../../least-squares-solution-of-a-linear-inverse-problem.md).

For example, on the [l2 sequence space](../../../../../../../l2-sequence-space.md), take $(Ku)_n=u_n/n$ and $f_n=1/n$. The equation would require $u_n=1$ for every $n$, which is not square summable. However, setting the first $N$ coordinates of $u$ to one and the rest to zero gives

$$
\|Ku-f\|^2=\sum_{n>N}\frac1{n^2}\longrightarrow0.
$$

Thus the least-squares [infimum](../../../../../../../infimum.md) is zero but is not attained, and **no [minimum-norm least-squares solution](../../../../../../../minimum-norm-least-squares-solution.md) exists for these data**.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [1](../../../1.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
