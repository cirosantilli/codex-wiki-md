<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Minkowski convex body theorem](../../../../../../minkowski-s-theorem.md) states that a centrally symmetric convex measurable set in $\mathbb R^d$ of volume greater than $2^d\operatorname{covol}(\Lambda)$ contains a nonzero point of the full lattice $\Lambda$. For a compact convex body, the weak inequality also suffices: apply the strict version to $(1+\varepsilon)C$, let $\varepsilon\downarrow0$, and choose a constant subsequence of the resulting lattice points in the bounded set $2C$. Its nonzero value belongs to $C$ by closedness.

For $Q>1$, apply this borderline version with $\Lambda=\mathbb Z^2$ to

$$
C_Q=\{(u,v):|u|\le Q,\ |xu-v|\le Q^{-1}\}.
$$

The linear transformation $(u,v)\mapsto(u,xu-v)$ has [determinant](../../../../../../determinant.md) of absolute value one, so this [parallelogram](../../../../../../parallelogram.md) has area four. A nonzero [lattice point](../../../../../../lattice-point.md) $(n,m)$ satisfies $|n|\le Q$ and $|nx-m|\le Q^{-1}$. If $n=0$, then $|m|<1$, giving the forbidden zero point; hence $n\ne0$. It follows that

$$
\boxed{\left|x-\frac mn\right|\le\frac1{Q|n|}\le\frac1{n^2}.}
$$

If $x$ is irrational, these pairs cannot remain in a finite set as $Q\to\infty$: the positive errors $|nx-m|$ of any such finite set have a positive minimum, contradicting their bound $Q^{-1}$. If $x=p/q$ is rational in lowest terms with $q>0$, the pairs $(n,m)=(jq,jp)$ for $j\ge1$ have zero error and are infinitely many distinct pairs. This proves the assertion for every real $x$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
