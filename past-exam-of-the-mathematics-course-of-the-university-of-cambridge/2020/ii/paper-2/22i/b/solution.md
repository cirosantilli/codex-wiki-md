<h1 id="22i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For integers $m,n\ge1$, let $E_{m,n}$ contain those $f\in C([0,1])$ for which there is some $x\in[0,1]$ such that

$$
|f(y)-f(x)|\le m|y-x|
$$

whenever $|y-x|<1/n$. Compactness of $[0,1]$ shows that $E_{m,n}$ is closed in the [uniform norm](../../../../../../supremum-norm.md): for a uniformly convergent sequence, choose convergent subsequences of the corresponding witness points and pass to the limit.

Each $E_{m,n}$ has empty interior. Given $f$ and a uniform-error tolerance, first approximate $f$ by a polygonal function, then add a sufficiently small-amplitude, sufficiently high-frequency sawtooth whose slopes dominate both $m$ and every slope of the polygonal approximation. At every point, one can move a distance below $1/n$ along one adjacent linear segment and obtain a difference quotient of magnitude greater than $m$. The perturbed function lies in the prescribed ball but outside $E_{m,n}$.

If $f$ is differentiable at some point, its nearby difference quotients are bounded, so $f\in E_{m,n}$ for some $m,n$. The functions differentiable somewhere therefore form a [meagre set](../../../../../../meagre-set.md). By the [Baire category theorem](../../../../../../baire-category-theorem.md), their complement is nonempty; indeed it is dense. Thus

$$
\boxed{C([0,1])\text{ contains a nowhere differentiable continuous function}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [22I](../../22i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
